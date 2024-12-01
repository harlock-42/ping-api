FROM node:18

ARG JWT_CHECKER

ENV JWT_CHECKER=${JWT_CHECKER}

WORKDIR /app

COPY package*.json ./

RUN npm install

RUN npm install -g serve

COPY . .

EXPOSE 3000

CMD ["npm", "run", "start:dev"]