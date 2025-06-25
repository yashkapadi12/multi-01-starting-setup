FROM node:18

WORKDIR /app

COPY package.json* .

RUN npm install

COPY . .
# ENV MONGODB_USERNAME root
# ENV MONGODB_PASSWORD secret
ARG DEFAULT_PORT=80
ENV PORT $DEFAULT_PORT
EXPOSE $PORT

CMD [ "npm","start" ]

