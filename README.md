# Breast-Cancer-Data-Analysis
Performed an in-depth analysis of a breast cancer dataset to explore correlations between tumor characteristics and cancer diagnoses. Conducted data cleaning and visualization using Tableau to uncover patterns and insights, enhancing understanding of key predictors for breast cancer detection and diagnosis.
Today, I’ll be presenting an analysis of a breast cancer dataset, discussing its structure, cleaning process, key questions, and insights derived from visualizations. The primary aim is to understand how tumor characteristics correlate with diagnoses and explore patterns in the data that can improve our understanding of breast cancer.

The dataset contains 570 rows, each representing a patient’s tumor record, and 32 columns, which are features extracted from tumor analysis. These features include measurements like radius, texture, perimeter, and smoothness, categorized into mean, standard error, and worst-case values.

Let’s walk through the steps of preparing this data for analysis, asking the right questions, and using visualization tools like Tableau to derive actionable insights.
First, let’s discuss the structure of the dataset.

The diagnosis column indicates whether a tumor is benign or malignant, serving as the target variable for classification.
The other 31 columns represent tumor features, which can be grouped as:
Mean features: Average values, like radius_mean and texture_mean.
Standard error features: Variability in these values, such as radius_se.
Worst-case features: The largest observed values, like radius_worst.
The dataset allows us to investigate patterns that differentiate benign from malignant tumors based on these features.

Before jumping into analysis, we needed to ensure the data was clean and reliable.

Data Cleaning Process 
To clean the dataset, we used Excel filters to:

Identify and remove missing values: Any rows with missing data in critical columns like diagnosis or radius_mean were filtered out.
Ensure numeric validity: We verified that numeric columns, such as area_mean or compactness_worst, contained valid numerical data.
Remove duplicates: Using Excel’s “Remove Duplicates” feature, we ensured that each record was unique.
After cleaning, we retained all 32 columns and 570 rows, ensuring the dataset was ready for exploratory analysis. This step is crucial, as incomplete or incorrect data could lead to misleading results.

Key Questions and Visualizations
Next, we formulated several key questions to extract meaningful insights from the data. For each question, we created a visualization using Tableau to interpret the results. Let’s go through these questions one by one:

1. What is the proportion of benign vs. malignant tumors?
Using a pie chart, we visualized the diagnosis column. This revealed that the majority of tumors in the dataset are benign, but a significant portion is malignant. This distribution provides a starting point for understanding the dataset’s balance and helps frame subsequent questions.

2. Do tumors with a higher texture mean tend to be malignant?
Texture can indicate irregularities in the tumor. By plotting texture_mean against diagnosis using a scatter plot, we observed that malignant tumors often have higher texture values. This supports the hypothesis that irregular textures are more associated with malignancy.

3. Is the tumor's mean smoothness different between benign and malignant tumors?
To investigate this, we used a box plot comparing smoothness_mean values for benign and malignant tumors. Malignant tumors displayed a wider range of smoothness, indicating more irregular surfaces compared to benign tumors, which tend to have smoother edges.

4. What is the average tumor size for benign vs. malignant cases?
Tumor size was examined using radius_mean. A bar chart showed that the average radius of malignant tumors is significantly larger than that of benign tumors, reinforcing the idea that size can be a key diagnostic factor.

5. Which features are most correlated with malignancy?
A heatmap of correlation coefficients revealed that features like concavity_mean, radius_worst, and area_worst are strongly correlated with malignancy. These features may serve as critical indicators in predictive modeling.

6. Which features are most correlated with benign tumors?
Similarly, features like smoothness_mean and symmetry_mean showed a negative correlation with malignancy, making them strong indicators of benign cases.

7. What is the distribution of tumor perimeter and area?
Using a scatter plot, we examined perimeter_mean against area_mean. This revealed clear clustering patterns, with malignant tumors occupying a distinct range compared to benign ones.

8. How do tumor shape features like smoothness, compactness, and concavity differ between benign and malignant cases?
A stacked bar chart for these features highlighted that malignant tumors generally exhibit higher compactness and concavity, whereas benign tumors tend to have higher smoothness.

9. How do “worst-case” measurements vary between benign and malignant tumors?
We used side-by-side bar charts for radius_worst, texture_worst, and perimeter_worst. Malignant tumors consistently showed higher worst-case values, indicating their irregular and invasive nature.

10–13. Comparisons Between Mean and Worst-Case Values
For features like radius, area, perimeter, and texture, we plotted dual-axis line charts comparing their mean and worst-case values. This analysis highlighted that malignant tumors tend to have greater disparities between mean and worst-case measurements, reflecting their variability and aggressiveness.

14. Do malignant tumors have a larger mean radius than benign tumors?
Finally, a bar chart comparing radius_mean across diagnoses confirmed that malignant tumors have significantly larger radii on average. This aligns with clinical observations of tumor growth patterns.

Conclusion and Next Steps 
Through these visualizations, we extracted valuable insights:

Malignant tumors tend to be larger, less smooth, and more irregular in shape.
Key features like radius_worst, concavity_mean, and texture_mean are strongly correlated with malignancy.
While we’ve answered many important questions, the dataset offers even more potential for exploration. Future steps could include:

Applying machine learning models for predictive analysis.
Conducting clustering to group similar tumor types.
Exploring relationships between multiple features simultaneously.
By continuing this analysis, we can deepen our understanding of tumor characteristics and enhance diagnostic tools for breast cancer.

Thank you for your attention, and I’m happy to answer any questions you may have!

