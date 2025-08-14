# Sakila DB Migration & Dashboard Automation

This project automates the migration of the Sakila MySQL database from a local environment to AWS Aurora MySQL in a private subnet. It includes an automated ETL pipeline using AWS Lambda that extracts data, saves query results as CSVs and manifests in S3, and visualizes the data through Amazon QuickSight dashboards.

## Folder Structure
- `/code`: Source code, Lambda functions, SQL migration scripts.
- `/output`: Generated CSV files, manifest JSON files, backups, and logs.
- `/source`: Original input data like the Sakila MySQL dump.
- `/report`: Documentation including project report, issue log, and usage instructions.

## How to Run
1. Set up AWS Aurora MySQL cluster in a private subnet.
2. Configure bastion host for secure database access.
3. Deploy and configure Lambda functions from `/code`.
4. Schedule Lambda execution with CloudWatch Events.
5. Import datasets into QuickSight using manifest files stored in `/output/manifests/`.
6. Build and explore interactive dashboards in QuickSight.

## Prerequisites
- AWS account with required IAM permissions.
- AWS CLI configured (optional but recommended).
- Python 3.8+ environment for local testing.

## Contact
Suyog Sukumar Desai  
[LinkedIn](https://linkedin.com/in/suyog-desai)  
Email: your.email@example.com
