# Data-Analyst-Task--3
Web Scraping for Product Details

# Task 3: 
- Web Scraping for Product Details
Perform web scraping from two e-commerce websites (e.g., Amazon, Flipkart, Chroma,
Reliance Digital). Create a dynamic Python script that allows the user to search for products
and save the details (e.g., name, price, ratings) in an Excel file. Ensure the code is robust and
handles dynamic search queries.

##  Features
- **Dynamic Search Query** → User can input any product name (e.g., "Laptop", "iPhone", "Samsung S23")  
- **Multi-Website Scraping** → Collects product details from **Amazon** and **Flipkart**  
- **Data Extraction** → Scrapes:
  - Product Name  
  - Price  
  - Ratings / Reviews  
- **Data Export** → Saves results into a clean **Excel file (.xlsx)**  
- **Error Handling** → Skips missing values and handles invalid search results  

## Data Fields
- **Source** : The platform where the products are listed (e.g., Amazon).
- **Product Name**: The name and brief description of the product.
- **Price**: The price information (currently marked as "Price not available").
- **Rating**: User ratings for the products, on a scale typically from 1 to 5.

- ## Key Features
1. Automated extraction of product listings.
2. Captures detailed product metadata for comparison and analysis.
3. Handles multiple entries and pages.
4. Designed to be scalable for other e-commerce platforms.


## some steps to run & install libraries:

**Step 1: Install required libraries**
Open your terminal/Anaconda prompt and install:

pip install selenium pandas openpyxl

- You need Chrome browser and ChromeDriver.
- 
**Step 2: Selenium Script (Flipkart + Amazon)**
Save this as selenium_scraper.py

**Step 3: Run it**
python selenium_scraper.py

**Enter: product_Name ( e.g.., Samsung S24)

### It will:

- Open Flipkart & Amazon in a headless Chrome browser
- Collect product name, price, rating
- Save results to samsung_s24_products.xlsx


# Example Output (Excel):

| Website  | Product                                      | Price       | Rating |
|----------|----------------------------------------------|------------|--------|
| Flipkart | SAMSUNG Galaxy S23 5G (Phantom Black, 128GB) | ₹52,999    | 4.4    |
| Flipkart | SAMSUNG Galaxy S23 Ultra 5G (Green, 256GB)   | ₹1,24,999  | 4.6    |
| Amazon   | Samsung Galaxy S23 5G (Green, 128GB)         | ₹52,999    | 4.3    |
| Amazon   | Samsung Galaxy S23 Ultra 5G (Phantom Black)  | ₹1,24,999  | 4.6    |
