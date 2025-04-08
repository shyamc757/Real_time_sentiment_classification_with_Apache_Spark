# Real-Time Sentiment Analysis Pipeline with Apache Spark

This project demonstrates a complete, scalable system for tracking tweet sentiment in real time, built on top of Apache Spark and its ecosystem. It leverages tools like Databricks, Delta Lake, and MLflow to deliver an efficient and production-ready pipeline. Spark Streaming is used within a medallion architecture pattern backed by Delta Lake, enabling real-time data processing and scalable inference using a pre-packaged MLflow model. The project also includes exploratory data analysis, system monitoring, and tracking features for end-to-end visibility and performance management.

## Features

- **Spark Streaming**: Real-time processing of tweet data.  
- **Medallion Data Architecture**: Efficient data management using Delta Lake.  
- **Spark Inference at Scale**: Deploy and manage ML models at scale using MLflow.  
- **Exploratory Data Analysis**: Dive deep into data insights with interactive notebooks.  
- **System Tracking and Monitoring**: Monitor the system's performance and data flow.  

## Notebooks Description

- `includes.ipynb`: Defines paths for raw data stored in the Amazon S3 bucket and sets essential variables for the project.  
- `utilities.ipynb`: Contains helper functions for listing contents of the S3 bucket, clearing previous runs, and managing Spark streaming jobs (stop specific/all running streams).  
- `Streaming Tweet Sentiment Analysis at Scale.ipynb`: The main PySpark implementation notebook. This notebook outlines the entire end-to-end pipeline following the medallion data architecture principles.

<br><br>
<img src="https://data-science-at-scale.s3.amazonaws.com/images/pipeline.drawio.png">
<img src="https://data-science-at-scale.s3.amazonaws.com/images/notebooks.drawio.png">

## Architecture Overview

The system follows the medallion architecture paradigm:

1. **Bronze Layer**: Ingests raw streaming data into Delta Lake tables.  
2. **Silver Layer**: Cleanses and enriches data for further analysis.  
3. **Gold Layer**: Applies machine learning models to perform sentiment analysis and stores the results for reporting.

## Technologies Used

- Apache Spark  
- Databricks  
- Delta Lake  
- MLflow  
- Amazon S3  

## Getting Started

To get started with this project, clone the repository and follow the setup instructions in each notebook to configure your environment and data paths.

### Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/shyamc757/real-time-sentiment-analysis.git
   ```

2. Set Up Environment

- Install necessary dependencies.  
- Configure access to data sources and storage as required.

### Running the Pipeline

1. **Data Ingestion**: Set up the streaming data source and configure the ingestion process.  
2. **Data Processing**: Utilize Spark Streaming to process incoming data through the Bronze, Silver, and Gold layers.  
3. **Model Deployment**: Deploy the sentiment analysis model using MLflow for real-time inference.  
4. **Monitoring**: Implement monitoring tools to track system performance and data quality.

## License

Apache License - see the `LICENSE.md` file for details.

## Authors

- Shyam Shah

## Acknowledgments

- Ajay Anand, Professor, Goergen Institute for Data Science and Artificial Intelligence, University of Rochester  
- Lloyd Palum, CTO at Tenstreet True Fuel Division and Adjunct Prof at University of Rochester

#ApacheSpark #DeltaLake #Databricks #Streaming #MLflow #HuggingFace #Transformer #MedallionArchitecture #TwitterAPI #SentimentAnalysis