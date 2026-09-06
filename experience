
## STEP1
Hi, I'm Shruti. I have around 4 years of experience as a Software Engineer, primarily working on backend development using Java, Spring Boot, REST APIs, Microservices, PostgreSQL, Kafka, and AWS.

Currently, I'm working at Alight Solutions, where I'm involved in developing a workflow management platform using Java 21 and Spring Boot. My work mainly involves developing REST APIs, implementing business workflows, database integration using Spring Data JPA and Hibernate, and asynchronous processing using Kafka and AWS S3.

One of the major areas I've worked on is an event driven file ingestion workflow, where files are uploaded to S3, Kafka events are generated, and downstream services process and validate those files asynchronously. I've also worked with Terraform for AWS infrastructure provisioning and implemented security using IAM, pre-signed URLs and encryption.

Before this, I was working in HCL Technologies on a Finance Management application involving customer accounts, loans and credit cards, and I also worked on migrating monolithic functionality to microservices and automating workflows using RabbitMQ.

Overall, my core strength is backend development and designing scalable, reliable services using Java, Spring Boot, Microservices, Kafka and AWS.

## STEP2
I’m currently working on an internal Workflow Management Platform for Member, Client and Entity Onboarding.
I work mainly on the backend using Java 21, Spring Boot, Spring MVC, JPA, Hibernate and PostgreSQL.
I develop REST APIs with layered architecture, DTOs, validation and global exception handling.
One of my key contributions is an asynchronous file-processing pipeline using Kafka and AWS S3.
When a user uploads a file, we generate a process ID and store the file securely in S3.
We then publish a Kafka event containing the process ID and S3 metadata.
An asynchronous service consumes the event, downloads and validates the file, and processes it.
The processed result is uploaded back to S3, and the workflow status is updated through another Kafka event.
This allows users to track the workflow status and download the final result.
I’ve also worked with pre-signed URLs, IAM, encryption and Terraform for AWS infrastructure.
For testing, I use JUnit, Mockito and Spring Mock MVC for unit and integration testing.
Overall, my main expertise is building scalable backend services using Java, Spring Boot, Microservices, Kafka and AWS.


The architecture
                  User / Workflow Portal
                           |
                           ↓
                    Load Balancer
                           |
                           ↓
                  Spring Boot APIs
                           |
             ┌─────────────┴─────────────┐
             ↓                           ↓
        PostgreSQL                     AWS S3
      Workflow Metadata              Input Files
                                         |
                                         ↓
                                  Kafka Event
                                         |
                                         ↓
                              Async Ingest Service
                                         |
                              ┌──────────┴──────────┐
                              ↓                     ↓
                         Validation              Processing
                              |                     |
                              └──────────┬──────────┘
                                         ↓
                                   PostgreSQL
                                         |
                                         ↓
                                   Result File
                                         |
                                         ↓
                                       S3
                                         |
                                         ↓
                                  Kafka Status Event
                                         |
                                         ↓
                                Workflow Portal




