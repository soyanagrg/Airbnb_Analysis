# Airbnb Market Analysis
A data-driven analysis of Airbnb listings across 5 major cities to help hosts make informed decisions about pricing, room types, and market positioning.

## Tools Used
- Python
- Pandas
- Numpy
- Matplotlib

## Dataset
Source: Kaggle
- 292,802 original listings
- 5 cities after cleaning: London, Rome, Barcelona, Amsterdam, Bangkok
- 20 columns including price, room type, neighbourhood, availability

## Data Cleaning
- Removed columns with 90%+ missing values
- Removed listings with missing prices
- Removed price outliers using IQR method (kept 10 to 714 USD/night)
- Converted date columns to datetime format
- Filled missing reviews_per_month with 0

## Questions Analyzed
1. Which cities offer the best opportunity considering price and competition?
2. Which room type is most common and how do prices compare?
3. Which neighbourhoods command the highest prices per city?
4. Do professional hosts charge more than single listing hosts?
5. What is the relationship between availability and reviews?

## Key Findings
- Bangkok has the highest average price at 553.79 USD but the fewest listings, making it the best opportunity for new hosts
  <img width="989" height="590" alt="Average Price vs Competition by City" src="https://github.com/user-attachments/assets/f29d9e5c-4eb4-4eab-99c2-5d8c3455490e" />

- Entire home/apt dominates with 70% of all listings, confirming guests strongly prefer privacy
  <img width="630" height="470" alt="Room Type Distribution" src="https://github.com/user-attachments/assets/9ec84e2e-16ed-4429-b348-27bc7ca5d5ee" />

- Professional hosts charge approximately 42 USD more per night than single listing hosts
  <img width="571" height="455" alt="Host Type and their pricing in USD" src="https://github.com/user-attachments/assets/3be2a87c-9451-4b0f-9784-59c5b59d0a0a" />

- Premium neighbourhoods exist even in competitive cities like London, where location within a city matters as much as the city itself
  <img width="1790" height="985" alt="Top 5 Most Expensive Neighbourhoods by City" src="https://github.com/user-attachments/assets/2d07c50a-2db1-4b8f-9314-4876fb25d3d4" />

  

## Notes
- Paris and Sydney were excluded due to insufficient pricing data
- Availability vs Reviews analysis based on a random sample of 5,000 listings
