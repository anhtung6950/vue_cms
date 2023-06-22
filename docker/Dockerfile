# Sử dụng image chứa Node.js
FROM node:16-slim

WORKDIR /var/www

# # Create user
ARG MAP_ID
ENV MAP_ID ${MAP_ID}
# RUN usermod -G node -g node -s /bin/sh -u ${MAP_ID} node && adduser node sudo

RUN usermod -G node -g node -s /bin/sh -u ${MAP_ID} node && adduser node sudo
# Set permissions
USER node:node
