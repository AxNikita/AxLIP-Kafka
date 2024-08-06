# AxLIP-Kafka

## Запуск

Для того чтобы брокер корректно запустился, необходимо выполнить следующие шаги:

1. **Запустить сбор контейнеров**:

    ```bash
    docker-compose up -d
    ```

2. **Запустить команду для создания **:

    ```bash
    docker exec -it kafka kafka-topics.sh --create --topic ax-lip-topic --bootstrap-server localhost:9998 --partitions 1 --replication-factor 1
    ```