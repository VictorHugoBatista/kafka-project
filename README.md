# Kafka Project

This project is a structure to practicing and studying the Kafka and KsqlDB environments. With container to setup Kafka, Zookeeper, KsqlDB server and KsqlDB CLI to manage Kafka.

## Producers

The producers in this project are using the help of an API rest, with a post request to send messages to a Kafka topic.

### Start producers

```bash
$ cd producers
$ npm run start
```

### Send message

```bash
$ curl --location --request POST 'http://localhost:3000/' \
--header 'Content-Type: application/json' \
--data-raw '{
    "message": "message text"
}'
```

## Consumers

The consumers is like a listeners, who will receive messages from a Kafka topic.

### Start consumers

```bash
$ cd consumers
$ npm run start
```

### Setup consumers

On `src/index.ts` file, can configure the consumers, editing their Id's and groupId's for each one.

