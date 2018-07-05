Launch the container

`docker run -d -p 80:80 myginx:v1`{{execute}}

-d: NGINX is designed to run as a background service

check:

`docker ps`{{execute}}

test: http://[[CLIENT_SUBDOMAIN]]-30300-[[KATACODA_HOST]].environments.katacoda.com/
