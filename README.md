# Big Data Challenge: Home Sales Analysis

## Summary
This project analyzes home sales data using PySpark to answer key business questions. The analysis calculates average home prices based on criteria such as bedrooms, bathrooms, floors, square footage, and view ratings. It also explores performance optimization through caching and partitioning.

---

## Objectives
- Analyze home sales data to identify trends and factors impacting property values.
- Provide actionable insights to support business decisions in real estate markets.
- Optimize big data workflows for large-scale analysis using PySpark.

---

## Data Description
The dataset contains the following fields:
- **date**: Sale date of the home.
- **bedrooms**: Number of bedrooms.
- **bathrooms**: Number of bathrooms.
- **floors**: Number of floors.
- **sqft_living**: Square footage of the living space.
- **view**: View rating of the home.
- **price**: Sale price of the home.
- **date_built**: Year the home was built.

---

## Included Scripts
1. **Home_Sales.ipynb**:
   - Reads the dataset from an AWS S3 bucket.
   - Creates a temporary table for SQL queries.
   - Executes SparkSQL queries to analyze home prices.
   - Implements caching to improve query performance.
   - Partitions data by `date_built` and exports it in Parquet format.

---

## Requirements

### Prerequisites
To run this project, ensure the following software is installed on your machine:
- **Java**: Required for running Apache Spark. Install Java 8 or later.
- **Apache Spark**: The core engine for processing big data.
- **Hadoop**: Required for Spark to handle file systems like HDFS.

### Installing Required Libraries
Once the prerequisites are installed, ensure you have Python and the following libraries:
```bash
pip install pyspark findspark
```

## Instructions
1. Open the `Home_Sales.ipynb` notebook in Jupyter Notebook or any compatible IDE.
2. Run the cells sequentially to execute the analysis.

---

## Features

### Data Analysis
Perform SparkSQL queries to calculate average home prices based on bedrooms, bathrooms, square footage, and view ratings.

### Performance Optimization
Implement caching to enhance query speed for repeated analyses and use data partitioning by `date_built` for efficient storage and querying.

### Exporting Data
Save the processed data in Parquet format to support further analyses.

---

## Results
The analysis provided insights into home prices based on various factors like bedrooms, bathrooms, floors, square footage, and view ratings. For detailed findings, refer to the [Home Sales Analysis Report](docs/Report.md).

---

## Contributions
We welcome and appreciate contributions from the community. If you have suggestions or improvements, please open an issue or submit a pull request.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.
