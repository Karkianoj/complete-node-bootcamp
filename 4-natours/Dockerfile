FROM node:22-alpine

WORKDIR /app

COPY package.json ./
RUN npm install

COPY config.env ./
COPY server.js ./
COPY app.js ./
COPY routes/ ./routes/
COPY controllers/ ./controllers/
COPY starter/dev-data/ ./starter/dev-data/

CMD ["node", "server.js"]
