# nginx-scale-docker-horizontally-with-nginx-load-balancing
How spawn out multiple Node.js processes/containers, and move the incoming request handler to an Nginx proxy to load balance and properly scale our Node.js app.

## Commands

1. docker build -t app-nginx .
2. docker run -d -p 8080:80 --link chicken --link steak app-nginx
3. curl localhost:8080
