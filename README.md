# Real-time-sensor-data-processing
Real time sensor data processing and analytics using Kafka and Tableau 


Built for real-world sensor-driven industries** — a scalable, cloud-based solution for ingesting, storing, cataloging, and visualizing high-frequency sensor data.


## Project Summary

This project showcases a **real-time data processing pipeline** built for sensor-intensive industries such as **Oil & Gas, Manufacturing, and Smart Infrastructure**. Designed using a blend of **Apache Kafka**, **AWS services**, and **interactive dashboards**, it supports seamless integration of sensor simulators, data streaming, and advanced analytics.

Developed as part of a systems-focused academic initiative, this pipeline demonstrates end-to-end technical fluency across data engineering, cloud architecture, and real-time analytics.



**Pipeline Flow:**

1. **Sensor Data Simulation:**  
   Simulated sensor values (e.g., pressure, temperature) generated from real-world CSV datasets.
   
2. **Data Producer:**  
   Python script acts as Kafka producer pushing records to a **Kafka broker** (hosted on Amazon EC2).

3. **Kafka Streaming:**  
   Apache Kafka handles high-throughput, low-latency streaming to the consumer layer.

4. **S3 Storage:**  
   A Kafka consumer writes incoming data to **Amazon S3** in real-time.

5. **Data Cataloging with AWS Glue:**  
   Glue Crawlers scan the S3 bucket and update the **AWS Glue Data Catalog** for schema discovery.

6. **Query with Amazon Athena:**  
   Athena enables SQL-like querying directly on raw S3 data via the Glue catalog.

7. **Interactive Dashboards in Tableau:**  
   Real-time insights visualized using **Tableau**, helping stakeholders monitor KPIs and detect anomalies.


## Tech Stack

| Layer             | Technologies Used                            |
|------------------|-----------------------------------------------|
| Data Simulation   | Python, Pandas                                |
| Streaming Broker  | Apache Kafka (EC2-hosted)                     |
| Cloud Platform    | Amazon Web Services (EC2, S3, Glue, Athena)   |
| Visualization     | Tableau                                       |
| Data Format       | CSV, JSON                                     |


> **Pre-requisites:** Python 3.10+, Kafka setup on EC2, AWS account with S3, Glue, and Athena enabled.

1. Clone the repo:
   ```bash
   git clone 'https://github.com/rasaghnak/Real-time-sensor-data-processing'
   cd sensor-data-pipeline
