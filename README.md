# Investigate Business Hotel - Hotel Booking Cancellation Analysis

## Overview

This project aims to analyze customer behavior in hotel bookings and its relationship with hotel booking cancellations. By uncovering trends and patterns, the analysis helps in understanding the factors that influence booking cancellations and assists in formulating strategies to improve hotel business outcomes.

## Objectives

- **Primary Goal:** Analyze the dataset to identify trends and patterns in customer behavior that impact hotel booking cancellation rates.
- **Outcome:** Provide actionable insights to enhance hotel business strategies.

## Tools & Techniques

- **Programming Language:** Python
- **Environment:** Jupyter Notebook
- **Libraries:** Pandas, Matplotlib, Seaborn
- **Methods:** Data Cleaning, Data Visualization, Trend Analysis

## Data Cleaning and Preprocessing

### Handling Missing Values

- **Children:** Replaced NaN values with `0`, assuming no children were involved in the booking.
- **City:** Replaced NaN values with `'unknown'`, indicating that the city was not specified.
- **Agent:** Replaced NaN values with `0`, assuming the customer did not book through an agent.
- **Company:** Replaced NaN values with `0`, assuming the booking was personal.

### Correcting Unsuitable Data

- **Data Types:** Changed data types from float to integer for the `children`, `agent`, and `company` columns.

### New Columns

- **total_guest:** Sum of `adults`, `children`, and `baby` columns. Rows with a total of 0 were removed.
- **stay_duration:** Sum of `stays_in_weekend_nights` and `stays_in_weekdays_nights` columns. Rows with a total of 0 were removed.

### Dropping Unnecessary Data

- Removed columns and rows that were irrelevant or did not contribute to the analysis.

## Analysis

### Booking Trends

- **Peak Months:** The highest bookings for both city and resort hotels occur in June, July, and December, coinciding with school holidays and festive seasons.
- **Low Seasons:** A significant drop in bookings is observed in August and September, with a gradual decline in other off-peak months.
- **Hotel Type Preference:** City hotels are consistently more popular than resort hotels.

### Proportion of Canceled Bookings

- **Stay Duration:** The likelihood of cancellation increases with longer booked stay durations.
- **Lead Time:** The greater the lead time between booking and check-in, the higher the probability of cancellation.

## Key Findings

1. **Seasonality:** Bookings peak during school holidays and festive seasons.
2. **City Hotels:** More popular and consistently show higher bookings compared to resort hotels.
3. **Cancellation Factors:** Longer stay durations and greater lead times increase the likelihood of cancellations.

## Recommendations

1. **Targeted Marketing:** Increase marketing efforts before peak seasons (June, July, December) to capitalize on high demand.
2. **Dynamic Pricing:** Implement pricing strategies that adjust based on demand to maximize revenue during peak seasons and attract more bookings during slower months.
3. **Promotions for Longer Stays:** Offer discounts or special deals for extended stays to reduce cancellation rates.
4. **Focus on City Hotels:** Invest in amenities, services, and marketing for city hotels to enhance their appeal and capitalize on their popularity.

## Conclusion

This analysis provides valuable insights into customer behavior and booking cancellation trends in the hotel industry. By implementing the recommended strategies, hotels can improve their booking rates and reduce cancellations, ultimately leading to better business performance.
