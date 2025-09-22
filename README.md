💻 Laptop Price Prediction Project

📌 Overview
This project focuses on predicting laptop prices based on specifications, ratings, and other attributes.
I collected data by scraping laptop listings from Flipkart, cleaned and engineered the features, and performed advanced exploratory data analysis (EDA).
The next step will be building and evaluating machine learning models for laptop price prediction.

📊 Dataset
The dataset was scraped from Flipkart and contains detailed information on laptop specifications, prices, ratings, and offers.

Key columns include:
laptop_names – Full name/model
price – Final selling price (₹ INR)
mrp – Maximum retail price before discount
star_rating – Customer star rating (out of 5)
off – Discount offered (₹ / %)
number_of_ratings – Total customer ratings
number_of_review – Total reviews
Ram_GB, memory_, ssd_type – RAM and storage details
warranty_year – Warranty duration
display_inch, display_category – Display specifications
processor, generation, Operating_system, bit_type – Processor and OS details
brand, IS_Touchscreen – Brand and touchscreen availability

🛠️ Workflow
Data Collection
Scraped laptop listings from Flipkart using Python (BeautifulSoup/Requests/Selenium).

Stored raw data in CSV format.
Data Cleaning
Removed duplicates and invalid records.
Handled missing values in price, rating, and reviews.
Converted string columns (price, MRP, RAM, storage) to numeric formats.
Feature Engineering

Extracted numeric values from text fields (e.g., Ram_GB, ssd_type, display_inch).
Created categorical features (e.g., display_category from screen size, generation from processor details).
Standardized brand and OS names.
Exploratory Data Analysis (EDA)
Performed univariate, bivariate, and multivariate analysis.
Visualized distributions, outliers, correlations, and brand-specific pricing trends.

Next Step (Work in Progress 🚧)
Build machine learning models for Laptop Price Prediction using regression and ensemble methods.

🔍 Problem Definition

1️⃣ Numeric Columns (Univariate Analysis)

Column	Questions Explored
price	Distribution, min/max/mean/median/quartiles, skewness, outliers
mrp	Distribution, how many laptops have mrp = price, extreme values
star_rating	Distribution of ratings, counts below 3, 3–4, above 4, frequent rating
off	Discount distribution (min, max, mean, median), heavily vs lightly discounted laptops
number_of_ratings	Few vs high ratings, skewness, histogram/log histogram
number_of_review	Distribution, extreme review counts
Ram_GB	Distribution of RAM sizes, most common RAM size
memory_	Distribution of memory types (DDR4, LPDDR4, LPDDR5)
ssd_type	Distribution of storage sizes, most common SSD capacity
warranty_year	Distribution of warranty durations (1, 2, 3 years)
display_inch	Distribution of display sizes, most common (13", 14", 15.6", 17")
bit_type	32-bit vs 64-bit OS distribution

2️⃣ Categorical Columns (Univariate Analysis)

Column	Questions Explored

brand	Count of laptops per brand, top 5 brands
IS_Touchscreen	Count & percentage of touchscreen vs non-touchscreen laptops
processor	Distribution of processor types (Intel, AMD, Apple)
Operating_system	Count of OS types (Windows 11, Windows 10, others)
generation	CPU generations distribution (10th, 11th, 12th, etc.)
display_category	Count of laptops per display size category

📈 Current Status
✅ Data scraping completed
✅ Data cleaning & preprocessing completed
✅ Feature engineering completed
✅ Advanced EDA completed
🚧 Model building in progress

🚀 Next Steps
Train ML models (Linear Regression, Random Forest, Gradient Boosting, XGBoost, etc.)
Evaluate model performance with RMSE, R², and cross-validation
Tune hyperparameters for best performance
Deploy model for interactive predictions (possibly using Streamlit or Flask)

📚 Tech Stack
Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Plotly)
BeautifulSoup / Selenium for web scraping
Jupyter Notebook for analysis and EDA
Streamlit (planned) for deployment

👤 Author
Sohil Khan, a data enthusiast passionate about data scraping, analytics, and machine learning.
M.com | PGDBF | B.com

