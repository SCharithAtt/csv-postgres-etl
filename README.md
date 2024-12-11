# CSV to SQL Database ETL Pipeline and Microservices

## Project Overview
This is a comprehensive ETL (Extract, Transform, Load) pipeline application designed to:
- Scan data sources (local/cloud storage)
- Validate and transform CSV files
- Match schemas with existing database tables
- Insert data into PostgreSQL
- Handle unmatched files
- Provide a web GUI for configuration
- Orchestrate using Airflow

## Architecture
- Microservices Architecture
- Docker Containerization
- Airflow Orchestration

## Services
1. **Data Source Scanner Service**
   - Scans specified data sources
   - Identifies CSV files

2. **Schema Matcher Service**
   - Compares CSV schemas with existing database tables

3. **Data Validator Service**
   - Validates data types
   - Transforms data as needed

4. **Database Inserter Service**
   - Inserts validated data into PostgreSQL

5. **Unmatched Files Handler Service**
   - Manages files with no matching schemas
   - Provides option to create new tables

6. **Web GUI Service**
   - Configure data sources
   - Manage ETL pipeline settings

7. **Airflow Orchestrator**
   - Schedules and manages ETL pipeline runs

## Prerequisites
- Docker
- Docker Compose
- Python 3.8+

## Setup and Installation
1. Clone the repository
2. Configure `.env` files for each service
3. Run `docker-compose up --build`

## Configuration
- Configuration files located in `/configs`
- Web GUI for dynamic configuration

## TODO
- Implement each microservice
- Create configuration interfaces
- Set up robust error handling
- Implement comprehensive logging

## Contributing
Please read CONTRIBUTING.md for details on our code of conduct and the process for submitting pull requests.

## License
This project is licensed under the MIT License - see the LICENSE.md file for details.
