# 🏡 Airbnb Rent Price Analysis (Excel-Based EDA)

---

## Project Description

This project focuses on **Exploratory Data Analysis (EDA)** of Airbnb rental data using **Microsoft Excel**.
The analysis includes **data cleaning, preprocessing, data understanding, univariate analysis with 5-point summary**, and **solving multiple business questions** to identify factors affecting Airbnb rental prices.

---

## Business Context

Airbnb is an online platform that allows people to rent short-term accommodation.
This ranges from regular people with a spare bedroom to property management firms who lease multiple rentals.

On one side, Airbnb enables owners to list their space and earn rental income.
On the other side, it provides travelers easy access to renting private homes.

Airbnb receives commissions from two sources upon every booking:

* Airbnb charges the guest **6–12%** of the booking fee
* Airbnb charges the host **3%** for every successful transaction

Airbnb is losing its commissions due to:

* **Under-pricing properties when demand is high**
* **Over-pricing properties when competitiveness is required**

Airbnb wants to **optimize its revenue and commissions** by optimizing property prices.

---

## Objective

As a Data Analyst at Airbnb, the objective is to perform **Exploratory Data Analysis** to understand the factors affecting accommodation prices in order to **maximize revenue**.

---

## Data Description

The dataset contains information about different types of rental rooms offered by Airbnb over a fixed period of time.

---

## Data Dictionary

* **id**: Property ID
* **room_type**: Type of room in the property
* **no_of_accommodates**: Number of adults the property can accommodate
* **no_of_bathrooms**: Number of bathrooms in the property
* **cancellation_policy**: Cancellation policy of the property
* **cleaning_fee**: Indicates whether the cleaning fee is included in rent
* **instant_bookable**: Indicates whether instant booking is available
* **review_scores_rating**: Review rating score of the property
* **no_of_bedrooms**: Number of bedrooms
* **no_of_beds**: Total number of beds
* **log_price**: Log of rental price (USD)

  * Example: If price = 12000 USD, then `log_price = log(12000)`

---

## Data Understanding & Cleaning

### Data Understanding

* Explored each column, its data type, and values
* Checked total number of records
* Checked for duplicate records
* Identified missing values and explained treatment methods

### Data Cleaning

* Missing values treatment:

  * Categorical variables → **Mode**
  * Continuous variables → **Mean / Median**
* Converted `log_price` to actual price using **EXP function**
* converted Bollean value to `Yes/No`

---

## Why Are Bathrooms in Decimals?

In the United States, bathrooms are categorized as:

* **Full bath**: Toilet, sink, shower/bathtub
* **Half bath (0.5)**: Toilet and sink
* **3/4 bath**: Toilet, sink, and shower

Decimal notation exists because:

* 2.5 bathrooms = 2 full + 1 half bath
* 3.2 bathrooms = 3 full + 2 half baths

This results in decimal bathroom values in real estate listings.

---

## Questions to Identify Factors and Insights

### Room Features

* Question 1.1: Do private rooms cost more than shared rooms?
* Question 1.2: Does the number of accommodates affect the price?
* Question 1.3: Does the number of bathrooms affect the price?
* Question 1.4: Does the number of bedrooms affect the price?
* Question 1.5: Does the number of beds affect the price?

### App Features

* Question 2.1: Do flexible cancellation rooms cost more than strict ones?
* Question 2.2: Does instant booking cost more than prior booking?
* Question 2.3: Do rooms with cleaning fees included cost more?
* Question 2.4: Do higher-rated rooms cost more?

### Additional Questions

* Question 3.1: Do shared rooms mostly have flexible cancellation?
* Question 3.2: Are private rooms significantly more expensive?
* Question 3.3: Is there a relationship between accommodates and price?
* Question 3.4: Are accommodates and cancellation policy correlated?
* Question 3.5: Are instantly bookable rooms mostly flexible?
* Question 3.6: Does shared room price increase with accommodates?

---

## Key Findings & Insights (Summary)

* Private rooms are priced higher than shared rooms
* Room size features do not show a strong linear relationship with price
* Strict cancellation policies are more expensive
* Cleaning fee inclusion increases average price
* Higher-rated rooms generally cost more
* Most customers prefer rooms with **1–4 accommodates**
* Shared rooms are the least preferred and lowest priced option

---

## Tools Used

* Microsoft Excel

  * Data Cleaning
  * Pivot Tables
  * Descriptive Statistics
  * Dashboard creation
  * Exploratory Data Analysis

---

## Conclusion

This project demonstrates a complete **Excel-based Exploratory Data Analysis workflow**, starting from raw data understanding to business-driven insights.
The analysis helps Airbnb understand pricing behavior and supports better **price optimization strategies** to maximize revenue.

---

## Author

### Ramakrushna Nayak

#### Aspiring Data Analyst

#### Excel | SQL | Power BI | Data Analysis
