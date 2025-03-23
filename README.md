# Credit Card Default Prediction

## Introduction
In today's rapidly evolving financial landscape, understanding consumer credit behavior is more critical than ever. With credit playing a vital role in both personal and business transactions, financial institutions constantly seek ways to mitigate risk and predict potential defaults. This project was born from the need to leverage data-driven insights to forecast credit card defaults accurately.

Developed as a graded challenge by Ogi Hadicahyo under the Hacktive8 curriculum (Batch HCK - 012, Phase 1), this project harnesses a comprehensive dataset from Google Cloud. Through meticulous exploratory data analysis and advanced machine learning techniques, the project aims to transform raw data into actionable insights, helping stakeholders make informed decisions in credit risk management.

## Main Feature
- **Data Loading and Exploration:**  
  The journey begins with importing a detailed dataset on credit card defaults. An initial exploratory data analysis (EDA) reveals hidden patterns and anomalies, setting the foundation for deeper insights.

- **Data Preprocessing:**  
  Building a reliable model requires a clean slate. The data undergoes rigorous cleaning, handling missing values, encoding categorical variables, and applying normalization techniques to ensure consistency and reliability.

- **Model Development:**  
  A variety of classification algorithms are explored to predict credit card defaults. Each model is carefully tuned and optimized, reflecting the iterative nature of crafting a robust predictive tool.

- **Model Evaluation:**  
  Comprehensive evaluation is performed using key metrics such as Accuracy, Precision, Recall, and F1 Score. Detailed visualizations including confusion matrices and performance graphs provide clarity on the model's strengths and areas for improvement.

- **Deployment:**  
  The final model is deployed on Hugging Face Spaces, transforming theoretical insights into a practical, interactive application. This enables real-time testing and showcases the model’s potential impact on financial decision-making.

## Methodology
The project follows a structured and methodical approach:

1. **Data Collection:**  
   The process begins with acquiring a rich dataset from Google Cloud that contains detailed information on credit card defaults. This dataset forms the backbone of the analysis and provides the necessary features to model consumer credit behavior.

2. **Exploratory Data Analysis (EDA):**  
   A thorough exploration of the dataset is conducted to uncover trends, patterns, and anomalies. This step involves visualizing data distributions and identifying key variables that may influence credit default, laying the groundwork for effective feature engineering.

3. **Data Preprocessing:**  
   With raw data in hand, preprocessing transforms it into a format suitable for modeling. Tasks include cleaning the data by addressing missing values and inconsistencies, encoding categorical variables into numerical formats, and applying normalization or scaling techniques to ensure that the features are on a comparable scale.

4. **Model Building:**  
   Multiple classification models are built and refined. The dataset is divided into training and testing subsets, and each model undergoes hyperparameter tuning to enhance its predictive power. The models explored include Logistic Regression, Support Vector Machine (SVM), and K-Nearest Neighbors (KNN).

5. **Model Evaluation:**  
   After an extensive process of hyperparameter tuning and model comparison, the Support Vector Machine (SVM) model emerged as the most effective approach. The evaluation phase involved assessing performance metrics such as Accuracy, Precision, Recall, and F1 Score, and leveraging visualizations like confusion matrices to compare the strengths and weaknesses of each model. This comprehensive analysis guided the selection of the best-performing model without revealing the specific numerical outcomes in this section.

6. **Deployment:**  
   The journey culminates in the deployment of the best-performing SVM model on Hugging Face Spaces. This interactive platform allows users to test and explore the model’s predictions in real time, bridging the gap between theoretical analysis and practical application.

## Results
The final SVM model, which stood out among the alternatives, achieved an overall accuracy of 57% on both training and testing datasets. In the training phase, the model exhibited a strong ability to classify non-defaulters with a high precision of 0.86 and a moderate recall of 0.54, resulting in an F1 score of around 0.66, while the default class showed a lower precision of 0.28 paired with a higher recall of 0.68, leading to an F1 score of approximately 0.40. This trend continued in the test phase, where the non-default class achieved a precision of 0.84 and a recall of 0.56, yielding an F1 score close to 0.67, and the default class recorded a precision of 0.29 and a recall of 0.64 with an F1 score near 0.40. These consistent results between training and testing phases highlight the robustness of the model, while also emphasizing the inherent challenges in credit risk prediction—particularly the delicate balance between accurately identifying defaulters and non-defaulters.

## Skills and Tools
This project is a blend of technical expertise and innovative problem-solving. The following skills and tools played a crucial role in its development:

- **Python:** The primary programming language that provided a powerful environment for data manipulation and machine learning.
- **Jupyter Notebook:** An interactive platform that facilitated the seamless integration of code, visualizations, and narrative documentation.
- **Pandas & NumPy:** Essential libraries for data manipulation, cleaning, and performing complex numerical computations.
- **Scikit-learn:** The machine learning library that enabled the implementation, training, and evaluation of various classification models.
- **Matplotlib:** A visualization library used to create clear, informative graphs and charts that illustrate key findings.
- **Hugging Face Spaces:** A modern deployment platform that allowed for the interactive demonstration of the predictive model in a real-world setting.
- **Google Cloud:** The source of the rich dataset, providing access to comprehensive information on credit card defaults.

## File Descriptions
- **Credit_Card_Default_Prediction.ipynb:**  
  This Jupyter Notebook encapsulates the entire project workflow—from data ingestion and exploratory analysis to model building, evaluation, and deployment.
- **Credit_Card_Default_Prediction_Inference.ipynb:**  
  This Jupyter Notebook encapsulates the Additional notebook focusing on further model insights.
- **Credit Card Dataset.csv:**  
  This .csv file contains the dataset used in this project.

## References
- **Dataset:**  [Credit Card Default Dataset on Google Cloud](https://console.cloud.google.com/bigquery?p=bigquery-public-data&d=ml_datasets&t=credit_card_default&page=table&pli=1&project=hacktive8-408704&ws=!1m9!1m4!4m3!1sbigquery-public-data!2sml_datasets!3scredit_card_default!1m3!8m2!1s805845835069!2s5fed4d090c56455390a4def8abaf5adb)

- **Deployment:**   [Hugging Face Spaces - Default Credit Card](https://huggingface.co/spaces/OgiHadicahyo/Default_Credit_Card)
