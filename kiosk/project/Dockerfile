FROM node:16

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

RUN npm run build

RUN npm install -g serve

EXPOSE 4998

CMD ["serve", "-s", "build", "-l", "4998"]