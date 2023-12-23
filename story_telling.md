# Sleep-Health-and-Lifestyle
This synthetic dataset contains sleep and cardiovascular metrics as well as lifestyle factors of close to 400 fictive persons.

The workspace is set up with one CSV file, `data.csv`, with the following columns:

- `Person ID`
- `Gender`
- `Age`
- `Occupation`
- `Sleep Duration`: Average number of hours of sleep per day
- `Quality of Sleep`: A subjective rating on a 1-10 scale
- `Physical Activity Level`: Average number of minutes the person engages in physical activity daily
- `Stress Level`: A subjective rating on a 1-10 scale
- `BMI Category`
- `Blood Pressure`: Indicated as systolic pressure over diastolic pressure
- `Heart Rate`: In beats per minute
- `Daily Steps`
- `Sleep Disorder`: One of `None`, `Insomnia` or `Sleep Apnea`

Check out the guiding questions or the scenario described below to get started with this dataset!
Feel free to make this workspace yours by adding and removing cells, or editing any of the existing cells.

Source: [Kaggle](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset/)

### 🔍 **Scenario: Automatically identify potential sleep disorders**

This scenario helps you develop an end-to-end project for your portfolio.

Background: You work for a health insurance company and are tasked to identify whether or not a potential client is likely to have a sleep disorder. The company wants to use this information to determine the premium they want the client to pay.

**Objective**: Construct a classifier to predict the presence of a sleep disorder based on the other columns in the dataset.
## **EDA**
### Exploring the Relationship Between Occupation and Sleep Patterns: A Comparative Analysis of Sleep Duration and Quality
The following visualizations serve as a foundation for understanding the complex relationship between occupation and sleep health. They highlight potential areas of concern where occupational demands might negatively impact sleep, and conversely, where certain job types might correlate with better sleep health. This analysis is crucial for developing targeted interventions or recommendations for improving sleep health in specific professional groups.

**1. Sleep Duration by Occupation:**
- Range and Median: Different occupations show varied ranges in sleep duration. For instance, if certain occupations like 'Software Engineers' or 'Doctors' have a wider range, it might indicate a more inconsistent sleep pattern within these professions. The median line within each box indicates the typical sleep duration for each occupation, which can be compared across different jobs.
- Outliers: If there are occupations with notable outliers (points that lie outside the typical range of the boxplot), this could suggest that individuals in these professions experience either significantly more or less sleep than their peers, possibly due to job-related stress or irregular work hours.
- Tight vs. Wide Distributions: Some occupations might have tighter distributions (smaller boxes), suggesting more uniformity in sleep duration among individuals in these jobs. Others with wider distributions indicate more variability among workers in that field.
**2. Quality of Sleep by Occupation:**
- Highs and Lows: Pay attention to occupations that have higher median sleep quality scores versus those with lower scores. This can suggest which professions are associated with better perceived sleep quality.
- Consistency: Occupations with boxes that have less spread (narrower boxes) indicate a more consistent sleep quality experience among individuals in that profession, whereas wider boxes show greater variance.
- Skewness: The skewness in the distribution (whether the box and whiskers are symmetric or skewed to one side) can indicate a tendency towards higher or lower sleep quality ratings in certain occupations.

### Analyzing the Intersection of Age, Sleep Duration, and Sleep Disorders: A Visual Exploration
The scatterplot visualizes the relationship between sleep duration, age, and the presence of sleep disorders, offering several valuable insights:

**1. Age and Sleep Duration Correlation:** The plot provides a visual representation of how sleep duration varies with age. Look for any trends such as increasing or decreasing sleep duration as age increases. If a trend is visible, it suggests a potential age-related change in sleep patterns.
**2. Impact of Sleep Disorders:** The use of different colors to represent different sleep disorders (None, Insomnia, Sleep Apnea) allows us to observe how these conditions are distributed across different age groups and how they might affect sleep duration. Key insights could include:
- Whether certain sleep disorders are more prevalent in specific age groups.
- How sleep duration varies among individuals with different sleep disorders. For instance, do those with insomnia tend to have shorter sleep durations?
**3. Cluster and Spread:** The distribution and clustering of points can indicate common patterns. A dense clustering of points in a certain area suggests a common sleep duration for a specific age group, while a more spread-out distribution indicates variability.
**4. Outliers and Anomalies:** Any points that lie far from the general cluster can indicate unusual cases, such as very young or old individuals with atypical sleep durations or specific sleep disorder patterns not common in their age group.

This scatterplot effectively combines three critical dimensions of the dataset—age, sleep duration, and sleep disorders—to provide a comprehensive view of how these factors interrelate. Such insights are invaluable for understanding the dynamics of sleep health across different age groups and for identifying specific age groups that might be more susceptible to certain sleep disorders.

### Assessing the Link Between Sleep Duration and Quality in the Context of Sleep Disorders: A Comparative Analysis
This line plot provides a valuable visualization of how sleep quality correlates with sleep duration, further categorized by the presence of sleep disorders (None, Insomnia, Sleep Apnea). The insights that can be drawn from this visualization include:
**1. Correlation between Sleep Duration and Quality:**
- The plot shows the relationship between how long individuals sleep (sleep duration) and how well they rate their sleep (quality of sleep). A positive or negative trend in the line would indicate a direct or inverse relationship, respectively.
- For example, if the line rises with increased sleep duration, it suggests that longer sleep is associated with better perceived sleep quality.
**2. Impact of Sleep Disorders on Sleep Quality:**
- The different lines for each sleep disorder provide a comparative view of how sleep quality is affected in the presence of these conditions.
- Key observations could include whether individuals with certain sleep disorders (like Insomnia or Sleep Apnea) consistently rate their sleep quality lower than those without a sleep disorder, regardless of sleep duration.
- It’s also insightful to see if the relationship between sleep duration and quality differs significantly among the different sleep disorder groups.
**4. Variations and Patterns:**
- Look for any notable peaks, troughs, or patterns in the lines. For instance, a peak might suggest an optimal sleep duration for quality sleep, while a trough could indicate a sleep duration where quality diminishes.
- The spread and overlap of the lines can indicate how similar or different the sleep quality experiences are for individuals with different sleep disorders.
**5. Consistency Across Sleep Disorders:**
If the lines for different sleep disorders follow a similar pattern, it suggests a consistent effect of sleep duration on quality across these conditions. Divergent patterns, on the other hand, would indicate that the type of sleep disorder significantly alters this relationship.

This visualization is instrumental in understanding the complex dynamics between sleep duration, quality, and disorders, offering critical insights for sleep health research and potential interventions.

### Comparative Analysis of Sleep Quality Across Different Sleep Disorders
The boxplot visualization provides an insightful comparison of how sleep quality varies among individuals with different sleep disorders (None, Insomnia, Sleep Apnea). From this visualization, several key insights can be derived:

**1. Median and Spread of Sleep Quality Scores:**
- The median (central line in each box) gives a quick indication of the typical sleep quality rating for each disorder category.
- The range (length of the box) shows the variability in sleep quality within each group. A larger range indicates greater variability.
**2. Comparison Between Groups:**
- By comparing the median and range of each box, we can see how sleep quality differs between those with no sleep disorder, insomnia, and sleep apnea.
- For example, a lower median in the Insomnia group compared to the None group would suggest that insomnia is associated with poorer sleep quality.
**3. Outliers and Extremes:**
- Outliers (points outside the box) highlight individuals with sleep quality ratings that are notably different from the majority in their group. This can indicate exceptionally good or poor sleep quality within a disorder category.
- Whiskers (lines extending from the boxes) indicate the range of the majority of the data, excluding outliers. A long whisker might reveal a wider spread of experiences in sleep quality.
**4. Skewness in Distribution:**
- The symmetry or asymmetry of the boxes can indicate a skew in sleep quality ratings. For instance, a box skewed towards higher ratings in the 'None' group would suggest that most people without a sleep disorder generally rate their sleep quality positively.

This boxplot is essential for understanding the impact of different sleep disorders on perceived sleep quality. It allows for a direct comparison between groups, providing insights into the severity of the impact of various sleep disorders on sleep quality. This information is crucial for healthcare professionals and researchers focusing on sleep health and the management of sleep disorders.

### Gender Distribution Across Different Sleep Disorders: A Comparative Pie Chart Analysis
These pie charts provide a clear visualization of the gender distribution within each category of sleep disorders (None, Insomnia, Sleep Apnea). From this visualization, several insights can be gleaned:
**1. Gender Proportions in Each Sleep Disorder:**
- The charts show the percentage breakdown of males and females within each sleep disorder category.
- This helps to understand if there's a gender prevalence in any particular sleep disorder. For example, a significantly higher percentage of one gender in a disorder like Insomnia could suggest a gender predisposition.
**2. Comparative Analysis Across Disorders:**
- By looking at the pie charts side by side, you can compare the gender distribution across different sleep disorders.
- Notable differences in gender ratios between disorders may indicate varying susceptibility or diagnosis rates among males and females.
**3. Overall Gender Balance:**
- These charts also provide a visual representation of the overall gender balance within the study population, specifically in relation to sleep disorders.
- A balanced distribution in the 'None' category would indicate a representative sample, while a skewed distribution in any disorder category might suggest an area for further investigation.
**4. Identifying Gaps or Biases:**
- If any of the sleep disorders show a significant imbalance in gender distribution, it could point to potential gaps or biases in diagnosis, reporting, or the prevalence of the disorder itself.

These visualizations are particularly useful for healthcare professionals and researchers to identify potential gender-related patterns or biases in the prevalence and diagnosis of sleep disorders. They also contribute to a broader understanding of how sleep disorders might differentially affect males and females.

### Occupational Breakdown in Relation to Sleep Disorders: A Countplot Analysis
This countplot provides a detailed view of how various sleep disorders are distributed across different occupations. Key insights that can be drawn from this visualization include:
**1. Prevalence of Sleep Disorders by Occupation:**
- The plot shows the frequency of each sleep disorder (None, Insomnia, Sleep Apnea) within different occupational groups.
- This helps in identifying if certain occupations are more prone to specific sleep disorders. For instance, a high count of Insomnia in a particular occupation could indicate a stress-related or work-environment factor influencing sleep health.
**2. Occupational Stress and Sleep Health:**
- Occupations with a higher frequency of sleep disorders may suggest higher levels of job-related stress or lifestyle factors that negatively impact sleep.
- Conversely, occupations with a predominantly 'None' category for sleep disorders could imply more conducive work environments for sleep health.
**3. Comparative Analysis Across Occupations:**
- By comparing the counts across different occupations, we can assess which professions are most affected by sleep disorders.
- This can guide further investigation into occupational health practices and the need for specific interventions or support systems in high-risk occupations.
**4. Distribution Trends:**
- The distribution of sleep disorders within each occupation, especially the relative proportions of Insomnia and Sleep Apnea, can reveal specific occupational health concerns.
- For example, a high incidence of Sleep Apnea in physically demanding jobs could point towards factors like obesity or physical health conditions common in those occupations.

This countplot is an effective tool for identifying potential occupational risk factors for sleep disorders and can be instrumental in guiding workplace health policies, awareness campaigns, and targeted interventions to improve sleep health in the workforce.

### Interplay Between Sleep Duration, Quality, Physical Activity, and Sleep Disorders: A Multifaceted Pairplot Analysis
The pairplot offers a comprehensive view of the relationships between sleep duration, quality of sleep, physical activity level, and sleep disorders. It provides a multi-dimensional perspective, revealing insights into how these variables interact with each other:
**1. Sleep Duration vs. Quality of Sleep:**
- This plot helps in understanding if there is a correlation between how long people sleep and how they rate the quality of their sleep. A positive correlation would suggest that longer sleep might be associated with better sleep quality.
**2. Sleep Duration vs. Physical Activity Level:**
- This plot explores the relationship between physical activity and sleep duration. Insights here could include whether more physically active individuals tend to have longer or shorter sleep durations, suggesting a potential impact of physical activity on sleep.
**3. Quality of Sleep vs. Physical Activity Level:**
- This plot assesses if there’s a relationship between physical activity levels and perceived quality of sleep. For instance, higher physical activity might be associated with better sleep quality, or there might be no clear pattern.
**4. Influence of Sleep Disorders:**
- The hue differentiation based on sleep disorders allows for the comparison of these relationships in the context of different sleep disorders (None, Insomnia, Sleep Apnea).
- This aspect helps in determining whether the presence of a sleep disorder alters the typical patterns observed between sleep duration, quality, and physical activity.
**5. Distribution and Overlap:**
- The distribution of points in each plot, especially the degree of overlap between different sleep disorders, can provide insights into how distinct or similar these groups are in terms of their sleep and activity patterns.
**6. Patterns and Outliers:**
- Any notable patterns, clusters, or outliers in the plots can reveal unique insights, such as specific trends within a sleep disorder category or exceptional cases that deviate from general trends.

This pairplot is a powerful tool for visualizing and understanding the complex relationships between key variables related to sleep health. It is especially useful for identifying patterns and relationships that might not be immediately obvious and can guide further statistical analysis or research.

### Analyzing the Impact of Stress Levels on Mean Sleep Duration Across Sleep Disorders: A Heatmap Perspective
The heatmap provides a visually compelling analysis of how average sleep duration varies across different sleep disorders and stress levels. It combines these two key aspects to offer several insights:

**1. Interaction Between Stress Level and Sleep Disorders:**
- The heatmap allows for an examination of how mean sleep duration is influenced by both stress level and the type of sleep disorder. This can reveal if higher stress levels correlate with shorter sleep durations within specific sleep disorders.
**2. Comparative Mean Sleep Duration:**
- Each cell in the heatmap represents the average sleep duration for a specific combination of sleep disorder and stress level. This allows for direct comparison across different groups.
- For example, cells with warmer colors (indicating shorter sleep duration) in high stress levels can suggest a significant impact of stress on sleep duration, particularly in the context of certain sleep disorders.
**3. Patterns and Trends:**
- Any noticeable patterns, such as a consistent decrease in sleep duration with increasing stress levels across all sleep disorders, would be indicative of a strong link between stress and reduced sleep.
- Similarly, variations in the pattern for different sleep disorders can shed light on how these conditions interact with stress to affect sleep.
**4. Identifying Critical Combinations:**
- The heatmap highlights critical combinations of stress levels and sleep disorders where sleep duration is significantly affected. This could be crucial for targeted interventions.
- For instance, if individuals with insomnia under high stress levels show markedly reduced sleep durations, this group might require specific stress management interventions.
**5. Overall Trends and Anomalies:**
- The general color trend across the heatmap can indicate overall tendencies, while any anomalies (such as an unexpectedly high or low average sleep duration in a particular cell) can point to areas needing further investigation.

This heatmap is a valuable tool for healthcare professionals, researchers, and policymakers to understand the complex interplay between stress, sleep disorders, and sleep duration, guiding effective strategies for improving sleep health.

### Heart Rate Variations in Relation to Different Sleep Disorders
The boxplot provides a visual comparison of heart rate distributions across various sleep disorders (None, Insomnia, Sleep Apnea). This visualization offers several key insights:

**1. Median Heart Rate per Sleep Disorder:**
- The central line in each box represents the median heart rate for each sleep disorder category. Comparing these medians can reveal whether certain sleep disorders are associated with higher or lower median heart rates.
- For example, a higher median in the Sleep Apnea category might suggest a link between this disorder and elevated heart rates.
**2. Range and Variability of Heart Rates:**
- The length of each box (interquartile range) shows the spread of heart rates within each disorder category, indicating the variability in heart rate among individuals with the same sleep disorder.
- Wider boxes suggest greater variability, while narrower boxes indicate more uniform heart rates within that group.
**3. Outliers and Extremes:**
- Outliers (points outside the box) highlight individuals with heart rates significantly different from the majority in their group. This can indicate exceptional cases that might warrant further investigation.
- The whiskers (lines extending from the boxes) show the range of typical heart rates, excluding outliers. Long whiskers indicate a wider range of heart rates.
**3. Comparative Analysis Across Disorders:**
- By examining the position and spread of boxes across different sleep disorders, it's possible to assess how these conditions might impact heart rate.
- For instance, if the box for Sleep Apnea is noticeably higher or has more outliers than other categories, it might suggest a distinct impact of this disorder on cardiovascular health.
**4. Symmetry and Skewness:**
- The symmetry of the boxes can indicate whether the heart rate distribution is skewed higher or lower within each disorder category.

This boxplot is instrumental in understanding the potential cardiovascular implications of different sleep disorders. It can be particularly useful for healthcare professionals in identifying sleep disorders that may have a more pronounced effect on heart rate, guiding more targeted medical evaluations and interventions.

### Exploring the Link Between Physical Activity Levels and Sleep Disorders: A Boxplot Perspective
The boxplot visualization offers a clear comparison of physical activity levels across different sleep disorder categories (None, Insomnia, Sleep Apnea). This visualization provides several key insights:
**1. Median Physical Activity Level per Sleep Disorder:**
- The central line in each box indicates the median physical activity level for each sleep disorder category. This can reveal if certain sleep disorders are associated with higher or lower median activity levels.
- For example, a lower median in the Insomnia category might suggest reduced physical activity among individuals with this disorder.
**2. Range and Variability in Activity Levels:**
- The length of each box shows the spread of physical activity levels within each disorder group, indicating the variability among individuals.
- Wider boxes indicate a greater range of activity levels, suggesting diverse lifestyles within that sleep disorder category.
**3. Outliers and Extremes:**
- Outliers (points outside the box) highlight individuals with unusually high or low activity levels compared to the majority in their group. This can point to exceptional cases that might require additional scrutiny.
- The whiskers (lines extending from the boxes) show the typical range of activity levels, excluding outliers. Long whiskers indicate a broad range of physical activity levels.
**4. Comparative Analysis Across Disorders:**
- By comparing the position and spread of boxes across different sleep disorders, it's possible to assess how these conditions might correlate with physical activity levels.
- If a particular sleep disorder category consistently shows lower activity levels, it might suggest a link between that disorder and reduced physical activity.
**6. Symmetry and Distribution:**
- The symmetry of the boxes can provide insight into the distribution of activity levels. A skewed box might indicate a tendency towards either higher or lower activity levels within a sleep disorder category.

This boxplot is crucial for understanding the potential relationships between physical activity levels and different sleep disorders. It provides valuable insights for healthcare professionals and researchers, suggesting areas where lifestyle interventions might be beneficial, particularly for individuals with specific sleep disorders.

## Features Engineering and Modeling
The dataset has undergone comprehensive feature engineering, including standardization, encoding, and reduction of multicollinearity through correlation analysis. This process has refined the dataset into a format that is optimized for predictive modeling, ensuring that the features included are relevant and appropriately formatted for the analysis. The final feature set is expected to provide a strong foundation for developing a robust model to predict sleep disorders.
The process included the following:
1. Renaming Columns
•	Objective: To ensure consistency and ease of data handling.

•	Action: All column names were converted to lowercase, and spaces were replaced with underscores.

2. Encoding Blood Pressure
•	Objective: To create a more analytically useful representation of blood pressure.

•	Action: Calculated the ratio of systolic to diastolic blood pressure and stored it in a new column 'bp_ratio'.

3. Encoding the Target Variable
•	Objective: To transform the categorical target variable 'sleep_disorder' into a numerical format.

•	Action: Applied Label Encoding to the 'sleep_disorder' column, converting categories to numerical labels. A DataFrame (label_df) was created to map original and encoded labels.

4. One-Hot Encoding of Categorical Variables
•	Objective: To convert categorical variables into a format suitable for modeling.

•	Action: Applied One-Hot Encoding to 'occupation', 'gender', and 'bmi_category', with the first category dropped to avoid multicollinearity.

5. Correlation Analysis
•	Objective: To reduce collinearity and dimensionality in the dataset.

•	Action: Calculated the correlation matrix for the encoded dataset, excluding 'person_id', 'blood_pressure', and 'sleep_disorder'.

•	Visualized these correlations using a heatmap to identify highly correlated features.

6. Dropping Columns Based on Correlation Analysis
•	Objective: To remove features that are highly correlated or redundant.

•	Action: Dropped several columns, including 'person_id', 'blood_pressure', 'sleep_disorder', 'daily_steps', certain occupation categories ('occupation_Nurse'), 'stress_level', and 'quality_of_sleep'.

7. Final Feature Set
•	Objective: To define the final set of features for the predictive model.

•	Action: Created a final feature set named features by dropping the identified columns.

## Modeling
**Part 1: Basic Decision Tree Classifier**

1. Objective: To establish a baseline model using a Decision Tree Classifier.
2. Process:
- Feature-Target Split: Separated the dataset into features (X) and the target variable (y).
- Train-Test Split: Divided the data into training and testing sets with an 80-20 split, ensuring class stratification.
- Scaling: Standardized the features using StandardScaler to ensure equal weighting.
- Model Training: Fitted a Decision Tree Classifier on the training data.
- Model Evaluation: Evaluated the model on the test set and calculated accuracy. Also generated a classification report.

**Results:**
- Achieved an accuracy of 89.33%.
- Classification report indicated varying precision, recall, and F1-scores across different classes.

**Part 2: Hyperparameter Tuning Using Grid Search**
1. Objective: To optimize the Decision Tree model by tuning its hyperparameters.
2. Process:
- Defined a grid of hyperparameters, including max_depth, min_samples_split, min_samples_leaf, and criterion.
- Conducted Grid Search with cross-validation to find the best parameter combination.
- Evaluated the best parameters and score.

**Results:**
- The best parameters were found to be criterion: entropy, max_depth: None, min_samples_leaf: 1, and min_samples_split: 10.
- The best score from the grid search was approximately 88.3%.

**Part 3: Decision Tree Classifier with Optimized Parameters**
1. Objective: To apply the best parameters from grid search to the Decision Tree model.
2. Process:
- Initialized a new Decision Tree Classifier with the optimized parameters.
- Fitted the model to the training data and made predictions on the test set.
- Generated a classification report for the optimized model.

**Results:**
- The classification report showed improved precision, recall, and F1-scores, indicating better performance compared to the baseline model.
- The accuracy increased to approximately 93%.

**Part 4: Confusion Matrix Analysis**
1. Objective: To visually interpret the model's performance.
2. Process:
- Generated and printed the confusion matrix for the optimized model.
- Plotted the confusion matrix as a heatmap for better visualization.

**Results:**
- The confusion matrix provided a detailed breakdown of the model's predictions versus the actual values.
- The heatmap visualization assisted in identifying the model's performance in correctly predicting each class.

## Conclusion

Throughout the four-part modeling process for the Sleep Health and Lifestyle project, significant improvements were observed in the model's accuracy and recall rates. The final model, optimized through meticulous hyperparameter tuning, demonstrated an accuracy of approximately 93%, indicating a high level of proficiency in classifying sleep disorders.

However, given the medical nature of the case, it is crucial to acknowledge the possibility of further enhancing model performance. Exploring alternative modeling techniques or different data preprocessing methods could potentially yield even better results. Nonetheless, a threshold for model performance was set, keeping in mind the critical importance of accuracy in medical diagnoses.

This threshold serves a dual purpose: first, it ensures that the model maintains a high standard of accuracy and recall, which is vital in a medical context. Second, it acts as a precautionary measure, informing healthcare professionals that while the model is a valuable tool for initial screening, it is not infallible. In cases where the model indicates a sleep disorder, it is recommended that doctors conduct further examinations to confirm the diagnosis. This approach balances the efficiency of machine learning with the need for precision and caution in medical decision-making, ensuring the best possible care for patients.
