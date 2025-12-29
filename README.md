# Google Play Store Analytics

<div align="center">

<img src="google.avif" alt="drawing" width="500"/>

</div>

## Overview
Comprehensive analysis of 10,841 Google Play Store apps exploring ratings, reviews, installs, categories, and pricing strategies. Delivered actionable insights for app developers and marketers to optimize app performance and user engagement.

## Dataset Overview
- **Size**: 10,841 unique apps spanning 34 categories with 13 features including app metadata, performance metrics, and user engagement data.
- **Key Metrics**: Average rating of 4.19, predominantly free apps (92.6%), most popular category is FAMILY (1,972 apps), followed by GAME and TOOLS.
- **Features**: App name, category, rating (1-5 scale), reviews count, size (MB), installs range, type (Free/Paid), price, content rating, genres, last updated date, current version, and minimum Android version.
- **Install Distribution**: Ranges from 0-100 downloads to 1 billion+ installs, with 1 million+ being the most common install bracket (1,579 apps).
- **Pricing**: 10,040 free apps, 801 paid apps with prices ranging from $0.99 to $400, most paid apps under $5.
- **Content Ratings**: Majority rated "Everyone" (8,714 apps), followed by Teen (1,146), Mature 17+ (447), and Everyone 10+ (376).
- **Data Quality**: Contains missing values in ratings (1,474 nulls), some size and version fields marked as "Varies with device" requiring cleanup.

## Analysis
- **Exploratory Data Analysis (EDA)**:  
  - Cleaned data by handling missing ratings, converting size from text to numeric MB values, extracting minimum Android version numbers, and transforming install ranges into average install counts.
  - Analyzed category distribution finding GAME apps are largest in size (avg 40.8 MB) while TOOLS apps are smallest (9.3 MB), reflecting different functionality needs.
  - Discovered free apps average 437K reviews versus paid apps with only 11.9K reviews, indicating massive engagement gap.

- **Visualizations**:  
  - Created bar charts showing category-wise ratings, with EDUCATION (4.37) and ART_AND_DESIGN (4.37) leading, while DATING (4.01) and MAPS_AND_NAVIGATION (4.06) lag behind.
  - Built install range analysis revealing higher install brackets correlate with better ratings, peaking at 4.37 for 50M-1B install apps.
  - Visualized top reviewed apps including Facebook (78M reviews), WhatsApp (69M reviews), and Instagram (66M reviews), all with 1 billion+ installs.

- **Category Performance**:  
  - GAME category dominates total installs with 31.5 billion, followed by COMMUNICATION (24.1B) and SOCIAL (12.5B), showing entertainment and connectivity drive adoption.
  - Content rating analysis shows "Everyone" apps dominate both free (80.5%) and paid (86.5%) segments, indicating family-friendly content performs best commercially.
  - Identified pricing sweet spots with most successful paid apps priced between $0.99-$4.99, balancing affordability and perceived value.

- **Insights for Developers**:  
  - Apps with perfect 5.0 ratings but minimal reviews (under 100) suggest niche success or limited exposure, highlighting growth opportunities.
  - Regular updates correlate with higher ratings, with most top-rated apps updated in 2018, demonstrating importance of active maintenance.
  - Free apps with in-app purchases generate significantly more engagement than paid apps, validating freemium business models in the Play Store ecosystem.

## How to Use
- Clone the repository:
  ```git
  git clone https://github.com/PratyushPuri/Google-Play-Store-Analytics.git
  ```
- Install required dependencies:
  ```python
  pip install -r requirements.txt
  ```
- Typical libraries include pandas, numpy, seaborn, matplotlib for analysis and visualization.
- Open `google-play-store-analytics.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
- Run cells from top to bottom to load data, perform cleaning, generate visualizations, and extract insights.
- Original Kaggle notebook:  
[google-play-store-analytics](https://www.kaggle.com/code/pratyushpuri/google-play-store-analytics)
- Customize the analysis:  
- Filter by specific categories or content ratings to focus on target markets.
- Add sentiment analysis on review text data if available to understand user satisfaction drivers.
- Compare app performance over time by analyzing update frequency versus rating trends.
- Create predictive models to estimate potential installs based on category, size, and pricing strategy.
- Use insights to inform app development decisions around category selection, pricing models, size optimization, and update schedules.

## Author & Contact
- Name: `Pratyush Puri`  
- Contact: `pratyushpuri17@gmail.com`  
- LinkedIn: [https://www.linkedin.com/in/pratyushpuri](https://www.linkedin.com/in/pratyushpuri)

