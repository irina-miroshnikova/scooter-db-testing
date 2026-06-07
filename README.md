# Scooter Service Testing Project

This repository contains SQL checks and basic API automated tests for a scooter rental service training project.

The project demonstrates practical QA skills in database testing, SQL query writing, API test automation, and structured test documentation.

## What is tested

* Order data in the database
* Order status validation
* Data consistency checks
* API order creation
* API order retrieval by track number
* Basic positive API scenarios

## Tools and Technologies

* SQL
* PostgreSQL
* Python
* pytest
* requests
* Git / GitHub

## Project Structure

```text
scooter-db-testing/
├── api-tests/                 # API automated tests
│   ├── configuration.py        # Base URL and API endpoints
│   ├── data.py                 # Test data
│   ├── sender_stand_request.py # API request helper functions
│   ├── test_order_by_track.py  # API test for order retrieval
│   └── requirements.txt        # Project dependencies
├── sql/                       # SQL queries
│   ├── task_1_orders_in_delivery.sql
│   └── task_2_order_statuses.sql
├── results/                   # SQL query results
│   └── task_1_result.md
├── screenshots/               # Test run screenshots
│   └── api_test_passed.png
├── README.md                  # Project documentation
└── .gitignore                 # Ignored local and generated files
```

## SQL Testing Scope

The SQL part of the project includes database-level checks for scooter order data.

Main checks:

* Orders currently in delivery
* Order status calculation
* Data filtering and validation
* Result verification based on business logic

## API Testing Scope

The API part of the project includes basic automated tests for order-related functionality.

Main checks:

* Create an order via API
* Get order information by track number
* Validate response status code
* Validate response body

## How to Run API Tests

Go to the API tests directory:

```bash
cd api-tests
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run tests:

```bash
pytest
```

## QA Focus

This project focuses on combining database checks and API testing to verify application behavior from different levels.

It demonstrates the ability to check not only the user-facing behavior, but also the data layer behind the functionality.

## Notes

This is a training QA project.

No real credentials, tokens, or confidential data are stored in this repository.
