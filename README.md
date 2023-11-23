# Kafka Notifications

This project simluates communication between a kafka consumer and producer by using gin webframework to create two simple web-based servers for RESTFUL communication. 
The kafka broker is created from Bitnami's Docker image. 
To test the functionality simply run `docker-compose up` from the project root directory.
Then, use the go run command to start the server, and sample curl commands at the top of the producer.go and consumer.go files.
Then fetch the notifications using `curl http://localhost:8081/notifications/1` where 1 represents the id of the mock users in the producer.go file

### Future Directions

Integrate confluent UI for kafka broker to avoid curl commands
Use dynamic users from a db
