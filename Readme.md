### Test locally by building the Docker image (check Docker desktop app is running).
docker build . -t node-ec2-test

### Test locally by running the app. Expose port 3000 
### (we will later use Nginx reverse proxy to send HTTPS port 80 requests to localhost:3000)
docker run -p 3000:3000 node-ec2-test