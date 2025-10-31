# AirBnB-Project
Project made to showcase SQL and mainly PowerBI skills in a short timeframe (12 hours of work). The goal was to find insights, for both customers and AirBnB owners.


🏡 Airbnb Data Analytics Dashboard (SQL + Power BI)
📘 Project Overview

This project explores the Airbnb market using SQL for data preparation and modeling and Power BI for interactive visualization.
The dataset (from Kaggle: Airbnb Listings) covers thousands of listings across the Netherlands, primarily Amsterdam.

The goal was to design a complete BI workflow:

Clean and transform raw Airbnb data in PostgreSQL

Build dimensional models and feature-engineered facts

Visualize insights in Power BI using diverse chart types

Create a business-ready dashboard suitable for executive and analytical use

*I wanted to emphasise that this was a 2-day project. (10-12 hours of work). I wanted to showcase my time efficiency.*

The quality of the analysis is not so perfect, as it was mostly used to showcase the various skills possible in (basic) PowerBI.

🧮 SQL Data Preparation

All data preparation was done in PostgreSQL, organized under an analytics schema.
The process mimics a real data engineering pipeline — from raw cleaning to BI-ready facts.

Key Steps

Data Cleaning:

Used CAST, REGEXP_REPLACE, TRIM, LOWER, COALESCE, NULLIF for robust type conversions

Normalized text and standardized date formats (EU/US tolerant)

Deduplication:

Applied ROW_NUMBER() to retain only the latest listing per listing_id

Dimensional Modeling:

Created dim_host, dim_location, and dim_calendar_month

Included precomputed keys for easy Power BI joins

Feature Engineering:

Created proxies such as occupancy, revenue, and stay type (tourist vs long-term)

Added boolean flags (Wi-Fi, kitchen, AC, etc.) using pattern matching (ILIKE, regex)

Aggregation Views:

Built views for summaries, quantiles, and correlations (PERCENTILE_CONT, CORR)

Set Operations and QC:

Used INTERSECT and EXCEPT to identify logical inconsistencies

Created validation views to ensure clean joins and correct row counts

💡 Power BI Dashboard
Objectives

Prepare a visually rich, dynamic, and data-driven view of the Airbnb market

Focus on usability, storytelling, and visual variety for portfolio demonstration

Pages / Storyline

Dataset Overview: General KPIs, filters, and map visualization

Market Structure: Room types, host types, and regional mix

Pricing Insights: Price comparison, quantiles, and city-level metrics

Host Analysis: Host activity rate, tenure, and listings per host

Occupancy & Revenue: Proxies for booking behavior and revenue potential

Reviews & Amenities: Relationship between features, reviews, and satisfaction

Trends Over Time: Monthly growth, review volume, and pricing patterns

Quality Checks (QC): Logical validations and data consistency view

📊 Visuals Used (and Why)

Map Visual: Show geographic listing distribution and density

Card Visuals: Highlight KPIs (listings, hosts, avg price, revenue, reviews)

Bar / Column Charts: Compare city, room type, and host metrics

Stacked Column Charts: Visualize stay type proportions (tourist vs long-term)

Line / Area Charts: Show time-based trends for price, availability, and reviews

Matrix / Table: Cross-compare amenities and review quality

Scatter Plot: Correlate price, reviews, and host activity

Pie / Donut Charts: Show proportions for cancellation policies and room types

Decomposition Tree: Break down factors influencing pricing and ratings

Word Cloud: Highlight common amenities and key phrases

Q&A Visual: Allow natural-language exploration

KPI Cards: Display high-level indicators

Bookmarks & Drill-Throughs: Enable page navigation and listing-level deep dives

⚙ Tools & Skills Demonstrated

SQL (PostgreSQL): Data cleaning, transformation, feature creation, QC, optimization

Power BI: DAX measures, visuals, bookmarks, drill-throughs, interactivity

Data Modeling: Dimensional schema (fact + dims), keys, join management

Analytics: Time trends, quantile analysis, correlations, business segmentation

BI Storytelling: Insight-driven layout with a mix of descriptive and diagnostic visuals

- Outcome

Created a fully functional BI-ready data model

Showcased ability to handle end-to-end analytics workflow

Demonstrated Power BI proficiency through wide visual variety and clean layout

Ready to integrate as a portfolio project for business/data analyst roles

Author: Akshat Sungkur
