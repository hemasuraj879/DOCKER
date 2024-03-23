FROM node:14.21.3-alpine3.17
EXPOSE 8080
RUN addgroup -S cart && adduser -S cart cart
RUN echo "redis    redis" >> /etc/hosts
WORKDIR /app
RUN chown -R cart:cart /app
USER cart
COPY package.json .
COPY server.js .
RUN npm install
CMD ["node", "server.js"]