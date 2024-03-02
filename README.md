# NFL Prediction: Touchdowns

## Project Summary

### Overview
In this project, I set out to forecast NFL quarterbacks' touchdown counts for a season based on their performance data from the previous season. Utilizing machine learning algorithms, I built models that correlate various performance indicators with the number of touchdowns scored, aiming to predict future successes on the field.

### Data Preparation
The dataset comprised play-by-play data from the 2019 to 2021 NFL seasons. After a thorough cleaning process to ensure data quality, I selected features I believed would be indicative of a quarterback's ability to score touchdowns, including pass attempts, completions, interceptions, sacks, and yards gained from the previous season.

### Feature Engineering
I constructed new features to reflect a quarterback's performance in the season prior to the one I aimed to predict. This approach rests on the assumption that the previous season's performance metrics are predictive of the next season's touchdown scores.

### Model Selection and Training
Two regression models were utilized in this analysis:
- **Linear Regression:** A straightforward approach that assumes a linear relationship between the selected features and the number of touchdowns.
- **Ridge Regression:** An extension of linear regression that includes regularization to reduce overfitting and improve model generalizability.

I trained these models using the 2020 season data, allowing me to test their predictions against the actual 2021 season outcomes.

### Cross-Validation and Performance Metrics
To evaluate and fine-tune the models, I employed cross-validation techniques and calculated the Root Mean Squared Error (RMSE). This provided a measure of the models' prediction errors. Additionally, I computed the R-squared (R²) metric to determine the proportion of variance in touchdown scores the models could explain.

### Results
The models delivered promising results, with the Ridge Regression demonstrating a degree of robustness thanks to its regularization component. However, there was a tendency for the models to predict more accurately for quarterbacks with higher touchdown counts, while less accurate for those with fewer scores.

### Detailed Findings
For instance, the models predicted A. Rodgers to score 35.67 touchdowns, but he exceeded this with 58 actual scores. T. Brady was also predicted to score less than he actually did, with a prediction of 38.39 touchdowns against an actual score of 52.

### Visualization
The scatter plot of actual versus predicted touchdowns revealed a strong linear trend, endorsing the models' effectiveness for higher-scoring quarterbacks. However, the dispersion around the line for lower touchdown counts indicated that predictions for these players could be improved.

![image](https://github.com/prayagpadwal/NFL-prediction-touchdowns/assets/65147413/f197dff8-3689-4011-983d-77c87c4c48f1)

![image](https://github.com/prayagpadwal/NFL-prediction-touchdowns/assets/65147413/08458325-c536-483b-98ea-0a5a2b8e0980)

The analysis confirmed that past performance could be indicative of future success, but also highlighted the potential for refining the models. Future iterations will explore additional data sources, potentially encompassing off-field factors, to enhance the models' predictive accuracy across the full range of player performances.
