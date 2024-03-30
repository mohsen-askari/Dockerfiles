FROM node:14-alpine

WORKDIR /app

COPY package.json .
RUN npm install

COPY tsconfig.json .

COPY src .

RUN npm run build

EXPOSE 3000

CMD ["npm", "start"]

