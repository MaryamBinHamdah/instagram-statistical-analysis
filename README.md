# 📊 Instagram Influencers Statistical Analysis

This repository contains a comprehensive statistical data analysis project focused on the follower counts of top Instagram influencers across three continents: Asia, America, and Europe. This project was completed collaboratively as part of the "Statistical Inference (CIS 2003)" course.

## 🎯 Research Question & Objective

The core objective of this project was to apply statistical inference techniques to analyze the dataset and answer the following research question:
> **"Is the average number of followers for accounts in this dataset equal to 5 million?"**

We utilized the mean of the subscribers (per 1000 influencers) as our primary measure of central location to conduct our analysis and draw data-driven conclusions.

## 🛠️ Technologies & Tools Used
*   **Language:** Python
*   **Libraries:** `Pandas`, `NumPy`, `SciPy` (for statistical tests), `Matplotlib` / `Seaborn` (for data visualization).
*   **Documentation:** MS Word / PDF for the final statistical report.

---

## 📈 Statistical Analysis & Key Findings

The project was structured into four main analytical phases:

### Phase 1: Descriptive Statistics & Visualizations
We used Python to describe the data graphically and extract initial insights:

**1. Boxplot Analysis**
*   **Europe:** Median of 26.5 (Positively/Right-skewed).
*   **Asia:** Median of 9.1 (Positively skewed).
*   **America:** Median of 12.6 (Slightly skewed to the right with a longer tail).

![Boxplot of Followers by Continent](https://github.com/user-attachments/assets/e1fd47c5-4dc5-4361-abfc-59b153ec6bf3 )


**2. Histogram Analysis**
The overall distribution is right-skewed, meaning the majority of accounts have a lower number of followers, while a very small percentage have significantly high numbers. Europe has the most accounts with lower followers, America has the most with high followers, and Asia is relatively balanced.

![Histogram of Followers Distribution](https://github.com/user-attachments/assets/a4c67f49-b02e-4862-a2be-02c6134f9dbf )


### Phase 2: Normality Check & Outliers
*   **Five-Number Summary:** Minimum (2.8), Q1 (9), Median (14.4), Q3 (25.65), and Maximum (469.6).
*   **Outliers:** We identified 84 upper outliers (values > 50.625). Since the data represents human followers, there are no lower outliers (negative values).
*   **Skewness:** The calculated Pearson’s coefficient of skewness is **0.81**. This confirms a strong positive correlation and a positively skewed distribution, heavily influenced by the upper outliers.

### Phase 3: Estimation of Population Mean
*   **Point Estimate:** The sample mean ($\bar{x}$) was calculated as **29.46 million** followers (Sample size n=30, Standard Deviation = 71.27).
*   **Confidence Intervals:** We manually constructed confidence intervals to estimate the true population mean ($\mu$):
    *   **90% CI:** (7.99, 50.93) - Width: 42.94
    *   **95% CI:** (3.96, 54.96) - Width: 51.00
    *   **99% CI:** (-4.11, 63.03) - Width: 67.14
*   **Insight:** As the confidence level increases, the width of the confidence interval also increases, demonstrating that a wider interval is required to be more certain that it contains the true population mean.

### Phase 4: Hypothesis Testing
To verify our initial research question, we conducted a formal hypothesis test:
*   **Hypothesis:** Testing if the true average number of followers is 5 million ($\mu = 5$).
*   **Test Parameters:** Two-tailed Z-test, Significance Level ($\alpha$) = 10%, Sample Size (n) = 30.
*   **Calculations:** The calculated Z-score was **-1.88**, while the critical Z-value for a 90% confidence level is **±1.65**.
*   **Conclusion:** Since the calculated Z-score (-1.88) falls within the rejection region (beyond the critical value of -1.65), we **rejected the null hypothesis**. This statistically proves that the true average number of followers is significantly different from the hypothesized 5 million.

**3. Hypothesis Testing (Normal Curve)**
![Normal Curve for Hypothesis Testing](https://github.com/user-attachments/assets/83716e68-4aa3-41a6-a571-59458de30945 )

---

## 💡 Role & Contributions

As a core member of this collaborative project, my responsibilities included:
*   **Python Programming:** Collaborating on writing the Python scripts required to compute descriptive statistics, generate visualizations, and perform hypothesis testing.
*   **Statistical Interpretation:** Analyzing the outputs (such as Pearson's coefficient, confidence intervals, and Z-scores) to draw logical conclusions.
*   **Report Documentation:** Contributing to the comprehensive report, ensuring all statistical findings were accurately documented.
*   **Oral Defense:** Successfully presenting and defending our statistical methodology and findings during the individual viva assessment.

---

## 📄 Project Documentation & Code

For a detailed explanation of the statistical tests, manual calculations, and final conclusions, please refer to the full project report:
* [View Statistical Analysis Report (PDF)](instagram-statistical-analysis.docx/instagram-statistical-analysis.pdf)
