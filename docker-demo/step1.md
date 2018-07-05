Copy the following snippet to the Dockerfile:

<pre class="file" data-filename="Dockerfile" data-target="replace">
FROM nginx:1.11-alpine
COPY index.html /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
</pre>

FROM: base image.
It's recommended that you always use a particular version number as your tag and manage the updating yourself.
COPY: This is extremely useful for source code and assets that you want to be deployed inside your containe
EXPOSE: With our files copied into our image and any dependencies downloaded, you need to define which port application needs to be accessible on.
CMD: defines the default command to run when a container is launched
