FROM node:18

WORKDIR /app

# Copy package files
COPY package*.json ./
RUN npm install

# Copy source code
COPY . .

# Copy root .env file to backend
COPY ../.env .env

EXPOSE 5000

CMD ["node", "index.js"]
