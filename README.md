### Business Problem 
The objective of this project is to identify revenue drivers, understand customer purchasing behavior, segment customers based on their value and engagement, and identify opportunities to improve customer retention and sales performance.

### Tools
SQL | Python | Pandas | Power BI

### Key Findings

High Churn Rate After the First Month: The average M1 retention rate stands at 34.8%, indicating that a significant portion of customers make only a single purchase and do not return in subsequent months.
Stabilization of the Retention Curve: Following a sharp drop between month 1 and month 2, the multi-cohort trend curves flatten out from month 2 onward, showing that the remaining core customer base demonstrates long-term loyalty.
Cohort and Temporal Variations: Analyzing monthly cohorts reveals that different customer groups (tracked via the CohortMonth filters) exhibit varying drop-off velocities, with certain seasonal cohorts showing distinct spikes in engagement.
Geographical Segmentation: Filtering via the Country slicer clearly highlights primary markets driving the highest volume of repeat purchases, compared to regions where acquisition is high but repeat engagement is weaker.
 
 ### Repository Structure
 ```text
├── Data
| ├── online_retail.csv                   # Source dataset, downloaded from: https://www.kaggle.com/datasets/thedevastator/online-retail-transaction-data/code
| ├── clean_cata.csv                      # Clean source dataset 
| ├── cleaned_retail_data.csv             # Clean source dataset used in Power BI
| ├── rfm_segmentation.csv                # Dataset about customers with scores and segments used in Power BI
| ├── cohort_retention.csv                # Dataset calculated % retention by months used in Power BI
├── Python
| ├── 01_cleaning.ipynb                                # Data preprocessing and cleaning script
| ├── 02_eda.ipynb                                     # Exploratory Data Analysis notebook
| ├── sql_sales_analyst_customer_segmentation.ipynb    # SQL querying & RFM logic
| ├── SQLite database
| ├── customer_analysis.db                           # SQLite database instance
├── PowerBI
| ├── Customer_Cohort_Analysis_Dashboard.pbix        # Power bi dashboard
└── README.md                           # Project documentation

