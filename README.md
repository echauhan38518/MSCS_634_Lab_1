# MSCS_634_Lab_1 – Data Visualization, Preprocessing, and Statistical Analysis

## Purpose of the Lab

The purpose of this lab is to apply the fundamental data analysis techniques using Python and Jupyter Notebook. The lab focuses on exploring a real-world dataset, performing data visualization, cleaning and preprocessing data, and applying basic statistical analysis methods. Through this process, the lab demonstrates how raw, imperfect data can be transformed into a structured and meaningful form suitable for analysis and interpretation.

The dataset used for this lab is the **dirty_cafe_sales.csv** dataset obtained from Kaggle, which contains transactional sales data from a café, including items sold, quantities, prices, payment methods, and total spending.

---

## Key Insights from Visualizations and Statistical Analysis

### Data Visualization Insights
- Bar charts revealed that certain menu items are purchased more frequently than others, indicating clear customer preferences.
- Scatter plots showed a positive relationship between **Quantity** and **Total Spent**, confirming that higher quantities generally lead to increased spending.
- Histograms demonstrated that most transactions fall within a lower spending range, with fewer high-value purchases.
- Pie charts illustrated the distribution of payment methods and showed that some payment options are more commonly used than others.

### Statistical Analysis Insights
- Descriptive statistics (`.describe()`) showed that the dataset has noticeable variability in **Quantity** and **Total Spent**, indicating a mix of small and large transactions.
- Measures of central tendency (mean, median, and mode) provided insight into typical customer spending behavior.
- Dispersion measures such as standard deviation and interquartile range (IQR) highlighted the presence of outliers, particularly in the **Total Spent** column.
- Correlation analysis indicated a strong positive correlation between **Quantity** and **Total Spent**, while **Price Per Unit** showed a weaker relationship with quantity purchased.

---

## Challenges Faced and Decisions Made

One of the main challenges encountered during the lab was handling missing and inconsistent data. Several columns contained missing values, which required careful selection of appropriate imputation methods. Numeric columns were handled using forward fill, backward fill, and mean replacement, while categorical columns were filled with placeholder values such as `"Unknown"`.

Another challenge involved managing outliers in transaction data. The Interquartile Range (IQR) method was chosen to identify and remove extreme values in order to prevent skewing the statistical analysis.

Decisions were also made regarding data reduction and transformation. Less relevant columns were removed to simplify analysis, and sampling was applied to reduce dataset size for efficiency. Additionally, scaling and discretization techniques were used to standardize numeric values and convert continuous data into meaningful categories, improving interpretability.

Overall, these preprocessing decisions ensured that the dataset was clean, consistent, and suitable for visualization and statistical analysis.
