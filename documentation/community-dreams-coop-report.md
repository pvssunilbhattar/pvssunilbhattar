# Community Dreams Donor Management Application

## Overview

This project is a donor management application built for Community Dreams using Streamlit, Python, MongoDB, PyMongo, Pandas, and Excel export utilities. The goal was to replace inconsistent spreadsheet-based donor tracking with a structured application that supports clean data entry, validation, record review, and reporting.

## Problem

Community Dreams was managing donor information through manual spreadsheets. This created inconsistent formats, duplicate entries, incomplete fields, and reporting challenges. A centralized application was needed to improve data quality and make records easier to manage.

## Objectives

- Build a user-friendly donor entry interface with Streamlit
- Support create, read, update, and export workflows
- Store records in MongoDB
- Validate required fields and standardize input formats
- Detect duplicate records
- Export clean data into Excel
- Provide a dashboard view for reviewing stored data

## Technology Stack

| Layer | Technology | Purpose |
|---|---|---|
| Frontend | Streamlit | Forms, dashboard widgets, validation messages, export actions |
| Backend | Python | Data cleaning, validation, workflow logic |
| Database Access | PyMongo | MongoDB connectivity |
| Persistence | MongoDB | Document-based donor record storage |
| Reporting | Pandas / Excel Writer | Excel export for reporting |

## Workflow

1. User enters or updates donor information in the Streamlit interface.
2. The application validates required fields and standardizes formats.
3. Clean records are stored in MongoDB.
4. Stored data is displayed in dashboard views.
5. Records can be exported into Excel for reporting.

## Functional Modules

| Module | Purpose |
|---|---|
| Donor Form | Create and edit donor records |
| Search and Review | Locate existing records |
| Validation Layer | Standardize and verify input data |
| Persistence Layer | Insert or update MongoDB documents |
| Dashboard | Display totals, status, and quality insights |
| Export | Generate Excel-ready reports |

## MongoDB Data Model

MongoDB was selected because form data maps naturally into document-style records. Each record includes donor details, donation information, location fields, validation status, and timestamps such as created_at and updated_at. This design supports flexible updates, audit-friendly tracking, dashboard filtering, and reporting.

## Skills Demonstrated

- Python
- Streamlit
- MongoDB
- PyMongo
- Pandas
- CRUD workflows
- Data validation
- Duplicate detection
- Dashboard development
- Excel reporting

## Portfolio Value

This project demonstrates practical full-stack data application development, MongoDB integration, data quality improvement, dashboard design, and reporting automation.