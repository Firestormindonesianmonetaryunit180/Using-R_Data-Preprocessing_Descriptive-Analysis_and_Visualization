# 🍔 Fast Food Nutrition: Statistical Data Analysis & Preprocessing in R

[![R](https://img.shields.io/badge/R-276DC3?style=flat&logo=r&logoColor=white)](https://www.r-project.org/)
[![dplyr](https://img.shields.io/badge/dplyr-Data_Manipulation-blue?style=flat)](#)
[![ggplot2](https://img.shields.io/badge/ggplot2-Data_Visualization-green?style=flat)](#)
[![corrplot](https://img.shields.io/badge/corrplot-Correlation_Matrix-orange?style=flat)](#)

## 📖 Project Overview
This repository contains a comprehensive statistical analysis of the nutritional content of fast food. Using **R**, we explored a dataset of 515 menu items from various popular fast-food chains, evaluating 17 distinct variables, ranging from macronutrients (calories, fats, proteins) to micronutrients (vitamins, calcium). 

The core objective of this project is to apply rigorous data preprocessing, descriptive statistics, and Exploratory Data Analysis (EDA) to uncover the underlying nutritional patterns and distributions within the fast-food industry.

**Data Source:** [OpenIntro - Fast Food Nutrition](https://www.openintro.org/data/index.php?data=fastfood)

## ⚙️ Data Preprocessing & Cleaning Strategy
Real-world data is rarely perfect. A significant portion of this project focused on handling missing values (NAs) while preserving statistical integrity:

1. **Complete Case Analysis (`na.omit`):** Initially, dropping all rows with missing numeric values resulted in a 41.5% data loss (from 515 to 301 observations). While this ensures a complete matrix, it risks reducing the statistical power of the dataset.
2. **Mean Imputation:** To retain all 515 observations, we replaced missing numeric values (primarily in Vitamin A, Vitamin C, and Calcium) with the column mean. *Note: As observed in our diagnostics, this creates artificial clustering around the mean and compresses the interquartile range.*
3. **Categorical Mode Imputation:** Categorical variables (`restaurant`, `item`, `salad`) were evaluated for missingness and were confirmed to be 100% complete, requiring no mode imputation.

## 📊 Exploratory Data Analysis (EDA)

The analysis was structured into three distinct statistical tiers:

### 1. Univariate Analysis (Distributions & Outliers)
Using the Interquartile Range (IQR) method and visualizations (Histograms & Boxplots), we evaluated single-variable distributions:
* **Right-Skewed Distributions:** Nearly all nutritional attributes exhibit a heavy right-skew. The mean is consistently higher than the median.
* **The Outlier Reality:** There are **zero** low-end outliers. Instead, the dataset is packed with upper-end outliers (e.g., 70 high-end outliers for Vitamin C, 46 for Fiber). This proves that while standard fast-food items cluster around a baseline, there are numerous "extreme" menu items that drastically pull the averages upward.

### 2. Bivariate Analysis (Relationships)
We mapped the interactions between two variables to understand how they scale together:
* **Calories vs. Protein (Scatterplot + Regression):** Demonstrated a clear, positive linear relationship, as calories increase, protein generally increases alongside it.
* **Sodium by Restaurant (Density Plot):** Highlighted the distinct sodium profiles across chains, showing that while all are right-skewed, certain restaurants have much wider spreads of high-sodium items.
* **Calories by Restaurant (Boxplot/Bar Chart):** Revealed significant variations in the median and mean caloric offerings depending on the specific fast-food chain chosen.

### 3. Multivariate Analysis (Correlation Matrix)
We utilized a Correlation Heatmap (`corrplot`) to evaluate the entire numeric matrix simultaneously:
* **The Macronutrient Block:** There are incredibly strong positive correlations (r > 0.70) between Calories, Total Fat, Sodium, and Protein. If an item is high in one, it is almost certainly high in the others.
* **The Independent Micronutrients:** Vitamin A, Vitamin C, and Calcium showed near-zero (and sometimes slightly negative) correlations with the heavy macronutrients, indicating that a high-calorie/high-fat meal does not inherently scale with higher vitamin or mineral content.

## 🎯 Advanced Data Slicing (`dplyr::filter`)
To demonstrate targeted data retrieval, the `dplyr` package was used to chain quantitative and qualitative filters. For example, we successfully isolated highly specific niches, such as:
* **High-Energy Items:** Extracting all items strictly exceeding 800 calories.
* **Targeted Dietary Needs:** Combining qualitative and quantitative constraints to find specifically "Burger King" items with strictly under 1000 mg of sodium.

## 🛠️ Technology Stack
* **Language:** R
* **Data Manipulation:** `dplyr`, `tidyr`
* **Data Visualization:** Base R Graphics, `ggplot2`, `ggpubr`, `corrplot`
* **Statistical Methods:** IQR Outlier Detection, Mean/Mode Imputation, Linear Regression (`lm`), Pearson Correlation

## 💻 How to Run Locally

1. Clone the repository to your local machine.
2. Ensure you have R and RStudio installed.
3. Install the required libraries:
   ```R
   install.packages(c("ggplot2", "dplyr", "tidyr", "ggpubr", "corrplot"))
