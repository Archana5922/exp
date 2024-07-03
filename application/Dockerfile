# Use the official Nginx image as the base image
FROM nginx:alpine

# Copy the custom Nginx configuration file
COPY default.conf /etc/nginx/conf.d/default.conf

# Copy all files from the current directory to the Nginx html directory
COPY . /usr/share/nginx/html/

# Expose port 8000 to the outside world
EXPOSE 8000

# Start Nginx when the container starts
CMD ["nginx", "-g", "daemon off;"]
