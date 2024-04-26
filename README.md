# EDA Project on King County Housing Details by Monali Talele

This project is about Exploratory Data Analysis for King County Housing Details. 

## Task
- Create GitHub Repository
- Explore and Get data from PostgreSQL database
- Data Cleaning
- Defining Personas of buyer and client
- New Features
- Explore Relationships
- At Least 3 Insights, at least 1 geographical
- At Least 3 recommendations for Client


## Requirements
The requirements have been stated in requirements.txt file.

pyenv
python==3.11.3
altair==5.0.1
jupyterlab==4.0.1
ipywidgets==8.0.6
matplotlib==3.7.1
pandas==2.0.2
jupyterlab-dash==0.1.0a3
seaborn==0.12.2
python-dotenv==1.0.0
psycopg2-binary==2.9.7
SQLAlchemy==2.0.15
missingno==0.5.2
folium==

## Setup
The installation of virtual environment and required packages can be done with the following commands (macOS) 

pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt

## Data
The data is available in a postgreSQL database. There are 2 tables :
King_county_house_details : Table with details of houses.
King_county_house_sales : Table with details of house sales.

Both tables are related by the house_id column

I fetch the data from postgreSQL in Data_Fetching.ipynb using psycopg. I then save the data in data/eda.csv to be used for the exploratory data analysis

## Persona Definition
For this project I defined 2 personas : The Realor and the Buyer

The Realtor works with wealthy clients and is interested in making fat commissions. They charge 6% of house sale price as commission.

The Buyer is a wealthy client with an unlimited budget, wants either 4+ bathrooms or a smaller house nearby. He wants a big lot where he can have his own tennis court & pool. The house should have proximity to a Golf Course. He prefers a historic house, which is not at the Waterfront.

## Exploratory Data Analysis
In the EDA.ipynb notebook, I fetch the data from csv, clean it, add new features, explore relationships. I then find 3 insights and 6 recommendations for the Client.
