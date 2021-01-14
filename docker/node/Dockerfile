FROM node:15.5.0-stretch

WORKDIR /app

ENV PATH /app/node_modules/.bin:$PATH

COPY ./code/package.json ./
COPY ./code/package-lock.json ./
RUN npm install --silent
RUN npm install react-scripts@3.4.1 -g --silent

COPY ./code ./

CMD ["npm", "start"]