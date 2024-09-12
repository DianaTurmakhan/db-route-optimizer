# Database Table Analysis and Route Optimization

## Overview

This project performs the following tasks:

- Connects to a PostgreSQL database using `psycopg2` and fetches data from several tables.
- Loads the data into Pandas DataFrames for further analysis.
- Performs route optimization using the Open Source Routing Machine (OSRM) API.

## Prerequisites

Ensure you have the following installed:

- Python 3.9+
- PostgreSQL database with relevant data
- Required Python libraries:
  - `psycopg2`
  - `pandas`
  - `folium`
  - `requests`


The script connects to a local PostgreSQL database using the following connection parameters:

Host: localhost
Port: 5432
Database: data
User: ####
Password: ####

Tables fetched from the database include:

-cars
- drivers
- spatial_ref_sys
- tc_positions_recent
- several tables under the shuttle schema

## Route Optimization
For route optimization, the project uses the OSRM (Open Source Routing Machine) API to calculate optimized routes between a start and end location (latitude/longitude).
```bash
http://router.project-osrm.org/route/v1/driving

## Running Notebook
1.Ensure your PostgreSQL database is running and populated with the necessary tables.
2.Open and execute the notebook cells to load the data, perform analysis, and calculate routes.
