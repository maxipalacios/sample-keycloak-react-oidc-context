FROM node:20.12-bookworm
WORKDIR /app
COPY package.json package-lock.json ./
RUN npm install
COPY . .
RUN npm run build
CMD [ "node", "/app/dist/index.js" ]
