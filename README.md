# Swiggy Case study
### Comprehensive Data Pipeline with Azure Data Factory, Databricks and Dashboard on Restaurants Dataset | Swiggy

This project aims to build a comprehensive, scalable data pipeline to enable seamless data ingestion, transformation, and analytics for delivering business insights. The solution will integrate Azure Data Factory for managing data ingestion from diverse sources, and Databricks with PySpark and Spark-SQL for data transformation and visualization/ analytics.

<img src="https://github.com/user-attachments/assets/386c598f-d9c5-4bf0-b386-ee6966772b2c" width="40%" />

## Data


| **File Information**     | **Value**        |
|--------------------------|------------------|
| Size                     | 955.74 MiB       |

| **Restaurant Data**      |                  |
|--------------------------|------------------|
| Rows                     | 181,404          |
| Columns                  | 10               |
| Null                     | 12,031           |
| NA                       | 101              |
| Duplicates               | 19,530           |

| **Menu Data**            |                  |
|--------------------------|------------------|
| Rows                     | 13,379,782       |
| Columns                  | 5                |
| Null                     | 0                |
| NA                       | 0                |
| Duplicates               | 146,985          |




## Approach
### Data Design Pattern: Medallion Architecture
<img src="https://github.com/user-attachments/assets/f95f5ac0-6c12-448a-897d-6005922c2b6f" width="80%" />

#### Bronze layer
- Ingests raw Swiggy data from http source to Azure Data Lake Gen 2

#### Silver layer 
- Data cleanup and validation are performed in this layer and saved as Delta Table.

#### Gold layer
- This layer contains the most up-to date data, designed for business users


## Architecture
<img src="https://github.com/user-attachments/assets/8f8ef4be-3f16-4d95-af4e-4e2fb6a0b721" width="80%" />

## Final ADF Pipeline
<img src="https://github.com/user-attachments/assets/f1faea06-44fe-4fd4-a37d-0b1a076deed4" width="80%" />

### Alternate approach
<img src="https://github.com/user-attachments/assets/6accaa07-69f2-4cff-8396-2b6edf046264" width="80%" />




