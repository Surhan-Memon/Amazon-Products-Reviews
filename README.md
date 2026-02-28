# Amazon-Products-Reviews
This project focuses on analyzing Amazon customer reviews using Python, with the goal of exploring patterns in user feedback and brand performance. I worked with a dataset of 34,660 reviews, cleaned it, handled missing values, removed irrelevant columns (reviews.userCity, reviews.userProvince, reviews.id, reviews.didPurchase), and ensured no duplicates remained. Missing text fields were filled with 'Unknown' and numeric fields like reviews.rating and reviews.numHelpful were replaced with 0 when missing.

I explored the dataset with Pandas and visualized trends using Matplotlib and Seaborn. Some key analyses include:

Distribution of ratings: Most reviews were 4 or 5 stars, with very few 0 or 1 ratings.

Helpfulness votes: Explored the number of helpful votes per review, focusing on meaningful votes (0–50) and plotting a histogram.

Ratings vs helpfulness: Bar plots showed average helpfulness votes increase with higher ratings.

Review length analysis: Created a reviews.length column to study how review text length relates to ratings using boxplots.

Recommendations vs ratings: Compared whether recommended products aligned with higher ratings.

Brand insights: Calculated average ratings for each brand, visualized top brands, and analyzed which brands received the most reviews.

Time-series analysis: Converted review dates to datetime, set them as the index, and resampled by month to track how average ratings evolved over time.

For modeling preparation, I selected relevant features (brand, manufacturer, reviews.rating, reviews.text, reviews.title, reviews.numHelpful, reviews.doRecommend, reviews.dateAdded) and applied one-hot encoding to categorical columns like brand and manufacturer. The dataset is now structured and ready for building predictive models or further analysis.

This project demonstrates real-world data cleaning, feature engineering, EDA, and visualization, providing insights into customer behavior and brand performance. It’s a great practice project for beginners wanting hands-on experience with large datasets, Python data tools, and deriving actionable insights from e-commerce reviews.
