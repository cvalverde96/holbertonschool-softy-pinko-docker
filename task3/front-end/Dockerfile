# Use the latest version of nginx
FROM nginx:latest

# Your softy-pinko-front-end files must be copied to /var/www/html/softy-pinko-front-end on the Docker image.
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# softy-pinko-front-end.conf must be copied to the Docker image to /etc/nginx/conf.d/default.conf
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

