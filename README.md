# Pharmacy-Sales-Analysis
# Introduction:
The pharmaceutical industry relies heavily on accurate forecasting of drug consumption to optimize production and distribution. Accurate predictions enable efficient resource allocation and inventory management. In this context, data-driven approaches, specifically machine learning models, have proven effective in forecasting drug consumption based on historical data. This project aims to leverage machine learning techniques, particularly XGBoost regression, to predict drug consumption in the pharmaceutical sector.

# oneAPI
   oneAPI is an open, standards-based programming model designed to simplify development across diverse computing architectures. It is an initiative led by Intel, aiming to provide a unified programming model for heterogeneous computing environments, including CPUs, GPUs, FPGAs, and other accelerators.Optimizing code for oneAPI involves leveraging the features and tools provided by the oneAPI programming model to achieve better performance on diverse computing architectures.For optimizing your XGBoost project with oneAPI, start by installing the oneAPI toolkit on your system. When building XGBoost from source, use the Intel C++ Compiler (icc) from the oneAPI toolkit for potential performance improvements on Intel CPUs. Alternatively, consider using the Intel Distribution for XGBoost, specifically designed for Intel architectures. If you have Intel GPUs and aim to offload computations to the GPU using oneAPI, modify the XGBoost code or use compatible APIs such as DPC++. Profiling tools like Intel VTune Profiler can help identify performance bottlenecks. Stay updated by referring to the official documentation of XGBoost, the oneAPI toolkit, and relevant tools, as software features may evolve. These steps ensure an optimized integration of XGBoost with oneAPI for efficient machine learning on Intel architectures in your project.
![Screenshot 2024-01-28 220247](https://github.com/Nithish-Kanagaraj/Pharmacy-Sales-Analysis/assets/143336408/337f673c-37bd-4dbe-9cc1-c95c40acc178)


# Objective:
The primary objective of this project is to develop a robust and accurate model for predicting drug consumption in the pharmaceutical industry. The model is trained on historical data, considering factors such as time, day, and drug type. By utilizing XGBoost regression and optimizing hyperparameters through grid search, the goal is to create a reliable tool for forecasting drug consumption. The proposed system is designed to provide pharmaceutical companies with insights into future demand, enabling them to make informed decisions regarding production planning and supply chain management.

# Proposed System:
The proposed system involves several key steps:

1. *Data Exploration and Visualization:* The initial phase involves exploring and visualizing historical drug consumption data. Various plots and charts, such as line charts and bar charts, are utilized to understand consumption trends over time, by drug category, and on a monthly or yearly basis.

2. *Data Preprocessing:* The dataset undergoes preprocessing steps, including encoding categorical variables using LabelEncoder and melting the data to facilitate machine learning model training.

![WhatsApp Image 2024-01-28 at 21 47 51_28f9ed1c](https://github.com/Nithish-Kanagaraj/Pharmacy-Sales-Analysis/assets/143336408/952d0239-3eca-4f8d-9497-d2b08622d96d)


3. *Model Training:* XGBoost regression is chosen as the predictive model due to its effectiveness in handling complex relationships within the data. The model is trained on historical data, with an emphasis on features such as year, month, day, and drug type.

4. *Hyperparameter Tuning:* Grid search is employed to optimize the hyperparameters of the XGBoost model, ensuring the best possible performance. The grid search explores combinations of parameters such as the number of trees, learning rate, maximum depth, subsample ratio, and column subsample ratio.

![WhatsApp Image 2024-01-28 at 21 47 51_fa2fe09f](https://github.com/Nithish-Kanagaraj/Pharmacy-Sales-Analysis/assets/143336408/faf2ad2d-bc3b-4ac9-8616-625bf40b46db)


5. *Model Evaluation:* The model's performance is evaluated using metrics such as mean squared error on a test set. This step ensures the model's ability to generalize to new, unseen data.

6. *Deployment and Prediction:* Once the model is trained and optimized, it is deployed and used to predict drug consumption for a specified time period and drug category.

![WhatsApp Image 2024-01-28 at 21 47 51_7df69568](https://github.com/Nithish-Kanagaraj/Pharmacy-Sales-Analysis/assets/143336408/3e45a320-c43f-43da-9a1f-7e2e070ff4b6)

7. *User Inteface:* Once the forecast is generated, you can view the predicted drug consumption for the selected timeframe through interactive visualizations and charts.
# Features:

1. *Billing Software:* MediBilling is a robust and user-friendly billing software designed specifically for healthcare professionals and medical facilities. Whether you're a small clinic or a large hospital, our software offers a comprehensive solution to manage all aspects of your billing needs efficiently.
   
# Conclusion:
In conclusion, this project demonstrates the application of machine learning, specifically XGBoost regression, in predicting drug consumption in the pharmaceutical industry. By analyzing historical data and optimizing the model's hyperparameters, the proposed system provides accurate and reliable forecasts. This tool empowers pharmaceutical companies to make proactive decisions in production and supply chain management, ultimately improving efficiency and reducing costs. The project showcases the potential of data-driven approaches in enhancing decision-making processes within the pharmaceutical sector.
