Launch the container

`docker run -d -p 80:80 myginx:v1`{{execute}}

-d: NGINX is designed to run as a background service

test: http://[[CLIENT_SUBDOMAIN]][[KATACODA_HOST]].environments.katacoda.com/
