# Decarbonizing Travel — Sustainability Capstone

Summer Analytics 2026, Consulting & Analytics Club, IIT Guwahati
Ruchismita Pradhan

Analysis of business travel data (Celonis) to figure out where carbon emissions come from and how to cut them, plus a model that predicts which trips will be high-carbon.

## What I found

- 65,289 trips analyzed, 178M kg CO2e total, ~2,728 kg per trip on average
- Trips booked less than 3 days before departure emit 83% more CO2e (people end up on Business Class instead of trains/economy)
- Sales team accounts for 34% of all emissions — the highest of any team
- Out-of-policy trips emit 44% more CO2e than in-policy ones

## What I'd recommend

- Require travel requests at least 3 days in advance
- Set a lower carbon cap for Sales team travel
- Flag out-of-policy trips at approval, not after booking

## Model

Trained an XGBoost classifier to predict whether a trip will be high-carbon, using route info, transport type, trip purpose, business unit, policy status, and features engineered from booking/approval timestamps.

## Files

- `Ruchismita_SummerAnalytics_Sustainability.pptx` — full presentation
- `Ruchismita_Part2_HighCarbonPrediction.ipynb` — model code
- `Ruchismita_predictions.csv` — model predictions

Tools: Python (pandas, scikit-learn, XGBoost), Celonis
