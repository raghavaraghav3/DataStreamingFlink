This project gets the data generated by Kafka and is processed using Flink and stored in Postgres. Use the below codes to build Kafka, Postgres and Flink images and then create a container for the images and run the program.

1. Go to postgres location. Create Postgres Image
        docker build -t postgres .
2. Go to kafka-producer location. Create Kafka Image
        docker build -t kafka-producer .
3. Go to flink-processor location. Create Flink Image
        docker build -t flink-processor .

After creating Images we have to compose up the docker

docker compose up


