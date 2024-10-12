# PlayerMarketValue-AnalyticsProject

### Data Analysis

In predicting the market value of football players, we started by examining key features that may influence our target variable. One of the significant observations was the disparity in average market values across different leagues. The English Premier League (EPL) consistently showed higher average market values compared to other leagues. This can be attributed to factors such as a broader audience, substantial investments from wealthy owners, and the presence of elite coaching, which enhance both performance and revenue.

<img width="544" alt="Screenshot 2024-10-12 at 7 03 19 PM" src="https://github.com/user-attachments/assets/ffc41c11-27a5-4343-839c-9ef1735ad08e">

Aggregating players by the top 20% market value per league revealed a narrower gap, but the EPL still maintained a noticeable advantage. Delving deeper into player positions, left-wingers emerged as the highest valued, showcasing an average market value approximately $4M above other positions. This reflects the importance of skill sets like dribbling and pace, often displayed by legendary players such as Ronaldinho and Thierry Henry.

<img width="543" alt="Screenshot 2024-10-12 at 7 03 35 PM" src="https://github.com/user-attachments/assets/5793f66e-8535-4cd2-9a50-39dc52969ae1">

In 2019, Neymar Jr. topped the valuation chart at $175M, followed closely by Eden Hazard and Lionel Messi. Notably, five out of the ten highest-valued players were left-wingers, reinforcing the position's market dominance.

<img width="463" alt="Screenshot 2024-10-12 at 7 03 47 PM" src="https://github.com/user-attachments/assets/6a8fe56f-4006-4c80-9409-d46f890a98a1">

### Key Predictors

Analyzing the correlation metrics, we identified several top predictors for market value. The most significant predictor was ThruBalls, highlighting the importance of line-breaking passes in enhancing market value. Progressive Carries and Goal Creating Actions (GCA) also ranked high, emphasizing actions that lead to scoring opportunities. Additionally, the npxG+xA metric illustrates the value of quality chances created, adding depth to our understanding of player contributions.


### Data Preprocessing
We employed dummy encoding for categorical variables and checked for normality in the data. The target variable displayed a right-skewed distribution, indicating that transformations were not applied, as they could compromise interpretability. Standardization was performed to mitigate biases due to varying feature magnitudes, ensuring that features such as GCA and xA were comparably weighted in our models.

<img width="480" alt="Screenshot 2024-10-12 at 7 04 48 PM" src="https://github.com/user-attachments/assets/e78f9396-919a-4ca6-a169-671da7d79187">

### Machine Learning Models
To predict market values, we split the data into training and test sets, utilizing various regression algorithms to determine the model with the best performance. The models tested included:

Simple Linear Regression
Ridge Regression
Lasso Regression
K Nearest Neighbors
Random Forest
Neural Networks

#### Prediction Results – Phase 1
In the initial phase, we encountered issues with NaN and infinite values in binary features. After removing these, the Mean Absolute Deviation (MAE) metric was employed for model evaluation due to its interpretability in the context of football analytics. The Random Forest Regressor emerged as the top-performing model, achieving the lowest MAE.

<img width="316" alt="Screenshot 2024-10-12 at 7 02 19 PM" src="https://github.com/user-attachments/assets/b04c0b6b-020a-49e7-a9fb-5da3b2ebe8aa">


#### Prediction Results – Phase 2
In the second phase, we reintroduced binary features for position and league, using the same models with an additional focus on Neural Networks. This enhancement in the dataset improved the performance metrics across the board, suggesting the importance of comprehensive feature representation in model training.

<img width="547" alt="Screenshot 2024-10-12 at 7 02 33 PM" src="https://github.com/user-attachments/assets/85fff7e8-4ed4-41e2-9595-e1564db99051">


### Conclusion
The analysis underscored the critical features influencing player market value while demonstrating the efficacy of machine learning models in accurately predicting these values. The insights gained pave the way for further exploration into player valuation dynamics, offering valuable perspectives for stakeholders in the football industry.
