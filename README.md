# Airline Big Data Streaming Pipeline

An end-to-end big data pipeline for processing airline flight data using
Kafka, Spark, HDFS, ClickHouse, and Grafana.

## Architecture

Raw Airline Data
        |
        v
      HDFS
        |
        v
   Spark Processing
        |
        v
      Kafka
        |
        v
Spark Structured Streaming
        |
        v
    ClickHouse
        |
        v
     Grafana

## Technologies

- Apache Kafka
- Apache Spark
- HDFS
- ClickHouse
- Grafana
- Docker
- Python
- SQL

## Dataset

The raw dataset is not included because of its large size.

Place the CSV files in:

data/raw/

## Running the Project

### 1. Clone the repository

git clone <your-repository-url>

cd airline-project

### 2. Start the infrastructure

docker compose up -d

### 3. Check containers

docker compose ps

### 4. Start the Kafka producer

python scripts/producer.py

### 5. Start Spark streaming



### 6. Open Grafana

Open Grafana in your browser and import the dashboard.

## Dashboard

The Grafana dashboard provides:

- Total flights
- Delayed flights
- Delay rate
- Cancellation rate
- Flights processed over time
- Flight status distribution
- Flights by airline
- Delay rate by departure hour
- Cancellation/diversion rate
- Average arrival delay