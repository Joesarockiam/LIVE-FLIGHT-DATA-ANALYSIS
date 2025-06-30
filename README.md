# Live Flight Data Analysis

Real-time flight data monitoring and visualization system using OpenSky Network API and AWS services.

## Overview

This project fetches live flight data, stores it in AWS S3, and provides real-time visualizations through Power BI dashboards. Includes an alert engine for monitoring critical flight events.

## Architecture
OpenSky API → AWS Lambda → S3 → AWS Athena → Power BI
↓
Alert Engine → Email Alerts

## Features

- **Real-time Data**: Automated flight data collection from OpenSky API
- **Cloud Storage**: AWS S3 for scalable data storage
- **Visualizations**: Interactive Power BI dashboards
- **Alert System**: Monitors altitude drops, suspicious callsigns, and ground congestion

## Tech Stack

- Python (requests, boto3)
- AWS (Lambda, S3, Athena)
- Power BI
- OpenSky Network API

## Quick Setup

1. Create AWS S3 bucket
2. Deploy Lambda function with provided code
3. Configure Athena for data querying
4. Connect Power BI to Athena
5. Set up email alerts

## Usage

The system automatically fetches flight data every few minutes, stores it in S3, and updates Power BI dashboards in real-time. Email alerts are sent for critical flight events.

## Project Structure
├── lambda_function.py     # Data fetching
├── alert_engine.py       # Alert monitoring
└── powerbi_templates/    # Dashboard templates

## Author

**JOES AROCKIAM X** - Coimbatore Institute of Technology

---

*Real-time aviation data analysis for operational insights*
