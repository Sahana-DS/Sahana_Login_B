FROM node:20-alpine
WORKDIR /app

# Install only production deps
COPY package*.json ./
RUN npm ci --only=production

# Copy source
COPY . .

EXPOSE 3103
CMD ["node", "server.js"]

