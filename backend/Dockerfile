FROM node:18.17.1

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

RUN apt-get update && apt-get install -y sendmail

COPY . .

EXPOSE 9000

CMD ["npm", "start"]
