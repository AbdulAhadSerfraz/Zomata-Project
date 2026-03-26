# Data Dictionary

## Zomato Dataset Schema

This document describes all columns in the `Zomato data .csv` file.

| Column Name | Data Type | Description |
|---|---|---|
| **name** | String | Name of the restaurant |
| **online_order** | String (Yes/No) | Whether the restaurant accepts online orders |
| **book_table** | String (Yes/No) | Whether the restaurant allows table booking |
| **rate** | Float (0.0-5.0) | Average customer rating on Zomato (normalized from 5-star scale) |
| **votes** | Integer | Total number of customer votes/reviews received |
| **phone** | String | Restaurant phone number(s) |
| **location** | String | Physical location/address of the restaurant |
| **rest_type** | String | Category of restaurant service (e.g., Casual Dining, Fine Dining) |
| **cuisines** | String | Comma-separated list of cuisine types offered |
| **approx_cost(for two people)** | Integer | Approximate cost in local currency (INR) for a meal for two people |
| **listed_in(type)** | String | Zomato listing category (Dining, Cafes, Buffet, Other) |
| **listed_in(city)** | String | City where the restaurant is located |

## Data Notes

- **Rate values**: Pre-processed from "X/5" format (e.g., "4.1/5") to float (4.1)
- **Votes**: Cumulative count of customer ratings/reviews
- **Cost**: Approximate and rounded to nearest 10 or 50
- **Missing values**: Minimal; mostly complete dataset
- **Dataset size**: 151 unique restaurants
- **Time period**: Data snapshot (specific date not specified in original dataset)

## Analysis Focus Areas

- `listed_in(type)`: Primary grouping variable for restaurant type analysis
- `online_order`: Binary variable for online vs offline comparison
- `rate`: Key satisfaction metric
- `votes`: Engagement/popularity metric
- `approx_cost(for two people)`: Consumer spending analysis
