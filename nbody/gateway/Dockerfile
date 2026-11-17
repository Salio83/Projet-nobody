FROM node:22-alpine
WORKDIR /server
COPY package.json ./
RUN npm install
COPY server.js ./

EXPOSE 3000
ENV PORT: 3000
ENV STORE_URL: http://localhost:4000
ENV LEASE_MS: 15000

CMD ["node", "server.js"]