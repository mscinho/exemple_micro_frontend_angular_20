# Dockerfile para desenvolvimento do dashboard
FROM node:20-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 4201
CMD ["npm", "start"]
