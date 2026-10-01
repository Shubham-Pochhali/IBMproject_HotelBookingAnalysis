# Hotel Booking Analysis

## 📌 Project Overview

**Hotel Booking Analysis** is a data analysis and visualization project
focused on understanding hotel reservation patterns and identifying
factors associated with booking cancellations.

The project analyzes historical booking data for **City Hotel** and
**Resort Hotel** to explore cancellation behavior, average daily rates
(ADR), monthly reservation trends, country-wise cancellations, and other
booking characteristics.

The primary business objective is to provide data-driven insights that
can help hotels understand cancellation patterns and improve
revenue-management and promotional strategies.

------------------------------------------------------------------------

## 🎯 Business Problem

City Hotel and Resort Hotel have experienced a significant number of
booking cancellations. Cancellations can result in vacant rooms, reduced
occupancy, and potential revenue loss.

This project investigates the available booking data to answer questions
such as:

-   What factors are associated with hotel reservation cancellations?
-   How do cancellation patterns differ between City Hotel and Resort
    Hotel?
-   How does Average Daily Rate (ADR) relate to cancellation behavior?
-   Which months show higher reservation and cancellation activity?
-   Which countries account for a larger share of canceled reservations?
-   How can the analysis support pricing and promotional decisions?

------------------------------------------------------------------------

## 📊 Dataset

The analysis uses a hotel booking dataset containing **119,390 records
and 32 columns**.

### Dataset

**[View / Download the project
dataset](./hotel_bookings%202%281%29.csv)**

The dataset contains information such as:

-   Hotel type
-   Cancellation status
-   Lead time
-   Arrival date
-   Length of stay
-   Number of guests
-   Meal type
-   Country
-   Market segment
-   Distribution channel
-   Previous cancellations and bookings
-   Reserved and assigned room types
-   Deposit type
-   Waiting-list days
-   Customer type
-   Average Daily Rate (ADR)
-   Special requests
-   Reservation status
-   Reservation status date

------------------------------------------------------------------------

## 🔎 Key Analysis Areas

### 1. Reservation Cancellation Analysis

The project calculates the proportion of canceled and non-canceled
reservations and visualizes the overall reservation status distribution.

### 2. City Hotel vs Resort Hotel

Reservation status is compared across the two hotel categories to
identify differences in booking volume and cancellation behavior.

### 3. Average Daily Rate (ADR)

ADR is analyzed over time for both hotel types and is also compared
between canceled and non-canceled reservations.

### 4. Monthly Reservation Trends

Monthly reservation activity is examined to identify periods with
relatively high or low reservation and cancellation counts.

### 5. Country-wise Cancellation Analysis

The countries associated with canceled reservations are analyzed,
including a visualization of the top 10 countries by cancellation count.

### 6. Market Segment Analysis

Market segments are examined to understand their distribution across the
overall dataset and among canceled reservations.

------------------------------------------------------------------------

## 🧹 Data Preparation

The notebook performs the following preparation steps:

1.  Loads the CSV dataset using **Pandas**.
2.  Converts `reservation_status_date` into a datetime format.
3.  Checks the dataset structure, columns, descriptive statistics,
    unique categorical values, and missing values.
4.  Removes rows containing missing values.
5.  Uses a box plot to inspect the `adr` distribution.
6.  Removes records where `adr >= 5000` to reduce the effect of extreme
    ADR values.
7.  Creates a `month` column from `reservation_status_date` for monthly
    analysis.

> **Note:** The cleaning steps are based on the project notebook and are
> intended specifically for this analysis.

------------------------------------------------------------------------

## 📈 Visualizations

The project includes visualizations such as:

-   Reservation Status Count
-   Hotel Reservation Status
-   Average Daily Rate in City and Resort Hotels
-   Reservations per Month
-   ADR per Month
-   Top 10 Countries with Canceled Reservations
-   Average Daily Rate for Canceled vs Non-Canceled Reservations

These visualizations are used to make booking and cancellation patterns
easier to interpret.

------------------------------------------------------------------------

## 💡 Project Findings

The project report highlights several observations from the analysis:

-   A substantial proportion of reservations in the analyzed data were
    canceled.
-   City Hotel has a higher overall number of bookings than Resort
    Hotel.
-   ADR varies over time and between City Hotel and Resort Hotel.
-   Reservation activity differs across months, with August showing high
    reservation activity in the report.
-   Portugal appears as the leading country among the countries shown in
    the cancellation analysis.
-   The analysis observes a relationship between higher ADR and
    cancellation behavior.

The report uses these observations to discuss possible pricing,
discounting, promotional, and service-related strategies for reducing
cancellations and improving hotel revenue.

------------------------------------------------------------------------

## 🛠️ Technologies Used

  Technology             Purpose
  ---------------------- ------------------------------------------------------
  **Python**             Data analysis and processing
  **Pandas**             Data loading, cleaning, transformation, and analysis
  **Matplotlib**         Data visualization
  **Seaborn**            Statistical and categorical visualizations
  **Jupyter Notebook**   Interactive analysis environment

------------------------------------------------------------------------

## 📁 Project Structure

``` text
Hotel-Booking-Analysis/
│
├── hotel_bookings 2(1).csv
├── ShubhamPochhali_HotelBookingAnalysis.ipynb
├── requirements.txt
└── README.md
```

> File names may vary depending on how the project is organized in your
> local machine or GitHub repository.

------------------------------------------------------------------------

## ⚙️ Installation & Setup

### 1. Clone the repository

``` bash
git clone <YOUR-GITHUB-REPOSITORY-URL>
cd Hotel-Booking-Analysis
```

### 2. Create a virtual environment

``` bash
python -m venv venv
```

Activate it on Windows:

``` bash
venv\Scripts\activate
```

Activate it on macOS/Linux:

``` bash
source venv/bin/activate
```

### 3. Install dependencies

``` bash
pip install -r requirements.txt
```

The required Python libraries are:

``` text
pandas
matplotlib
seaborn
```

### 4. Launch Jupyter Notebook

``` bash
jupyter notebook
```

Open:

``` text
ShubhamPochhali_HotelBookingAnalysis.ipynb
```

### 5. Run the analysis

Make sure the dataset is located in the same directory as the notebook,
then execute the notebook cells sequentially.

------------------------------------------------------------------------

## 📋 Requirements

-   Python 3.9+
-   Jupyter Notebook / JupyterLab
-   Pandas
-   Matplotlib
-   Seaborn

------------------------------------------------------------------------

## 📌 Key Information

**Project Type:** Exploratory Data Analysis (EDA)\
**Domain:** Hospitality / Hotel Booking\
**Dataset Size:** 119,390 rows × 32 columns\
**Primary Focus:** Booking cancellations and hotel reservation patterns\
**Hotels Covered:** City Hotel and Resort Hotel\
**Analysis Period:** Historical booking data covering 2015--2017\
**Programming Language:** Python

------------------------------------------------------------------------

## 📚 Project Report

A detailed project report accompanies this analysis and documents the
business problem, assumptions, research questions, analysis,
visualizations, findings, and recommendations.

------------------------------------------------------------------------

## 👤 Author

**Shubham Pochhali**

B.Tech Computer Science & Engineering

------------------------------------------------------------------------

## 📄 License

This project is intended for educational, analytical, and portfolio
purposes. Please verify the original dataset's licensing and attribution
requirements before redistributing the dataset itself.
