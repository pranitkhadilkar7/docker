### To use named volume
1. docker build --tag feedback-app:volume
2. docker run -p 3000:80 -d --rm --name feedback-node --volume feedback:/app/feedback feedback-app:volume