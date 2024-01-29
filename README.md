# Pharmacy-Sales-Analysis
# Introduction:
The pharmaceutical industry relies heavily on accurate forecasting of drug consumption to optimize production and distribution. Accurate predictions enable efficient resource allocation and inventory management. In this context, data-driven approaches, specifically machine learning models, have proven effective in forecasting drug consumption based on historical data.In addition to leveraging machine learning techniques for drug consumption prediction, this project also incorporates the development of a billing software feature for the pharmaceutical sector. This billing software aims to streamline the financial aspects of the industry by automating the billing process and providing accurate and efficient invoicing for pharmaceutical products.The billing software feature will be seamlessly integrated into the overall system, allowing pharmaceutical companies to generate invoices and manage financial transactions with ease.The addition of report analysis prediction to the project allows for the prediction of sales analysis. With this feature, the billing software can generate comprehensive reports that provide insights into sales patterns and trends.

# oneAPI
   oneAPI is an open, standards-based programming model designed to simplify development across diverse computing architectures. It is an initiative led by Intel, aiming to provide a unified programming model for heterogeneous computing environments, including CPUs, GPUs, FPGAs, and other accelerators.Optimizing code for oneAPI involves leveraging the features and tools provided by the oneAPI programming model to achieve better performance on diverse computing architectures.For optimizing your XGBoost project with oneAPI, start by installing the oneAPI toolkit on your system. When building XGBoost from source, use the Intel C++ Compiler (icc) from the oneAPI toolkit for potential performance improvements on Intel CPUs. Alternatively, consider using the Intel Distribution for XGBoost, specifically designed for Intel architectures. If you have Intel GPUs and aim to offload computations to the GPU using oneAPI, modify the XGBoost code or use compatible APIs such as DPC++. Profiling tools like Intel VTune Profiler can help identify performance bottlenecks. Stay updated by referring to the official documentation of XGBoost, the oneAPI toolkit, and relevant tools, as software features may evolve. These steps ensure an optimized integration of XGBoost with oneAPI for efficient machine learning on Intel architectures in your project.


![image](https://github.com/Nithish-Kanagaraj/Pharmacy-Sales-Analysis/assets/143336408/aec204f5-04cd-4281-9c0e-743bb4e77168)


# Objective:
The primary objective of this project is to develop a robust and accurate model for predicting drug consumption in the pharmaceutical industry. The model is trained on historical data, considering factors such as time, day, and drug type. By utilizing XGBoost regression and optimizing hyperparameters through grid search, the goal is to create a reliable tool for forecasting drug consumption. this project also incorporates the development of a billing software feature for the pharmaceutical sector.The addition of report analysis prediction to the project allows for the prediction of sales analysis. With this feature, the billing software can generate comprehensive reports that provide insights into sales patterns and trends.

# Proposed System:
The proposed system involves several key steps:

1. *Data Exploration and Visualization:* The initial phase involves exploring and visualizing historical drug consumption data. Various plots and charts, such as line charts and bar charts, are utilized to understand consumption trends over time, by drug category, and on a monthly or yearly basis.

2. *Data Preprocessing:* The dataset undergoes preprocessing steps, including encoding categorical variables using LabelEncoder and melting the data to facilitate machine learning model training.

![image](https://github.com/Nithish-Kanagaraj/Pharmacy-Sales-Analysis/assets/143336408/6328a7ae-bd75-4039-8204-9fa6ef748d90)




3. *Model Training:* XGBoost regression is chosen as the predictive model due to its effectiveness in handling complex relationships within the data. The model is trained on historical data, with an emphasis on features such as year, month, day, and drug type.

4. *Hyperparameter Tuning:* Grid search is employed to optimize the hyperparameters of the XGBoost model, ensuring the best possible performance. The grid search explores combinations of parameters such as the number of trees, learning rate, maximum depth, subsample ratio, and column subsample ratio.

5. *Model Evaluation:* The model's performance is evaluated using metrics such as mean squared error on a test set. This step ensures the model's ability to generalize to new, unseen data.

6. *Deployment and Prediction:* Once the model is trained and optimized, it is deployed and used to predict drug consumption for a specified time period and drug category.

![image](https://github.com/Nithish-Kanagaraj/Pharmacy-Sales-Analysis/assets/143336408/a39703c7-566e-436f-8ff3-dc56b2eeed65)



7. *User Inteface:* Once the forecast is generated, you can view the predicted drug consumption for the selected timeframe through interactive visualizations and charts.
# Features:

1. *UserLogin:* A login ID is provided to users to access a system or platform specifically designed for managing sales-related activities. With their unique login ID, individuals can log in to the system, track sales data, process orders, manage inventory, and perform other sales-related tasks efficiently and securely.

![image](https://github.com/Nithish-Kanagaraj/Pharmacy-Sales-Analysis/assets/143336408/e4b96191-e04a-423c-83fa-2b30550bbfad)


   
2. *Billing Software:* Billing is a robust and user-friendly billing software designed specifically for healthcare professionals and medical facilities. Whether you're a small clinic or a large hospital, our software offers a comprehensive solution to manage all aspects of your billing needs efficiently.

![IMG-20240129-WA0008](https://github.com/Nithish-Kanagaraj/Pharmacy-Sales-Analysis/assets/143336408/c59f958c-e84a-4995-8b50-93440307c5ee)

3. *Overall Sales Analysis:* Analytics offers powerful tools and analytics to help you understand and optimize your overall sales performance. Whether you're a small business or a large enterprise, our platform provides the insights you need to make data-driven decisions and drive growth.

![image](https://github.com/Nithish-Kanagaraj/Pharmacy-Sales-Analysis/assets/143336408/63c2f84a-4b8b-466a-88bf-a25f26fb0e21)

![image](https://github.com/Nithish-Kanagaraj/Pharmacy-Sales-Analysis/assets/143336408/a822738a-264d-44cd-835c-3edf7b920f91)

# Setup:
1.Open XGBOOSTER.ipynb file in Jupyter notebook.

2.Upload the dataset Salesdaily.csv in the Jupyter notebook.

The coding is provided to perform the below in XGBOOSTER.ipynb:

i.Explore the data

ii.Train the machine learning model

iii.Launch the Gradio interface for real-time predictions

Before running the code run the following commands to install the necessary dependencies
import pandas as pd

pip install scikit-learn

pip install gradio

from sklearnex import patch_sklearn

patch_sklearn()
# Conclusion:
In conclusion, this project demonstrates the application of machine learning, specifically XGBoost regression, in predicting drug consumption in the pharmaceutical industry. By analyzing historical data and optimizing the model's hyperparameters, the proposed system provides accurate and reliable forecasts. This tool empowers pharmaceutical companies to make proactive decisions in production and supply chain management, ultimately improving efficiency and reducing costs. The project showcases the potential of data-driven approaches in enhancing decision-making processes within the pharmaceutical sector.
