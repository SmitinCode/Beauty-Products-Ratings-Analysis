This project aims to analyze a dataset containing ratings for beauty products. The dataset is loaded into a DataFrame using the pandas library.

Data Exploration:

The df.describe() function provides summary statistics for numerical columns, giving insights into the distribution of ratings.
The df.head(5) function displays the first 5 rows of the dataset, giving a glimpse of the data.
The df.shape attribute reveals the dimensions of the dataset, indicating the number of rows and columns.
The df.info() function provides information about the dataset's structure, including data types and memory usage.

Data Cleaning:
The presence of missing values and duplicates is checked using df.isnull().sum() and df.duplicated().sum() respectively.

Analysis:
The number of unique users and products is determined using len(df.UserId.unique()) and len(df.ProductId.unique()).

The number of ratings per product is calculated by grouping the data by product ID and counting the ratings for each product.

A histogram of ratings distribution is plotted using plt.hist(df["Rating"]), giving insight into the distribution of ratings.

The percentage of products with a rating of 5 is calculated by dividing the number of unique products with 5-star ratings by the total number of unique products.

The product with the highest average rating is identified by calculating the mean rating for each product, sorting the results in descending order, and selecting the top product.

The number of users giving 5-star and 1-star ratings for a specific product ('0205616461') is determined by filtering the data accordingly, and a bar plot is created to visualize the results.
Conclusion:
This analysis provides valuable insights into the beauty products ratings dataset, including the distribution of ratings, popularity of products, and behavior of users. It helps in understanding factors such as product satisfaction, user preferences, and overall trends in the beauty products market.
