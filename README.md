# Docker Website Project
This is a simple website served using Nginx in a Docker container. The project includes HTML, CSS, and asset files that are served as a static website.

docker build -t vilawebsite .

docker run -d -p 8080:80 --name vilawebsite -v $(pwd):/usr/share/nginx/html nginx:alpine

http://localhostip:8080

Notes:
The website is served using the Nginx web server running inside a Docker container.
Any changes made to the files in the project folder will be automatically reflected on the website without needing to rebuild the container.
