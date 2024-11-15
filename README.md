
This project explores the relationship between geographic location, business type, and socioeconomic status to predict minority ownership among women-owned businesses in Greater Boston. The analysis pipeline involves:

Data Collection and Preprocessing:

Data on women-owned businesses was sourced from Boston city government datasets.
Geospatial and socioeconomic data were integrated by geocoding business addresses and performing spatial joins with census tracts.
Feature Engineering:

Business types were recategorized into nine categories (e.g., retail, healthcare) and encoded as binary dummy variables.
Geospatial features like distance and bearing from downtown Boston were computed to analyze spatial patterns.
Exploratory Data Analysis (EDA):

Visualizations highlighted disparities in income and location between minority and non-minority women-owned businesses.
Principal Component Analysis (PCA) reduced dimensionality, emphasizing the importance of location and median income.
Predictive Modeling:

k-Nearest Neighbors (kNN): Used normalized geographic and income data, achieving a maximum accuracy of 71.1%.
Random Forest: Assessed feature importance, showing median income and geographic distance as key predictors.
Logistic Regression: Identified statistically significant predictors using forward stepwise selection.
Visualization and Mapping:

Interactive maps created using tmap visualized business distribution and socioeconomic factors.
Correlation matrices and bar charts provided deeper insights into variable relationships and model results.
Findings:

Minority-owned women’s businesses are more likely to be located in areas with lower median income and further from downtown Boston.
Business type contributed minimally to prediction accuracy, highlighting the dominant role of socioeconomic and geographic factors.
This pipeline demonstrates the use of R for integrating geospatial, socioeconomic, and business data with predictive analytics, supporting policymakers in targeting resources to empower minority-owned women’s businesses in disadvantaged areas.
