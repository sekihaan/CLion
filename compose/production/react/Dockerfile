FROM node:16.3.0-slim

WORKDIR /app

ENV PATH /app/node_modules/.bin:$PATH

COPY ./frontend/package.json ./
RUN npm install --silent
RUN npm install react-scripts -g --silent

COPY ./frontend ./

CMD ["npm", "start"]
