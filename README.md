# Real Estate ROI Prediction Model
Master's Practicum II - [Barsha Kakshapati]

## Data Sources & Access
This project integrates three primary datasets using 5-digit Zip Codes as the joining key.

### 1. Market Price Data (Target)
* **Source:** Zillow Research (ZHVI All Homes Time Series)
* **File:** `zillow_data_clean.csv`
* **Access Note:** Due to GitHub's file size limits, this file is hosted externally. 
* **Download Link:** [Zillow Research Data](https://www.zillow.com/research/data/)

### 2. Educational Infrastructure (Predictor)
* **Source:** National Center for Education Statistics (NCES)
* **File:** `school_data.csv` (Uploaded)

### 3. Socio-Economic Baseline (Predictor)
* **Source:** US Census Bureau (ACS 5-Year Estimates, Table B19013)
* **File:** `ACSDT5Y2024.B19013-Data.csv` (Uploaded)

## Integration Plan
Data will be processed in Python using Pandas to merge economic and educational indicators with housing price trends to identify high-ROI investment zones.
