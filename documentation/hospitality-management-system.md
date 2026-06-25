# Hospitality Management System

## Project Overview

The Hospitality Management System is a database-driven analytics project designed to improve hotel operations, booking management, guest management, room inventory, partner tracking, and reporting. The system centralizes hotel data and supports data-driven decision-making for hotel staff, administrators, and business users.

## Problem Statement

Hotels manage large volumes of booking requests, room availability, guest details, agents, pricing information, and reservation statuses. When this data is scattered across spreadsheets or disconnected systems, it can lead to inefficiencies, overbooking, reporting delays, and inconsistent decision-making.

This project solves that problem by designing a structured database system that acts as a single source of truth for hotel operations and analytics.

## Target Users

- Hotel staff
- Reservation managers
- Front desk teams
- Hotel administrators
- Database administrators
- Business analysts
- Guests using booking platforms indirectly

## Dataset

The project used a hotel booking demand dataset from Kaggle. Additional preprocessing was performed using Python, Jupyter Notebook, and Excel to prepare the dataset for database design and analytics.

## Data Preprocessing

Key preprocessing steps included:

- Handling missing values using statistical techniques such as mode imputation
- Dropping less useful or incomplete fields where appropriate
- Adding a price column based on room type and stay duration
- Adding a city column based on country-level data
- Preparing structured booking, customer, hotel, room, agent, and reservation data

## Database Design

The database was designed around key entities such as:

- Hotel details
- Customer details
- Room details
- Reservation details
- Booking details
- Agent details
- Arrival and booking-related attributes

The schema was refined across milestones to improve clarity, reduce redundancy, and support analytics more effectively.

## Normalization and BCNF

The project applied normalization principles and checked tables against Boyce-Codd Normal Form requirements. Functional dependencies were analyzed for each table. Where violations existed, the schema was decomposed to improve data integrity and eliminate unnecessary dependency issues.

Example improvement:

- `agent_id -> company_id` caused a BCNF issue inside the booking table.
- The solution was to extract agent-related attributes into a dedicated AgentDetails table.

## SQL Analytics

The project included multiple business-oriented analytics queries, such as:

- High-performing hotels by number of bookings
- Total bookings by month
- Top-performing agents by total revenue
- Hotels with high demand based on waiting list
- Average lead time by customer market segment
- Average booking price by hotel type and agent
- Average booking duration by room type
- Total bookings by country

## Performance Optimization

Indexing was introduced to improve query performance for larger datasets and complex joins. Indexes were created on important columns such as:

- `room_id`
- `agent_id`
- booking-related join fields

This helped improve the performance of analytics queries involving room details, booking durations, revenue analysis, and agent performance.

## Analytics Dashboard Concepts

The project includes dashboard-style analytics views such as:

- Top-performing agents
- Total bookings by month
- High-performing hotels by number of bookings
- Average lead time by customer segment
- Average booking price by hotel type and agent
- Booking duration and revenue by room type
- Total bookings by country

## Skills Demonstrated

- SQL and PL/SQL
- Database design
- Data normalization
- BCNF analysis
- Entity relationship modeling
- Query optimization
- Indexing
- Python preprocessing
- Analytics query design
- Dashboard-ready reporting

## Portfolio Value

This project demonstrates strong database engineering fundamentals, schema design, normalization, query optimization, and analytics thinking for real-world hospitality operations.