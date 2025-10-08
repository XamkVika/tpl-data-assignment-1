# Data Ingestion, Storage, and Processing with Python Packages

## Objective

This project demonstrates a modular Python data pipeline that handles API data ingestion, database storage, pseudonymization/anonymization, and data exploration.

- Use **SQLite** with **SQLAlchemy** and **Alembic** for migrations.
- Fetch and store structured data from a public API.
- Apply **data masking** techniques.
- Explore and summarize data with **Pandas**.
- Organize code into **modular packages and modules**.
- Manage dependencies with a **virtual environment**.

The data source for this project is the **JSONPlaceholder Users API**:  
[https://jsonplaceholder.typicode.com/users](https://jsonplaceholder.typicode.com/users)

### Project Structure

*Use proper project structure.* Your project should use packages and modules properly. Refer to the previous exercises, check also for example [Python guide](https://docs.python-guide.org/writing/structure/).

The files and modules you need to include:
```
database                # A database module to create a database
api                     # An API module to fetch data from API and save to DB
data protection         # A simple data aprotection module
main.py                 # Main script that uses modules mentioned above
requirements.txt        # Dependencies list
```


## Setup Instructions

1. Create and activate a virtual environment.
2. Initialize Alembic for database migrations.


## Part 1 – Database Design and Migration

- Inspect the JSONPlaceholder Users API and design your table schema and datatypes (id, name, username, email, city, company_name, phone, website).
- Define models and create Alembic migration scripts.


## Part 2 – Fetch and Store Data

- Fetch users from the API using the `requests` library.
- Insert the data into the database using SQLAlchemy ORM.


## Part 3 – Data masking

Create function(s) to mask the phone numbers, leave only two last digits visible.


## Part 4 – Orchestration Script

Your `main.py` should run the full pipeline step-by-step.


## Deliverables

- Complete Python project with proper structure
- db file included



## Optional Enhancements

- Add logging (INFO/WARNING/ERROR)
- Use environment variables for database path
- Add unit tests for pseudonymization functions
- Create data visualizations (e.g., users by city)
