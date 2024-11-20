# Exploring-Realtime-Streaming

## Introduction
This repository is a learning-focused adaptation of a robust end-to-end data engineering pipeline. It demonstrates how to seamlessly handle data ingestion, processing, and storage while utilizing cutting-edge technologies like Apache Airflow, Kafka, Zookeeper, Spark, Cassandra, and PostgreSQL. To ensure easy deployment and scalability, the entire setup is containerized using Docker.

## System Architecture

![Data engineering architecture](https://github.com/user-attachments/assets/79463fa1-0e28-4a60-be35-aca0ea0c41f3)

The pipeline is built using the following components:
- **Data Source**: Random user data is generated using the `randomuser.me` API.
- **Apache Airflow**: Orchestrates the pipeline and stores raw data in a PostgreSQL database.
- **Apache Kafka & Zookeeper**: Handles real-time data streaming from PostgreSQL to the processing layer.
- **Control Center & Schema Registry**: Facilitates monitoring and schema management for Kafka streams.
- **Apache Spark**: Processes the streamed data using a distributed computing framework.
- **Cassandra**: Serves as the final storage layer for processed data.

## Key Learning Outcomes
By working on this project, you will:
- Understand how to set up and manage a data pipeline using **Apache Airflow**.
- Gain hands-on experience with **real-time data streaming** using **Apache Kafka**.
- Learn distributed synchronization techniques with **Apache Zookeeper**.
- Explore advanced **data processing** methods with **Apache Spark**.
- Dive into data storage solutions using **Cassandra** and **PostgreSQL**.
- Master containerization of a full data engineering setup using **Docker**.

## Technologies Used
This project employs the following tools and frameworks:
- Apache Airflow
- Python
- Apache Kafka
- Apache Zookeeper
- Apache Spark
- Cassandra
- PostgreSQL
- Docker

## Getting Started
Follow these steps to set up and run the project on your local machine:

### Clone the Repository
1. Clone the repository:
```
git clone https://github.com/Moiz101-ch/Exploring-Realtime-Streaming.git
```

2. Navigate to the project directory:
```
cd Exploring-Realtime-Streaming  
```

3. Access the components:
   - Airflow Web UI: http://localhost:8080
   - Kafka Control Center: http://localhost:9021

### Explore the Pipeline
- The pipeline fetches data from the `randomuser.me API`.
- The data flows through PostgreSQL, Kafka, and Spark before being stored in Cassandra.

# Acknowledgments
This project draws inspiration from the original implementation by [Yusuf Ganiyu (airscholar)](https://github.com/airscholar). It has been adapted for learning purposes with some modifications.



