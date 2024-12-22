FROM nginx:latest

# Copy the front-end files to the appropriate directory
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the Nginx configuration file
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose the required port
EXPOSE 9000
