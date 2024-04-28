FROM nginx:latest

# Remove the default configuration file
RUN rm /etc/nginx/nginx.conf

# Copy the custom Nginx configuration from the host to the container
COPY nginx.conf /etc/nginx/nginx.conf

# Expose port 443 for SSL traffic
EXPOSE 443
