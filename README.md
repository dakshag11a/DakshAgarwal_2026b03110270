# Project 8: Food Delivery Operations Analytics

**Industry:** FoodTech / Logistics  
**Student:** Daksh Agarwal (ID: 2026b03110270)  
**Tools:** Python, NumPy, Pandas

## Business scenario
Evaluate delivery times, order outcomes, restaurant performance and city-level operations to identify service improvements.

## Repository contents
| File | Description |
|---|---|
| `SRS_FoodDeliveryAnalytics.docx` | Software Requirements Specification |
| `food_delivery_analysis.ipynb` | Source code and results (tasks 109 to 123) |
| `08_food_delivery.csv` | Dataset (2,000 orders, 10 columns) |
| `README.md` | This file |

## How to run
1. Open `food_delivery_analysis.ipynb` in Google Colab (File > Upload notebook).
2. Upload `08_food_delivery.csv` to the Colab session files panel.
3. Run all cells (Runtime > Run all).

## Key findings
- 2,000 orders: 82.10% delivered, 9.25% cancelled, 8.65% delayed.
- 28 missing delivery times were filled with the median of each order-status group. No duplicate Order_IDs.
- Average delivery time is similar across cities (35.65 to 36.54 minutes). Delhi has the highest cancellation rate (11.11%).
- Peak ordering hours: 10:00, 13:00, 21:00 and 18:00.
- Pizza Point has the highest total order value (INR 202,159.89).
- 15 deliveries are unusually long by the IQR rule (above 64 minutes).
- Delivery bands: Fast 31.2%, Standard 49.2%, Delayed 19.6%.

Five operational recommendations are in the last cell of the notebook and in the SRS.

## Concepts used
Core Python, a function, assert checks, Pandas (`groupby`, `pivot_table`, `value_counts(normalize=True)`), NumPy (`median`, `std`, `percentile`, `select`).
