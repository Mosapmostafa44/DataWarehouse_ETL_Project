# Data Warehouse ETL Project

## Overview
This repository contains an SSIS (SQL Server Integration Services) project designed to extract, transform, and load data into a data warehouse. The project includes dimension tables (`Dim_Product`, `Dim_Customer`, `Dim_Date`, `Dim_Territory`) and a fact table (`Fact_Sales`).

## Table of Contents
- [Project Structure](#project-structure)
- [Key Components](#key-components) 
- [How to Use](#how-to-use)
- [Dependencies](#dependencies)

### Project Structure
### Key Components
- **Dimension Tables:**
  - `Dim_Product`: Product details with categories and subcategories.
  - `Dim_Customer`: Customer information with slowly changing dimensions.
  - `Dim_Date`: Date-related attributes for time-based analysis.
  - `Dim_Territory`: Geographical data for sales territory management.
- **Fact Table:**
  - `Fact_Sales`: Transactional data linking dimensions to capture sales metrics.
- **ETL Processes:**
  - Slowly Changing Dimensions (SCD Type 2) implemented for `Dim_Customer` and `Dim_Product`.
  - Lookups and derived columns used for data enrichment and validation.

### How to Use
1. Clone this repository.
2. Open the `.dtsx` files in SQL Server Data Tools (SSDT).
3. Configure connection managers as needed.
4. Run the packages to execute the ETL processes.

### Dependencies
- SQL Server Integration Services (SSIS)
- SQL Server Database Engine
- Excel (for some data sources)

## Contact
If you have any questions or need further assistance, feel free to reach out!
