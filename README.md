# **Customer Segmentation Using Rossmann Sales Data**

This project leverages the Rossmann Store Sales dataset to predict and
analyze customer segmentation. The dataset provides insights into
various store attributes, customer behavior, and sales data over a
specific time frame. Below is a detailed guide to understanding the
dataset and the methodology used for analysis.

## **Dataset Overview**

The project utilizes two primary datasets:

1.  **Sales Data (train.csv)**

    -   **Records**: \~1 million observations.

    -   **Columns**:

        -   Id: Transaction ID (combination of Store and Date).

        -   Store: Unique Store ID.

        -   Sales: Sales per day (Target variable).

        -   Customers: Number of customers on a given day.

        -   Open: Boolean indicating whether the store is open (1) or
            > closed (0).

        -   Promo: Indicates if a store is running a promo on that day
            > (1 = Yes, 0 = No).

        -   StateHoliday: Categorical variable denoting the type of
            > state holiday (a, b, c, 0 = None).

        -   SchoolHoliday: Indicates if public school closures affected
            > the store on that day (1 = Yes, 0 = No).

2.  **Store Information Data (store.csv)**

    -   **Records**: 1,115 unique stores.

    -   **Columns**:

        -   Store: Store ID.

        -   StoreType: Type of store (a, b, c, d).

        -   Assortment: Assortment type (a, b, c).

        -   CompetitionDistance: Distance to the nearest competitor in
            > meters.

        -   CompetitionOpenSinceMonth: Month when competition was
            > opened.

        -   CompetitionOpenSinceYear: Year when competition was opened.

        -   Promo2: Whether the store is running Promo2 (1 = Yes, 0 =
            > No).

        -   Promo2SinceWeek: Week when Promo2 started.

        -   Promo2SinceYear: Year when Promo2 started.

        -   PromoInterval: Months in which Promo2 is active.

## **Methodology**

### **1. Data Exploration**

-   **Key Statistics**:

    -   Average daily sales: \~5,773 Euros.

    -   Average customers per day: \~633.

    -   Stores open \~80% of the time.

    -   Promo campaigns active \~40% of the time.

-   **Insights**:

    -   Sales and customer distribution are approximately uniform across
        > weekdays.

    -   School holidays occur \~18% of the time.

### **2. Data Visualization**

-   **Missing Data**:

    -   Visualized using heatmaps to ensure data quality.

-   **Histograms**:

    -   Analyzed distributions for sales, customers, promotions, and
        > holidays.

### **3. Clustering Techniques**

-   **K-Means Clustering**: To group stores based on customer behavior
    > and sales.

-   **Principal Component Analysis (PCA)**: Reduced dimensionality for
    > visualizing clusters.

-   **Auto-Encoders**: Used neural networks for compact data
    > representation and improved clustering performance.

## **How to Run the Project**

### **Prerequisites**

-   Install the following Python libraries:

    -   pandas

    -   numpy

    -   matplotlib

    -   seaborn

### **Steps**

1.  Clone the repository:\
    > git clone \<repository_url\>

2.  Navigate to the project directory:\
    > cd \<project_directory\>

3.  Run the notebook or Python scripts for analysis.\
    > python analysis_script.py

## **Results**

1.  **Customer Segmentation**:

    -   Identified distinct customer groups with similar attributes.

    -   Enhanced understanding of customer behavior across stores.

2.  **Dimensionality Reduction**:

    -   Simplified datasets for better visualization and clustering.

3.  **Advanced Insights**:

    -   Auto-encoders revealed deeper patterns in customer data.

## **Contribution**

We welcome contributions! Feel free to submit issues or create pull
requests to enhance the project.

## **License**

This project is licensed under the MIT License. See LICENSE for details.

## **Acknowledgments**

-   Dataset sourced from the [[Rossmann Store Sales
    > Competition]{.underline}](https://www.kaggle.com/c/rossmann-store-sales/data)
    > on Kaggle.
