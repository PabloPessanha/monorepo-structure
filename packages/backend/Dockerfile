FROM node:14-slim

WORKDIR .

COPY package*.json ./

RUN npm install

COPY . .

RUN npm run build

EXPOSE 3333

CMD ["npm", "run", "start:prod"]
