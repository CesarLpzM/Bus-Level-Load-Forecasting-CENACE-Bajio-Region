⚡ Bus-Level Load Forecasting – CENACE (Bajío Region)
📊 Time-Series Forecasting of Hourly Electricity Demand in Mexico

This project presents a bus-level load forecasting model using open data from CENACE, focused on the Bajío region of Mexico. It was developed as a practical exercise to demonstrate applied time-series analysis, forecasting techniques, and energy analytics.

🧠 Project Overview

Electricity demand forecasting is essential for grid reliability, energy trading, and operational planning.
This project applies SARIMA modeling to predict hourly electricity load (MW) for the Bajío region, capturing daily and weekly seasonal patterns.

The workflow follows a typical data science lifecycle:
Data Collection: Hourly load data from CENACE (public dataset).
Exploratory Data Analysis (EDA): Time-series visualization and basic descriptive statistics.
Feature Preparation: Handling timestamps and missing values.
Modeling: SARIMA model optimized for daily seasonality.
Evaluation: Quantitative and visual comparison between actual and predicted load.

🧾 Data Source

Source: CENACE México – Sistema de Información del Mercado (SIM)
Region: Bajío
Frequency: Hourly
Variables: Timestamp (FechaHora), Real Load (DemandaReal)
Period: Selected date range (user-defined, typically 1–3 months)

🧰 Tech Stack
Programming Language:	Python
Data Analysis:	Pandas, NumPy
Visualization:	Matplotlib, Seaborn
Modeling:	Statsmodels (SARIMAX)
Evaluation Metrics:	MAE, RMSE, MAPE
Environment	Jupyter Notebook

📈 Modeling Approach
The SARIMA (Seasonal ARIMA) model was selected for its ability to handle temporal dependencies and recurring daily seasonality.

🔍 Results Summary
Metric	Value	Description
MAE	~120 MW	Average absolute deviation
RMSE	~180 MW	Root mean square deviation
MAPE	~3.5%	Relative error rate



Key Insights:
The model successfully captures daily demand cycles and weekday/weekend effects.
Forecast accuracy improves with longer training windows and weather feature inclusion.
The workflow can easily scale to bus-level or node-level data when available.

⚙️ How to Run
Clone the repository or download the notebook.
Install required libraries:
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn
Download your regional demand dataset from CENACE
Update the file path in the notebook:
df = pd.read_csv("DemandaRegional_BAJIO.csv")
Run the notebook to visualize, model, and evaluate results.

💬 About the Author
César López
Data Scientist | Industrial Engineer
Specialized in process optimization, predictive analytics, and applied machine learning.
Experience in manufacturing, energy analytics, and data-driven decision making.

📍 León, Guanajuato, México
🔗 LinkedIn
 | GitHub
