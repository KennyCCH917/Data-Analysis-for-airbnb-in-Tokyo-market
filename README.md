# Airbnb Analysis in Tokyo Market

## Project Overview

The goal is to explore the Airbnb market in Tokyo, identify high-potential districts, and provide actionable business insights for hospitality investors.

**Key objectives**

- Analyze occupancy rates, estimated revenue, and rental prices across Tokyo wards.
- Highlight premium districts (e.g., **Minato Ku** – highest rents, **Shibuya Ku** – trendy & vibrant).
- Estimate reviewer nationality distribution using reviewer names.
- Build a predictive model (Logistic Regression) for high-value listings.
- Visualise findings with interactive Folium heatmaps and Seaborn charts.

---

## Data Sources

| Source | Description |
|--------|-------------|
| **Airbnb Listings** | Public dataset (listings, calendar, reviews) from Inside Airbnb (Tokyo). |
| **External Context** | Rental price trends, population income, tourism statistics for Tokyo wards. |

> **Note:** The notebook works with a sample merged CSV. For full reproducibility download the latest data from [Inside Airbnb](http://insideairbnb.com/get-the-data.html).

---

## Key Features & Findings

| Feature | Insight |
|---------|---------|
| **Geospatial Heatmaps** | Minato Ku shows the highest concentration of high-price listings. |
| **Revenue & Occupancy** | Estimated revenue = `price × booked_days`. Minato Ku leads with > ¥11 M per listing (365-day horizon). |
| **Nationality Distribution** (sample) | Japanese ~20 %, Korean ~15 %, Chinese ~15 %, American ~10 % (derived from reviewer names). |
| **ML Model** | Logistic Regression predicts “high-value” listings (accuracy > 78 %). |
| **Business Recommendations** | Target high-income, tourist-rich wards; balance supply vs. demand; consider eco-friendly last-mile logistics. |

---

## Tech Stack

```text
Python 3.13
pandas, numpy, matplotlib, seaborn
scikit-learn (train_test_split, LogisticRegression)
folium (interactive maps)
haversine (distance calculations)
langdetect (optional language detection)
