# **Geospatial and Socioeconomic Analysis of Minority Ownership Among Women-Owned Businesses in Greater Boston**

This project explores the relationship between geographic location, business type, and socioeconomic status to predict minority ownership among women-owned businesses in Greater Boston. By integrating geospatial, socioeconomic, and business data, the project provides actionable insights for policymakers to support minority-owned women’s businesses in disadvantaged areas.

---

## **Overview**
This analysis pipeline involves:
- **Data Collection and Preprocessing**: Integrating geospatial and socioeconomic data with business data.
- **Feature Engineering**: Creating meaningful variables like business categories and spatial features.
- **Exploratory Data Analysis (EDA)**: Identifying disparities using visualizations and dimensionality reduction techniques.
- **Predictive Modeling**: Building models to predict minority ownership using socioeconomic and geographic features.
- **Visualization and Mapping**: Creating interactive maps and insightful visualizations.

---

## **Pipeline Components**

### **1. Data Collection and Preprocessing**
- Data on women-owned businesses was sourced from Boston city government datasets.
- Geospatial and socioeconomic data were integrated by:
  - **Geocoding**: Converting business addresses into geographic coordinates.
  - **Spatial Joins**: Mapping business locations to census tracts to link socioeconomic data.

---

### **2. Feature Engineering**
- Business types were recategorized into nine categories (e.g., retail, healthcare) and encoded as binary dummy variables.
- Geospatial features like:
  - **Distance** from downtown Boston.
  - **Bearing (direction)** relative to downtown.
- These features were computed to identify spatial patterns.

---

### **3. Exploratory Data Analysis (EDA)**
- Visualizations highlighted:
  - **Income disparities** between minority-owned and non-minority-owned women’s businesses.
  - **Location differences**, emphasizing the geographic spread.
- **Principal Component Analysis (PCA)**:
  - Reduced dimensionality.
  - Highlighted the significance of location and median income as key factors.

---

### **4. Predictive Modeling**
#### **k-Nearest Neighbors (kNN)**:
- Used normalized geographic and income data.
- Achieved a maximum accuracy of **71.1%**.

#### **Random Forest**:
- Analyzed feature importance.
- Identified **median income** and **distance from downtown** as the most critical predictors.

#### **Logistic Regression**:
- Applied forward stepwise selection.
- Highlighted statistically significant predictors.

---

### **5. Visualization and Mapping**
- **Interactive Maps**:
  - Created using the `tmap` R package.
  - Visualized business distribution and socioeconomic factors.
- **Correlation Matrices** and **Bar Charts**:
  - Showed relationships between variables.
  - Provided insights into model performance and key findings.

---

## **Findings**
- **Location and Income**:
  - Minority-owned women’s businesses are more likely to be located in areas with **lower median income** and **further from downtown Boston**.
- **Business Type**:
  - Contributed minimally to prediction accuracy.
  - Socioeconomic and geographic factors were dominant predictors.

---

## **Tools & Technologies**
- **Programming Language**: R
- **Packages Used**:
  - `tmap`, `spatial`, `caret`, `ggplot2`, `sf`, `dplyr`, `tidyverse`
- **Data Sources**:
  - Boston city government datasets.
  - U.S. Census Bureau.

---

## **Conclusion**
This pipeline demonstrates the effective integration of geospatial, socioeconomic, and business data with predictive analytics. It provides valuable insights to policymakers aiming to empower minority-owned women’s businesses in disadvantaged areas.

---

## **Future Work**
- Include additional variables like industry-specific factors or funding availability.
- Explore temporal trends to analyze how these patterns evolve over time.
- Enhance accuracy by testing ensemble models or deep learning approaches.

---

## **Contributors**
- **[Your Name]**
- [Additional contributors, if applicable]

---

Feel free to adapt this structure or let me know if you'd like additional sections or modifications!
