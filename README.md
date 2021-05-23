## Insurance companies and data scientists
The first thing that comes to mind when it comes to insurance is a call. Insurance calls were always annoying to get while busy or doing important things, but people did not hang up because they could not be rude to a very kind counselor. Insurance is basically based on compensation for events or accidents that will happen in the future. Therefore, insurance products are basically designed based on a model that predicts the future. In the case of life insurance, most insurance companies either build life expectancy prediction models, or they also build models that predict whether a person is interested in insurance, as in [Kaggle](https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction). Based on these models, you can calculate how much insurance you will set, how much you will pay for it, or what the insurer's expected profits will be. So, for this project, let's create a model to predict whether you are interested in car insurance through customer information of a particular company using the above caval dataset!


## Project Background
The original description of the Kaggle is as follows.

- *Our client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the policyholders (customers) from the past year will also be interested in Vehicle Insurance provided by the company.*

Among customers who have been subscribed to health insurance since last year, the goal is to design a model that predicts whether they are interested in car insurance or not. The goal is to communicate with interested customers through the results of the prediction model, optimize automobile insurance design, and maximize profits. The data set provided by the insurance company includes demographic data (gender, age, region code type), vehicle age, and health insurance information (premium, sourcing channel).

## Data

The dataset is obataiend from [Kaggle](https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction). Train data contains information from 354,405 customers and has 12 features. Test data has a total of 11 features, excluding our target features, for a total of 127,037 customer information. This shows that our target feature is Response. Now let's check what information each feature contains.


## Results  
|Model|F1 score|Area Under Curve(AUC)|Hyper Parameter Optimization|
|:----------:|:-------------:|:------:|:------:|
|RandomForest|0.15|0.8462593298989705| RandomizedSearchCV |
|XGB|0.46|0.8646973570321353| optuna |
|LGBM| 0.44  |0.866483369025105 | None |
  
