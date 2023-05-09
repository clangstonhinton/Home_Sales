# Home_Sales
Utilize PySpark and Spark SQL on Google Colab, to analyze home sales data and determine key metrics.

<img width="807" height="500" alt="Screen Shot 2023-05-09 at 12 32 48 PM" src="https://github.com/clangstonhinton/Home_Sales/assets/44728723/cb7876c4-2d19-46d0-9605-a482cc28c6e1">

## Overview of the Analysis
The purpose of this analysis was to leverage PySpark and Spark SQL to analyze home sales data.

### Data Description:
 - The dataset contains information for over 33,000 homes sold between 2019-2022.  The original dataset can be found HERE.
 - The dataset has 11 columns including: id, date, date_built, price, bedrooms, bathrooms, sqft_living, sqft_lot, floors, waterfront, and view (the number of times the home was viewed).

### Approach:
 - Create a Spark Session and read in the CSV file into a dataframe
 - Preview the first 20 rows of the dataframe
 - Create temporary views of the data
 - Run queries on cached and uncached data and compare the run times
 - Partion the data and leverage parquet formatted data
 - Answer the questions below

### Key Questions & Metrics:
 1. What is the average price for a four-bedroom house solde each year?
<img width="182" alt="Screen Shot 2023-05-09 at 12 57 09 PM" src="https://github.com/clangstonhinton/Home_Sales/assets/44728723/754010ca-ed6e-4fe7-8024-addddd3a3cc5">

 2. What is the average price of a home for each year it was built that has 3 bedrooms and 3 bathrooms?
<img width="235" alt="Screen Shot 2023-05-09 at 12 57 31 PM" src="https://github.com/clangstonhinton/Home_Sales/assets/44728723/f66da5a0-a741-45e0-8e1e-6e87c7581144">

 3. What is the average price of a home for each year that has 3 bedrooms, 3 bathrooms, 2 floors and is greater than or equal to 2,000 square feet?
<img width="226" alt="Screen Shot 2023-05-09 at 12 57 56 PM" src="https://github.com/clangstonhinton/Home_Sales/assets/44728723/fab423ec-0827-4b17-9f50-c3f368d4e8da">

 4. What is the "view" rating for homes costing more than or equal to $350,000?
<img width="216" alt="Screen Shot 2023-05-09 at 12 56 22 PM" src="https://github.com/clangstonhinton/Home_Sales/assets/44728723/81ea9def-c8c3-460f-97be-ebe43c7a7705">



    
