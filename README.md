# Practicum-II-Real-Estate-ROI

# Project Proposal: Data Sources Section


Data Sources & Integration Plan
This project utilizes a multi-dimensional dataset integrated at the Zip Code (ZCTA) level to predict real estate ROI. The data architecture consists of three primary layers:

Market Price Layer (Target Variable): >     * Source: Zillow Home Value Index (ZHVI)

Details: Monthly time-series data representing the typical home value for all homes in a given Zip Code, smoothed and seasonally adjusted.

Educational Infrastructure Layer (Predictor):

Source: National Center for Education Statistics (NCES) - ELSI (2024-2025)

Details: Public school directory data including school names, district (agency) names, and enrollment totals to assess neighborhood infrastructure density.

Socio-Economic Layer (Predictor):

Source: US Census Bureau, American Community Survey (ACS) 5-Year Estimates (Table B19013)

Details: Median Household Income by Zip Code Tabulation Area (ZCTA). This provides the economic baseline to correlate neighborhood wealth with property appreciation.

Integration Strategy:
All datasets will be programmatically joined in Python using a left-join on the 5-digit Zip Code. Data cleaning will involve handling the multi-row headers in Census data and aggregating school-level counts to a Zip Code-level summary.
