### To use named volume
1. docker build --tag feedback-app:volume .
2. docker run -p 3000:80 -d --rm --name feedback-node --volume feedback:/app/feedback feedback-app:volume   --> this creates a feedback folder in local and maps it to /app/feeback
in the conatiner

### To check the active volumes
docker volume ls

### to remove volume
docker volume rm VOL_NAME

### Using Bind Mount
2. docker run -p 3000:80 -d --rm --name feedback-node --volume /Users/pranitk/Documents/Code/docker/section-3-managing-data-working-with-volume:/app/feedback --volume /app/node_modules feedback-app:volume   --> this creates a feedback folder in local and maps it to /app/feeback