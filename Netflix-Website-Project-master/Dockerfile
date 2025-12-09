# Dockerfile for static website
FROM nginx:alpine
# Remove default nginx content (optional but safe)
RUN rm -rf /usr/share/nginx/html/*
# Copy site files
COPY . /usr/share/nginx/html
# Expose http port
EXPOSE 80
# Run nginx in foreground
CMD ["nginx", "-g", "daemon off;"]

# Use lightweight Nginx image
FROM nginx:alpine
COPY . /usr/share/nginx/html
EXPOSE 80












































