# Kafka-Spring-Boot-Application

This project demonstrates a basic Spring Boot application integrated with Apache Kafka. The application includes a Kafka producer that publishes messages to a Kafka topic and a Kafka consumer that listens to and processes messages from the same topic.

## Getting Started

### Prerequisites

To run this application, you need to have the following installed on your system:

- Java Development Kit (JDK) 17 or later
- Apache Kafka

## Apache Kafka Setup

Download and refer the Apache Kafka documentation from the given link: https://kafka.apache.org/quickstart

### Running Kafka

Before starting the application, ensure that Kafka is up and running. If you haven't installed Kafka yet, you can download it from the official website and follow the instructions to start the Kafka server.

### Configuration

The Kafka server address and topic name are configured in the `application.properties` file:

```properties
spring.kafka.bootstrap-servers=localhost:9092
kafka.topic=my-topic
```

Update these properties if your Kafka server is running on a different address or if you want to use a different topic name.
Running the Application

To run the application, execute the following command from the project root directory:
```
./mvnw spring-boot:run
```

The application will start, and you should see the Spring Boot banner in the console.

## Sending Messages

You can send messages to the Kafka topic using a REST endpoint. Send a POST request with a message as the request body to the following URL:

```
http://localhost:8080/publish
```

The application will publish the message to the Kafka topic, and you should see the message being processed by the Kafka consumer in the console.


## Additional Customization
You can modify the KafkaController class to add more endpoints or customize the message publishing behavior.
For more advanced Kafka configurations and features, refer to the official Spring Kafka documentation: Spring Kafka Reference Guide

👍 Contribution
1. Fork it
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -m 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create new Pull Request

Show some ❤️ and star the repository to support the project

For more contact me @Gmail,
Facing Any Problem or need any Help❔

Incase you face any problem or need any help write me in issues section.
