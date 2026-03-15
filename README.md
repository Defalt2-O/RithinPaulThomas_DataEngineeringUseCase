# RithinPaulThomas_DataEngineeringUseCase

This repository contains the implementation of a pipeline that ingests, transforms, and curates data into business ready metrics.

Contains:
- ADF ingestion, transformation and curation pipelines
- Data Flow Transformations and Aggregations
- Curated data
- Power BI Dashboard to showcase Server performance
- Presentation that explains the development approach briefly.

## ARCHITECTURE

### STAGING

#### INGESTION PIPELINE
  - Validate files
  - Copy to From Staging Container to Raw Container
  - Move Stage files to Archive Folder

#### TRANSFORMATION PIPELINE
  - Transform data via Databricks Notebook (Pyspark)
  - Data is cleaned, validated, hashed, and metrics are added
  - Write Transformed data to Processed Container
  - Move Raw files to Archive Folder

#### CURATION PIPELINE
  - Transformations via Data Flows to group and aggregate data
  - Grouped outputs are written to Curation Container in separate folders

Import to Power BI
   
