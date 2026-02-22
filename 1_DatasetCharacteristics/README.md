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
[Provide a brief description of each feature or group of features in your dataset. If you have many features, group them logically and describe each group. Include information about data types, ranges, and what each feature represents.]

**Example format:**
- **Feature 1 (feature_name):** [Description of what this feature represents, data type, and any relevant details]
- **Feature 2 (feature_name):** [Description of what this feature represents, data type, and any relevant details]
- **Feature Group (group_name):** [Description of a group of related features]

## Exploratory Data Analysis

The exploratory data analysis is conducted in the [exploratory_data_analysis.ipynb](exploratory_data_analysis.ipynb) notebook, which includes:

- Data loading and initial inspection
- Statistical summaries and distributions
- Missing value analysis
- Feature correlation analysis
- Data visualization and insights
- Data quality assessment
