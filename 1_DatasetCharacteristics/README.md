# Dataset Characteristics

**[Notebook](exploratory_data_analysis.ipynb)**

## Dataset Information

### Dataset Source
- **Dataset Link:** [https://github.com/mofreund99/TeamCPH/blob/cf92ab3dd288d89a6d61c81a1105a22519ccda0e/model_df.csv]
- **Dataset Owner/Contact:** [If applicable, provide contact information for private datasets]

### Dataset Characteristics
- **Number of Observations:** [9292 samples ]
- **Number of Features:** [ 18 features ]

### Target Variable/Label
- **Label Name:** [Umsatz]
- **Label Type:** [Regression]
- **Label Description:** [Umsatz represents the daily revenue (sales value) for a given product category (Warengruppe). The prediction task is to forecast daily revenue based on temporal, seasonal, event-based, and lagged revenue features.]
- **Label Values:** [countinous variable, range: 7.05 - 1879.46, mean: 206.65, standard deviation: 144.36]
- **Label Distribution:** [The distribution is right-skewed, with most revenues concentrated below 300 and some high-value outliers reaching up to ~1879. This suggests occasional peak sales days]

### Feature Description
[The dataset contains 18 columns and 9,292 observations. All features are numeric]

1. Revenue-Based Features
   
Feature 1 (Revenue_lag1): Description: Revenue from the previous day (t-1), Range: 7.05 – 1879.46, Purpose: Captures short-term temporal dependency (autocorrelation).

Feature 2 (Revenue_lag7): Description: Revenue from 7 days prior (t-7), Range: 7.05 – 1879.46, Purpose: Captures weekly seasonality patterns.

2. Product Category Features
   
Feature 3 (Warengruppe), 
Range: 1 – 6, 
Description: Categorical identifier for product group. Feature Group (WG_2, WG_3, WG_4, WG_5, WG_6), One-hot encoded product categories, WG_2 = 1 → observation belongs to product group 2 etc. Warengruppe = 1 serves as the reference category.

3. Calendar & Event Features
Feature 4 (holiday): 
Description: Indicates whether the day is a public holiday.

Feature 5 (IsWeekend):
Description: 1 if Saturday/Sunday, otherwise 0.

Feature 6 (IsNewYears):
Description: 1 if the date is New Year’s Day.

Feature 7 (Easter):
Description: 1 if the day is during Easter period.

Feature 8 (KielerWoche):
Description: 1 if the day falls within Kieler Woche (regional event), capturing local event-driven demand spikes.

4. Seasonal (Cyclical) Features

These features encode annual seasonality using sine/cosine transformations to preserve cyclical structure.

Feature 9 (sin_1y):
Range: -1 to 1
Description: First harmonic sine transformation of yearly cycle.

Feature 10 (cos_1y)
Range: -1 to 1
Description: First harmonic cosine transformation of yearly cycle.

Feature 11 (sin_2y)
Range: -1 to 1
Description: Second harmonic sine term (captures more complex seasonal patterns).

5. Transformed Target Feature
Feature 12 (log_Umsatz)
Description: Natural logarithm of revenue.


## Exploratory Data Analysis

The exploratory data analysis is conducted in the [exploratory_data_analysis.ipynb](exploratory_data_analysis.ipynb) notebook, which includes:

- Data loading and initial inspection
- Statistical summaries and distributions
- Missing value analysis
- Feature correlation analysis
- Data visualization and insights
- Data quality assessment
