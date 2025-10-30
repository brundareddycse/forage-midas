
JPMC Advanced Software Engineering Program - Midas Core

This project is my submission for the JPMC Advanced Software Engineering Forage program. It simulates the development and enhancement of Midas Core, a backend microservice written in Spring Boot for processing financial transactions.

Key Features

This application demonstrates a series of backend development tasks, including:

Kafka Message Consumption: The service listens to a Kafka topic (transactions) for incoming transaction messages in real-time.

Data Validation & Business Logic: Each transaction is validated against a database to:

Ensure both the sender and recipient exist.

Verify the sender has sufficient funds.

Database Integration (JPA): Valid transactions are persisted to an in-memory H2 database. User balances are updated accordingly in an atomic, transactional way.

External API Integration: The service communicates with an external Incentives API via a REST call (RestTemplate) to fetch and apply incentive bonuses to the recipient's account for each valid transaction.

Tech Stack

Language: Java

Framework: Spring Boot

Messaging: Spring Kafka

Database: Spring Data JPA & H2 (In-memory)

API Communication: Spring RestTemplate

Build & Dependency: Maven
