RetailPulse: AI-Powered Customer Analytics \& Demand Forecasting Platform



\---



\##  About The Project



\*\*RetailPulse\*\* is an enterprise-grade, AI-driven retail analytics and demand forecasting platform. Built during the Data Science \& Analytics Internship at \*\*Zidio Development\*\*, this project addresses critical retail supply chain challenges—specifically stockouts, overstock holding costs, customer churn risks, and unpredictable buying behavior. 



The platform seamlessly bridges raw multi-source transactional data with robust predictive modeling, MLOps tracking, and interactive business intelligence reporting.



\---



\##  Key Features \& Modules



1\. \*\* Customer Segmentation (RFM + K-Means):\*\*

&#x20;  \* Computes Recency, Frequency, and Monetary (RFM) behavioral metrics for 500+ unique buyers.

&#x20;  \* Employs K-Means clustering (validated via the Elbow Method) to group customers into distinct tiers (e.g., High-Value Frequent Buyers, Active Shoppers, At-Risk Re-engagement Targets).



2\. \*\* Advanced Demand Forecasting:\*\*

&#x20;  \* Analyzes historical daily sales data across 50 SKUs spanning a 2-year horizon (2024–2025).

&#x20;  \* Implements baseline, seasonal, and \*\*Random Forest Regressors\*\* incorporating rolling averages and calendar indicators to deliver reliable 30-day ahead sales projections.



3\. \*\* Churn Prediction \& Risk Mitigation:\*\*

&#x20;  \* Utilizes classification models (Logistic Regression \& XGBoost) to predict customer inactivity risks.

&#x20;  \* Integrates \*\*SHAP (SHapley Additive exPlanations)\*\* to ensure complete model interpretability and feature transparency.



4\. \*\* Inventory Optimization:\*\*

&#x20;  \* Dynamically translates forecasted demand and lead times into safety stock thresholds and reorder points.

&#x20;  \* Minimizes overstock holding costs while preventing stockouts across enterprise inventory snapshots (`inventory\_clean.csv`).



\---



\##  System Architecture

RetailPulse operates across four core structured layers:

\* \*\*Ingestion \& Storage Layer:\*\* Multi-source ingestion and validation of daily sales, inventory snapshots, and calendar logs using Python (`Pandas`/`NumPy`).

\* \*\*Analytics \& ML Layer:\*\* Customer clustering, time-series regression, and classification pipelines.

\* \*\*MLflow MLOps Layer:\*\* Hyperparameter logging, model version tracking, and experiment monitoring.

\* \*\*Power BI BI Layer (`RetailPulse.pbix`):\*\* Centralized reporting interface for DAX-calculated KPIs and visual dashboards.



\---



\##  Tech Stack



| Category | Technologies / Tools |

| :--- | :--- |

| \*\*Language\*\* | Python (v3.12) |

| \*\*Data Manipulation \& ML\*\* | Pandas, NumPy, Scikit-learn, XGBoost |

| \*\*Forecasting \& Modeling\*\* | Random Forest Regressors, Time-Series Analysis |

| \*\*Model Explainability\*\* | SHAP (SHapley Additive exPlanations) |

| \*\*MLOps \& Tracking\*\* | MLflow |

| \*\*Business Intelligence\*\* | Power BI (`RetailPulse.pbix`) |

| \*\*Version Control\*\* | Git \& GitHub |



\---



\##  Project Directory Structure



```text

RetailPulse/

│

├── dashboards/               # Power BI report file (RetailPulse.pbix)

├── data/

│   ├── raw/                 # Raw datasets (sales\_daily.csv, inventory\_snapshots.csv, calendar.csv)

│   └── processed/           # Cleaned \& integrated files (sales\_clean.csv, inventory\_clean.csv, and more.)

│

├── notebooks/               # Step-by-step Jupyter Notebook pipeline

│   ├── 01\_data\_exploration.ipynb

│   ├── 02\_data\_cleaning.ipynb

│   ├── 03\_demand\_forecasting.ipynb

│   ├── 04\_inventory\_analysis.ipynb

│   ├── 05\_customer\_segmentation.ipynb

│   └── 06\_churn\_prediction.ipynb

├──reports/

│     ├── Project\_reports.pdf

│

└── README.md                # Project Documentation

└── requarment.txt            # dependencies





Execution Workflow (Notebooks)

To reproduce or explore the analysis, execute the Jupyter notebooks in chronological order:



01\_data\_exploration.ipynb: Validates initial data structures and data quality.



02\_data\_cleaning.ipynb: Handles missing values, standardizes date formats, and merges datasets.



03\_demand\_forecasting.ipynb: Evaluates sales trends and executes regression models.



04\_inventory\_analysis.ipynb: Computes inventory risk tiers and reorder recommendations.



05\_customer\_segmentation.ipynb: Generates RFM features and implements K-Means clustering.



06\_churn\_prediction.ipynb: Runs classification models and computes SHAP explanations.





Business Intelligence \& Dashboard



The enterprise reporting layer (RetailPulse.pbix) connects directly to the processed data warehouse schema. It provides stakeholders with:



Real-time revenue tracking and seasonal performance monitoring.



Interactive filters for customer clusters and regional metrics.



Automated inventory stock-gap alarms and reorder quantities.



&#x20;Author \& Project Details

Developer: Priyanka Dipak Jogi



Company: Zidio Development



Domain: Data Science \& Analytics Domain Internship



Duration: 20 September 2026 – 20 October 2026

