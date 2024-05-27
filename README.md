# Bitcoin_Price_Forecasting

![BITCOIN](https://github.com/23Soham/Bitcoin_Price_Forecasting/assets/144841969/f494dc84-991d-4516-a453-18a4c8a1abfc)


## **Background**
Bitcoin's market volatility represents both a risk and an opportunity for investors, analysts, and traders. With the increasing adoption of cryptocurrencies, understanding and predicting price movements of Bitcoin is crucial for risk management and investment strategy. By harnessing the power of extensive historical datasets, such as the one capturing over three million Bitcoin price records from 2017 to 2023, financial experts can employ advanced machine learning algorithms to identify trends, patterns, and anomalies that traditional analysis might miss.

This data-driven approach can provide deeper insights into the intricacies of market dynamics, enabling predictive models that can alert to potential price swings. By analyzing detailed attributes like open, high, low, and close prices in combination with trading volumes and timestamps, these models can unveil underlying factors that influence market behavior. The result is a more informed strategy that helps in mitigating risks associated with Bitcoin's notorious price fluctuations and in capitalizing on market trends, thus contributing to a more stable and secure cryptocurrency market environment.

## **Motivation**
The motivation behind analyzing the Bitcoin price dataset is to develop a predictive model that can accurately forecast Bitcoin's price fluctuations. By understanding the intricate patterns within the historical price data, the model aims to anticipate market trends, aiding investors in making informed decisions. Effective predictions could minimize risks and maximize returns by timing the market more accurately. Furthermore, such a model could enhance market efficiency, contribute to academic research on cryptocurrency behavior, and potentially inform regulatory decisions for a more stable financial landscape in the digital age.

## **Goals**
The primary goal is to create an accurate and reliable predictive model that can effectively forecast Bitcoin's price movements. This model is intended to enable stakeholders to understand, anticipate, and react to market trends, potentially leading to more informed decisions, reduced financial risk, and optimized investment strategies in the volatile cryptocurrency market.

1. Develop a predictive analytics model capable of forecasting Bitcoin's price movement by analyzing historical data from 2017 to 2023, using this extensive dataset to understand past trends and anticipate future changes.
2. Process and clean the dataset, ensuring the integrity of the data by handling any anomalies, missing values, or outliers that could skew the predictive model's accuracy.
3. Utilize a variety of statistical methods and machine learning algorithms to capture the complex dynamics of Bitcoin's price fluctuations, evaluating each model to find the most effective approach.
4. Determine the key factors that most significantly impact Bitcoin's price, such as trading volume or specific time intervals, and incorporate these into the model to enhance prediction precision.
5. Offer actionable insights and strategic recommendations based on the model’s findings to support investors, financial analysts, and market observers in making data-driven decisions in the cryptocurrency market.

## **Methodology**

### **Understanding the Dataset**
This phase involves understanding through data acquisition, cleaning, and preprocessing, which includes filling missing values, removing outliers, scaling features, and engineering new features for better model performance.

### **Exploratory Data Analysis**
Exploratory Data Analysis (EDA) will present a detailed examination of the Bitcoin price dataset, which includes over 3 million records from 2017 to 2023. The analysis will:

- Describe the data, highlighting key features like timestamp, open, high, low, close prices, and trading volume.
- Assess the completeness of the data, identifying any missing values or outliers.
- Explore patterns in price movements on an intraday basis and across different time frames to uncover any recurring trends.
- Investigate periods of high volatility and potential correlations with market or global events.
- Examine long-term price trends to understand how Bitcoin’s value has evolved over the years.
- Analyze the relationship between trading volume and price changes to determine the impact of market activity on price dynamics.
- Charts, graphs, and visual representations will be used to illustrate our findings, providing clear insights into Bitcoin’s market behavior. The goal is to understand the nuances of the dataset thoroughly, forming the basis for predictive modeling and further research.

### **Feature Engineering**
Feature engineering is crucial for effective machine learning in dynamic domains like cryptocurrency markets. In Bitcoin price forecasting, temporal features play a key role. These include:

Year: Captures long-term trends.
Month: Identifies seasonal patterns.
Day: Reflects pay cycle effects.
Weekday: Accounts for differences between weekdays and weekends.
Hour: Captures intraday volatility.
By leveraging these features, models can better grasp temporal correlations, leading to more accurate price forecasts in the 24/7 Bitcoin market.

<img width="359" alt="image" src="https://github.com/23Soham/Bitcoin_Price_Forecasting/assets/144841969/5005428e-68e2-4763-8371-7c00a8aaab41">


### **Metrics Used**
Since the output variable would range from 0 to 1, it is said to be a Regression model. Therefore the metrics that were considered are as follows:

- [Accuracy](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.accuracy_score.html)
- [Precision](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_score.html)
- [Recall](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.recall_score.html)
- [F1 Score](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html)
- [Confusion Matrix](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.confusion_matrix.html)

### **Machine Learning Models**
Following are the Machine learning Models used:

- [Logistic Regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
- [Gaussian Naive Bayes](https://scikit-learn.org/stable/modules/naive_bayes.html#gaussian-naive-bayes)
- [Decision Tree Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)
- [Random Forest Classifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)

### **Comparison of RMSE Across Different Machine Learning Models**

<img width="468" alt="image" src="https://github.com/23Soham/Bitcoin_Price_Forecasting/assets/144841969/7c3e2371-40ba-402d-9398-af1e461ee029">

Lower RMSE indicates better prediction accuracy. In comparing four regression models, Linear Regression performs best with RMSE of 12.91, suggesting strong fit. Random Forest follows closely at 15.58, showing good predictive performance. XGBoost's high RMSE of 123.07 may be due to suboptimal tuning. Decision Tree has highest RMSE at 490.28, possibly overfitting training data. Linear Regression and Random Forest are most accurate in this case.

