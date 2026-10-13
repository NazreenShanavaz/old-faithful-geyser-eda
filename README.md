# Old Faithful Geyser — Exploratory Data Analysis

## Project Overview

This project explores the Old Faithful geyser dataset using Python to understand patterns in eruption duration and waiting time. Through exploratory data analysis (EDA), I investigated distributions, relationships between numerical variables, differences between eruption types, and potential outliers.


## Objectives

- Explore and understand the dataset.
- Analyze the distributions of eruption duration and waiting time.
- Investigate the relationship between eruption duration and waiting time.
- Compare short and long eruptions.
- Identify potential outliers using the IQR method.
- Communicate findings through visualizations and summary statistics.

## Dataset Description

The dataset contains **272 observations and 3 columns**.

| Column | Description |
|---|---|
| `duration` | Duration of the geyser eruption, in minutes |
| `waiting` | Waiting time until the next eruption, in minutes |
| `kind` | Eruption type: short or long |

The dataset was loaded using Seaborn's built-in `geyser` dataset. No missing values were found during the initial data inspection.

## Tools and Libraries

- Python
- Pandas
- Matplotlib
- Seaborn
- Google Colab
- GitHub

## Analysis Performed

1. **Data inspection:** Examined the dataset's structure, column names, data types, and missing values.
2. **Descriptive statistics:** Analyzed the mean, median, standard deviation, minimum, maximum, and quartiles.
3. **Distribution analysis:** Created histograms to explore eruption duration and waiting time.
4. **Relationship analysis:** Used scatter plots and Pearson correlation to investigate the association between duration and waiting time.
5. **Group comparison:** Compared average waiting times for short and long eruptions.
6. **Outlier investigation:** Used box plots and the Interquartile Range (IQR) method to identify potential outliers.
7. **Correlation analysis:** Compared the overall correlation with correlations calculated separately for each eruption type and visualized the overall correlation matrix using a heatmap.

## Key Findings

- Eruption duration and waiting time showed two distinct clusters in their distributions.
- Duration and waiting time had a strong positive overall correlation of approximately **0.90**.
- Long eruptions had a mean waiting time of approximately **80.28 minutes**, compared with **54.75 minutes** for short eruptions.
- The within-group correlations were weaker than the overall correlation: approximately **0.32 for long eruptions** and **0.43 for short eruptions**.
- The IQR method flagged a waiting time of **96 minutes** in the long-eruption group as a potential outlier.

## 💡 Conclusion

This analysis revealed distinct patterns in Old Faithful geyser eruptions and a strong overall association between eruption duration and waiting time. Comparing eruption types showed that group-level patterns can differ from the overall relationship. The project also provided practice in using visualizations, descriptive statistics, correlation, and outlier detection to explore real-world data.

**Note:** Correlation indicates association, not causation. Potential outliers were identified statistically and were not automatically removed.

## Project Structure

```text
old-faithful-geyser-eda/
├── Old_Faithful_Geyser_EDA.ipynb
└── README.md
```

## How to Run

1. Open the notebook in Google Colab.
2. Run the cells from top to bottom.
3. Explore the visualizations and analysis outputs.

The dataset is loaded directly through Seaborn, so a separate dataset download is not required.

## Learning Outcomes


- Data inspection and descriptive statistics
- Data visualization with Matplotlib and Seaborn
- Grouping and aggregation using Pandas
- Correlation analysis
- IQR-based outlier detection
- Interpreting and communicating analytical findings



