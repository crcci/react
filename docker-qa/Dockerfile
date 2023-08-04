# Dockerfile for React app
FROM node:16 AS react-builder
ARG GITHUB_TOKEN
WORKDIR /app
COPY package.json /app/package.json
COPY package-lock.json /app/package-lock.json
RUN echo $GITHUB_TOKEN
RUN npm install
COPY . .
# RUN npm run build
EXPOSE 3000
