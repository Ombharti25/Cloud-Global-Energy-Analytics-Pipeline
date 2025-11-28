Global Energy Transition Analytics: A Cloud-Native Data Pipeline
This repository contains the source code for the Cloud Technologies final assignment, implementing a scalable Extract, Transform, Load (ETL) pipeline using Apache Spark (PySpark).

Project Summary & Details
Title: Global Energy Transition Analytics: A Cloud-Native Data Pipeline

Student: Om Nilesh Bharti (A00049459)

Framework: Apache Spark 3.x (PySpark)

Core Metric: Green Energy Ratio

Architecture: The pipeline uses Programmatic Ingestion to achieve statelessness and reproducibility in a cloud environment.

🛠️ How to Reproduce the Analysis (For Marker/Grader)
The code is designed to execute immediately in a cloud notebook environment (Google Colab is recommended).

Access Environment: Open a new notebook session in Google Colab.

Open Code: Upload and open the Cloud_Energy_Analytics_Pipeline.ipynb file.

Execution: Run all cells sequentially (Runtime -> Run all). The code handles all necessary installations (!pip install pyspark findspark).

Key Transformation Logic (T-Phase)
The pipeline performs essential data cleaning and analytical calculations on the distributed cluster:

Data Filtering: Includes filtering by year >= 2000 and enforcing iso_code IS NOT NULL to address the Regional Double Counting challenge.

Imputation: Applies Zero Imputation (.fillna(0)) to sparse consumption columns.

Metric Calculation: Calculates the Green Energy Ratio and aggregates results by country.

Final Output
The script achieves the Load (L) phase by printing the final aggregated report (Top 15 Countries) to the console and saving the complete, analysis-ready dataset to the local path /content/Green_Energy_Report.

🔗 Submission Links
Video Demonstration: [PASTE YOUR VIDEO LINK HERE] (This is the primary access point for your video presentation.)
