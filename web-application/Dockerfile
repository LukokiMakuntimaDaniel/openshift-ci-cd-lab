
FROM nginxinc/nginx-unprivileged:alpine

# Remove default Nginx content
RUN rm -rf /usr/share/nginx/html/*

# Copy application files
COPY index.html /usr/share/nginx/html/
COPY style/styles.css /usr/share/nginx/html/style/styles.css

# Use unprivileged HTTP port
EXPOSE 8080

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]