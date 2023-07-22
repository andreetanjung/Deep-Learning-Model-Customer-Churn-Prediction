# Deep-Learning-Model-Customer-Churn-Prediction
### Project Overview
Predicting Customer Churn with ANN Model

In this notebook will attempt to predict the customers are going to churn or not using ANN sequential and functional model based on the information about the purchasing behavior of customers on the company's website. The objective is to implement an artificial neural network model capable of accurately classifying the likelihood of customer churn based on the provided dataset.
### Data
The data was obtained via academy bootcamp and has been uploaded as `churn.csv`. The dataset provides information about the purchasing behavior of customers on the company's website.

Data field description:
| Column | Description |
| --- | --- |
| `user_id` | ID of a customer |
| `age` | Age of a customer |
| `gender` | Gender of a customer |
| `region_category` | Region that a customer belongs to |
| `membership_category` | Category of the membership that a customer is using |
| `joining_date` | Date when a customer became a member |
| `joined_through referral` | Whether a customer joined using any referral code or ID |
| `preferred_offer types` | Type of offer that a customer prefers |
| `medium_of operation` | Medium of operation that a customer uses for transactions |
| `internet_option` | Type of internet service a customer uses |
| `last_visit_time` | The last time a customer visited the website |
| `days_since_last_login` | Number of days since a customer last logged into the website |
| `avg_time_spent` | Average time spent by a customer on the website |
| `avg_transaction_value` | Average transaction value of a customer |
| `avg_frequency_login_days` | Number of times a customer has logged in to the website |
| `points_in_wallet` | Points awarded to a customer on each transaction |
| `used_special_discount` | Whether a customer uses special discounts offered |
| `offer_application_preference` | Whether a customer prefers offers |
| `past_complaint` | Whether a customer has raised any complaints |
| `complaint_status` | Whether the complaints raised by a customer was resolved |
| `feedback` | Feedback provided by a customer |
| `churn_risk_score` | Churn score <br><br> `0` : Not churn <br> `1` : Churn |
### Methodology
- Data preprocessing: make sure the data has no duplicate and missing value
- Exploratory data: understand more about the data with visualization
- Feature engineering and selection: using pipeline to handle missing value, outlier, and encoding. For the feature selection we use phik matrix, recursive feature elimination, and mutual info classification to compare and combine.
- Model Architecture: in here we build both sequential and functional model and comparing both result
- Model Tuning: use the best model from above to be tuned to get more better result
### Result and Evaluation
![image](https://github.com/andreetanjung/Deep-Learning-Model-Customer-Churn-Prediction/assets/123824152/5367a712-819f-4eeb-aacc-ed7931f0bed7)
<sub>model sequential after parameter tunning<sub>

![image](https://github.com/andreetanjung/Deep-Learning-Model-Customer-Churn-Prediction/assets/123824152/d09998d5-1bb2-49b4-bc4d-eaa88cc29fc8)
<sub>model functional after parameter tunning<sub>

![image](https://github.com/andreetanjung/Deep-Learning-Model-Customer-Churn-Prediction/assets/123824152/ace933eb-0828-4d41-8b7b-e04aa9933325)

<sub>confusion matrix from functional after parameter tunning<sub>

Based on the classification report, it appears that the model has a high accuracy in predicting both class 0 and class 1, indicating that it is effective in predicting individuals who are likely to churn and those who are likely to stay. The confusion matrix further supports this, as it shows a low number of false negatives and false positives. This means that the model can help the business identify which customers require more attention and which promotions may be most effective in retaining them
### Directory Structure and Brief Description of Files
`h8dsft_P2M1_Andrian_Tanjung.ipynb`is a Jupyter notebook that contains the complete project code, including data pre-processing, feature engineering with model, and evaluation.

### Model Deployment
Model deployment link: https://huggingface.co/spaces/andreetanjung/Milestone1-phase2
