# Bajaj Finserv Health Java Qualifier Solution

Spring Boot application that automatically performs the required tasks on startup:

1. **Generates a webhook** by sending POST request to the provided endpoint
2. **Solves SQL problem** based on the last two digits of registration number
3. **Submits the solution** to the generated webhook URL with JWT authentication

## Project Structure
src/
├── main/
│ ├── java/
│ │ └── com/
│ │ └── example/
│ │ └── hiringapp/
│ │ ├── HiringAppApplication.java
│ │ ├── service/
│ │ │ ├── WebhookService.java
│ │ │ └── SqlQuestionService.java
│ │ ├── config/
│ │ │ └── AppConfig.java
│ │ └── dto/
│ │ ├── GenerateWebhookRequest.java
│ │ ├── GenerateWebhookResponse.java
│ │ └── SubmitSolutionRequest.java
│ └── resources/
│ └── application.properties
└── pom.xml

## How to Build and Run

### Prerequisites
- Java JDK 11 or later
- Maven 3.6 or later

### Build the Project
```bash
mvn clean package
