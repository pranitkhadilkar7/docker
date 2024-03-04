### To use named volume
1. docker build --tag feedback-app:volume .
2. docker run -p 3000:80 -d --rm --name feedback-node --volume feedback:/app/feedback feedback-app:volume   --> this creates a feedback folder in local and maps it to /app/feeback
in the conatiner

### To check the active volumes
docker volume ls

### to remove volume
docker volume rm VOL_NAME