Frontend Deployment Without using nginx/apche Server
  - It is Frontend Deployment using single stage in decker
  - It can be done by adding dockerfile 
        FROM node:20-alpine AS builder
				WORKDIR /app
				COPY package*.json ./
				RUN npm ci
				COPY . .
				RUN npm run build
Output pictures : 
<img width="1432" height="85" alt="Screenshot 2025-10-25 094219" src="https://github.com/user-attachments/assets/f61a63b7-dad2-4737-9af2-f90305a0913b" />
<img width="1916" height="897" alt="image" src="https://github.com/user-attachments/assets/b5c0c4cc-9be0-471f-842b-a4e6d18bac1f" />

		
	
