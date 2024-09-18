# Python_Assignment
## ETL Pipeline with Python, PostgreSQL, AWS RDS & Interactive Mapping using Folium

This project demonstrates how to build an ETL (Extract, Transform, Load) pipeline using Python to clean address data, load it into PostgreSQL (both locally and on AWS RDS), and visualize the address data on an interactive map using Folium. It’s designed to guide users through each phase of the ETL process, including data cleaning, database integration, and geographical data visualization.

## Project Overview
This project involves:

Extracting raw address data from a CSV file using Python's Pandas library.
Transforming and cleaning the data by splitting the addresses into their components (house number, city, state code, zip code).
Loading the cleaned data into PostgreSQL (both local and AWS RDS instances).
Querying the data to count addresses by state.
Visualizing the addresses on an interactive map using the Folium library.


## Technologies Used

- **Python 3.x**: For data extraction, transformation, and loading.
- **Pandas**: For data manipulation and transformation.
- **PostgreSQL**: As the database to store the address data.
- **AWS RDS**: For cloud-based PostgreSQL storage.
- **psycopg2**: Python library for PostgreSQL database connections.
- **Folium**: For visualizing geographic data on interactive maps.
- **Jupyter Notebooks**: For development and testing (optional).



## Setup Instructions

### 1. Clone the Repository
git clone (https://github.com/dost0092/Python_Assignment.git)

### 2. Install Python Dependencies
- **pandas**
- **psycopg2**
- **folium**

### 3. Set Up PostgreSQL
Install PostgreSQL on your local machine if you haven't already.
Create a PostgreSQL database:

conn = psycopg2.connect(
    host="localhost",
    database="address_db",
    user="your_postgres_user",
    password="your_postgres_password"
)

### AWS RDS PostgreSQL Setup:
Set up an AWS RDS instance with PostgreSQL.
Create a database in your RDS instance.
Update the AWS RDS connection details in the etl_pipeline.py script:

conn = psycopg2.connect(
    host="your_rds_host",
    database="address_db",
    user="your_rds_user",
    password="your_rds_password",
    port="5432"
)

## How to Run the Project

### 1. Install Jupyter Notebook

pip install notebook
cd /path/to/your/project
start jupyter notebook

Open and Run the Notebook
Cell > Run All





![alt text](https://drive.google.com/file/d/1Mrp8u9ELVec3eFQXgbP9kaOB1ufYLDhL/view?usp=sharing)



- **Medium Link:** https://medium.com/p/d68577212da5
- **Jupyter Notebook PDF Link:** https://drive.google.com/file/d/1z9eol3b38I3ctRYHkj2CmN66t7pWIspE/view?usp=sharing
- **Jupyter Notebook HTML Link:** https://drive.google.com/file/d/1-dqc70Xf7gBc7Mkb9az5EEbm9d4uo51_/view?usp=sharing
