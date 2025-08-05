# IBM-applied-data-science-capstone-spacex

📌 Project Overview

This project is part of the **IBM Applied Data Science Capstone** and focuses on analyzing SpaceX's Falcon 9 launch records. 
The goal is to explore launch patterns, success rates, and build a machine learning model to **predict the likelihood of a successful first-stage landing**.

🛠 Tools & Technologies

- **Python 3.8+**
- **Jupyter Notebooks** (IBM Watson Studio)
- **Libraries**:  
  - `pandas`, `numpy` for data wrangling  
  -  `plotly` for data visualization  
  - `BeautifulSoup` for web scraping  
  - `scikit-learn` for machine learning  
  - `dash` for interactive dashboard  

📂 Data Sources

| Source | Description |
|--------|-------------|
| [SpaceX API](https://api.spacexdata.com/v4/launches) | Launch details (date, location, rocket, outcome) |
| Wikipedia | Falcon 9 launch records (scraped using BeautifulSoup) |
| Launch Site Geolocation | For interactive maps using Plotly |

🔍 Key Steps & Methodology

1. **Data Collection**  
   - Scraped Falcon 9 launch data from Wikipedia  
   - Retrieved additional metadata using the SpaceX REST API

2. **Data Wrangling & Cleaning**  
   - Parsed HTML tables  
   - Standardized column names and launch outcomes  
   - Removed duplicate or incomplete entries

3. **Exploratory Data Analysis**  
   - Payload mass vs. success rate  
   - Launch site-wise performance  
   - Booster version impact  
   - Orbit type vs. landing success

4. **Interactive Visualization with Plotly & Dash**  
   - Dropdowns, sliders, scatter plots, pie charts  
   - Real-time filtering based on site/payload

5. **Machine Learning Prediction**  
   - Classification models: Logistic Regression, Decision Trees, SVM, KNN  
   - Feature engineering (one-hot encoding, scaling)  
   - Hyperparameter tuning  
   - Model evaluation with accuracy, F1-score
