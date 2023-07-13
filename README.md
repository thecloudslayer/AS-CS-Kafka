# AS-CS-Kafka

```docker compose up ```



## Create a topic

``` 
docker exec broker \
kafka-topics --bootstrap-server broker:9092 \
             --create \
             --topic quickstart
```





## Show data in the topic

```
docker exec --interactive --tty broker \
kafka-console-consumer --bootstrap-server broker:9092 \
                       --topic quickstart \
                       --from-beginning
```

## Send data to Aerospike 

```node write.js```
