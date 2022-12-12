FROM node:alpine
WORKDIR /app
COPY package.json ./
COPY package-lock.json ./
COPY ./ ./
RUN npm i
RUN mkdir /app/node_modules/.cache && chmod -R 777 /app/node_modules/.cache
CMD ["npm", "run", "start"]