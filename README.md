# Auto Damage Estimator -- Big Data Pipeline 🚗📊

A scalable Big Data processing and machine learning system for vehicle
damage detection and repair cost estimation. Built using Apache Spark,
EfficientNet, distributed feature extraction, and an interactive Gradio
UI.

## Project Overview

This project processes large-scale vehicle damage datasets using Big
Data technologies and builds a complete end-to-end pipeline that:

-   Ingests and processes datasets in COCO JSON format
-   Distributes feature extraction using Spark DataFrames
-   Uses EfficientNet deep learning embeddings
-   Trains ML models (Spark Pipeline + KNN)
-   Deploys an interactive Gradio-based inference system

## Key Big Data Components

### 1. Data Ingestion

-   COCO-style annotations + image dataset
-   Automatic directory traversal
-   Handling missing/corrupt JSON entries
-   Spark schema creation

### 2. Distributed Processing

-   Uses PySpark for:
    -   Parallel data loading
    -   Distributed cleaning & transformation
    -   Converting images to Spark DataFrames
    -   Partitioned parquet output

### 3. Feature Engineering

-   EfficientNet-B0 for deep feature extraction
-   Batch-based preprocessing
-   Features stored as Spark DataFrame vectors & parquet files

### 4. Machine Learning Pipeline

-   Spark ML Pipeline (VectorAssembler, classifier)
-   KNN classifier (joblib) for secondary predictions
-   Predicts damage type & repair cost

### 5. Deployment

-   Gradio web UI:
    -   Upload car image
    -   Predict damage level
    -   Estimate repair cost

## Installation

    pip install pyspark findspark gradio joblib tensorflow

## Running the Big Data Pipeline

Open:

    Project_source_code.ipynb

## Running the User Interface

Open:

    project_UI.ipynb

## License

MIT License
