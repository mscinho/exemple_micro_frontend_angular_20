# Dockerfile para desenvolvimento do store
FROM node:20-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
EXPOSE 4202
CMD ["npm", "start"]
