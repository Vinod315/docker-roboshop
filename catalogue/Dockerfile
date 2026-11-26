From node:20
# creates /app and move
WORKDIR /app

COPY package.json .
COPY *.js .

RUN nom install

ENV MONGO_URL="mongodb://mongodb:27017/catalogue" \
    MONGO = "true"

CMD ["node", "server.js"]