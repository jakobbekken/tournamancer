FROM node:20-alpine

WORKDIR /app

ENV PATH /app/node_modules/.bin:$PATH

COPY *.json ./

RUN npm install

COPY . .

EXPOSE 4321

CMD ["astro", "dev", "--host", "0.0.0.0"]
