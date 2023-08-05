# Use the official Nginx image as the base image
FROM nginx:alpine

# Copy the HTML files and other static assets to the Nginx default serving directory
COPY ./index.html /usr/share/nginx/html/
COPY ./styles.css /usr/share/nginx/html/
COPY ./img /usr/share/nginx/html/img

# Expose port 80 for HTTP traffic (default port for Nginx)
EXPOSE 80

# Start Nginx server when the container runs
CMD ["nginx", "-g", "daemon off;"]
