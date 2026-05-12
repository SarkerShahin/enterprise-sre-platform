# use the light wight Alpine version of Nginx
FROM nginx:alpine

# Remove the defualt Nginx welcome page
RUN rm /usr/share/nginx/html/*

# Copy your custom Resume HTML into teh web server directory
COPY index.html /usr/share/ngix/html/index.html
# Expose port 80 to allow web traffic to the cluster
EXPOSE 80

#Start nginx in the foreground to keep the container running
CMD ["ngix", "-g", "daemon off;"]
