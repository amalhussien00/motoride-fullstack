FROM nginx:alpine

# Remove default content
RUN rm -rf /usr/share/nginx/html/*

# Copy all frontend folders
COPY Events /usr/share/nginx/html/events
COPY Goverment /usr/share/nginx/html/goverment
COPY SHOP /usr/share/nginx/html/shop
COPY SHOPOWNER /usr/share/nginx/html/shopowner
COPY admin /usr/share/nginx/html/admin
COPY diest /usr/share/nginx/html/diest
COPY maintenance /usr/share/nginx/html/maintenance

# Expose port 80
EXPOSE 80

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]
