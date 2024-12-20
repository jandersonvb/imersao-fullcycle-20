# This is a base node image with node user and /home/node/app as working directory
FROM node:22.8.0-slim

RUN apt update && \
    apt install openssl procps -y && \
    npm install -g @nestjs/cli@10.4.9

# Create a node user
USER node

# Create the working directory
WORKDIR /home/node/app

# Copy the package.json and package-lock.json
CMD ["tail", "-f", "/dev/null"]