# Use Nginx image for the front-end
FROM nginx:latest

# Copy the front-end files to the Nginx web root
COPY ./softy-pinko-front-end /usr/share/nginx/html

# Copy the Nginx configuration file
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
