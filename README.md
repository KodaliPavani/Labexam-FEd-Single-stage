Frontend Deployment Without using nginx/apche Server
  - It is Frontend Deployment using single stage in decker
  - It can be done by adding dockerfile 
        FROM node:20-alpine AS builder
				WORKDIR /app
				COPY package*.json ./
				RUN npm ci
				COPY . .
				RUN npm run build
	
