FROM mongo

ENV MONGO_INITDB_ROOT_USERNAME=root
ENV MONGO_INITDB_ROOT_PASSWORD=example

RUN apt-get update && apt-get install -y curl

RUN curl -o /usr/local/bin/mongo-express \
    https://github.com/mongo-express/mongo-express/releases/download/0.54.0/mongo-express-amd64 && \
    chmod +x /usr/local/bin/mongo-express

EXPOSE 27017 8081

CMD ["mongo-express"]
