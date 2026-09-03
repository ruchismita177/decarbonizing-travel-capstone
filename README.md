# Decarbonizing Travel — Sustainability Capstone Project

**Summer Analytics 2026, Consulting & Analytics Club, IIT Guwahati**
Author: Ruchismita Pradhan

## Overview

An end-to-end analysis of business travel emissions for a large company (Celonis), using process-mining and machine learning to identify where carbon emissions come from and how to reduce them — followed by a predictive model that flags high-carbon trips before they happen.

## Key Findings

- **65,289 trips analyzed** → 178 million kg CO2e total, averaging 2,728 kg CO2e per trip
- Trips booked **less than 3 days before departure emit 83% more CO2e** on average (travelers end up on Business Class flights instead of trains/economy)
- **Sales is the largest emitter**, responsible for 34% of all emissions — nearly double the next-highest team
- **Out-of-policy trips emit 44% more CO2e** on average
- Fixing the booking timeline alone could save close to **50 million kg of CO2e over 3 years**

## Recommendations

1. Require travel requests at least 3 days before departure
2. Set a lower carbon cap for Sales team travel, with pre-approval for Business Class on short routes
3. Flag out-of-policy trips at the approval stage, not after booking

## Predictive Model (Part 2)

Built an **XGBoost classifier** to predict whether a trip will be "high carbon," using:
- Route info (departure/arrival country & city), transport type, trip purpose, business unit, policy status
- Engineered features from event-log timestamps: booking lead time, approval lead time, number of process events, flags for manager pre-approval / trip extensions / flight or hotel changes

## Repository Contents

| File | Description |
|---|---|
| `Ruchismita_SummerAnalytics_Sustainability.pptx` | Full presentation — business questions, insights, dashboard, and recommendations |
| `Ruchismita_Part2_HighCarbonPrediction.ipynb` | Jupyter notebook: feature engineering, model training (XGBoost), evaluation |
| `Ruchismita_predictions.csv` | Model predictions (trip-level probability of being high-carbon) |

## Tools Used

Python (pandas, scikit-learn, XGBoost), Celonis (process mining / dashboarding)

---
*Part of the Summer Analytics 2026 program run by the Consulting & Analytics Club, IIT Guwahati.*
