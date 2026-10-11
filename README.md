# Swiggy-Analaysis-Project
# Swiggy Raw Data Excel Dashboard

## Overview

This project is an Excel-based dashboard built using Swiggy
food-ordering data. It explores restaurant and dish-level information to
summarize pricing, ratings, customer-facing categories, and ordering
patterns across locations and dates.

The workbook contains raw data, an analysis sheet with key performance
indicators (KPIs), and a dashboard sheet.

## Workbook Structure

  -----------------------------------------------------------------------
  Sheet                               Description
  ----------------------------------- -----------------------------------
  `Swiggy Data`                       Raw dataset containing location,
                                      order date, restaurant, dish, food
                                      category, price, rating, and
                                      rating-count fields.

  `Analysis`                          KPI calculations and supporting
                                      analysis used for the dashboard.

  `Dashboard`                         Dashboard presentation sheet.
  -----------------------------------------------------------------------

## Dataset Details

The raw data sheet contains approximately **197,430 records** and the
following fields:

-   **State** --- State associated with the restaurant/order
-   **City** --- City
-   **Order Date** --- Date associated with the record
-   **Day** --- Day of the week derived from the order date
-   **Quarter** --- Calendar quarter derived from the order date
-   **Week** --- Week number
-   **Restaurant Name** --- Restaurant name
-   **Location** --- Locality or area
-   **Category** --- Food/menu category
-   **Dish Name** --- Dish or menu-item name
-   **Food Type** --- Food-type classification
-   **Price (INR)** --- Price in Indian rupees
-   **Rating** --- Rating value
-   **Rating Count** --- Number of ratings

## Key Performance Indicators

The Analysis sheet includes these summary metrics:

-   **Total Price (INR):** Sum of the `Price (INR)` field.
-   **Average Rating:** Average of the `Rating` field.
-   **Total Rating Count:** Sum of `Rating Count`.
-   **Dish Record Count:** Count of dish-name records.
-   **AOV:** A calculated metric in the workbook, currently defined as
    total price divided by dish-record count. This should be interpreted
    according to the dataset's grain; it is not necessarily a true
    order-level average order value.

The workbook's current KPI calculations show a total price sum of
approximately **₹5.30 crore**, an average rating of **4.34**, a total
rating count of approximately **55.92 lakh**, and **197,430** dish
records. These figures reflect the current workbook and may change if
the source data or filters are updated.

## Tools Used

-   Microsoft Excel
-   Excel formulas
-   KPI calculations and dashboard-style reporting

## How to Use

1.  Download or clone this repository.
2.  Open `Swiggy Raw Data Excel Dashboard.xlsx` in Microsoft Excel.
3.  Review the `Swiggy Data` sheet to understand the source fields.
4.  Open the `Analysis` sheet to inspect KPI calculations.
5.  Open the `Dashboard` sheet to view the dashboard.
6.  If you update or replace source data, verify formulas, pivot tables,
    charts, and KPI totals before sharing results.

> Note: Excel features such as formulas, pivot tables, slicers, or
> charts may behave differently in other spreadsheet applications. Open
> the workbook in Excel for the most reliable experience.

## Project Goals

-   Summarize Swiggy menu-item data across cities and locations.
-   Understand price and rating patterns.
-   Compare food categories, restaurants, and dishes.
-   Present raw data in a more accessible reporting format.

## Repository Contents

``` text
.
├── README.md
└── Swiggy Raw Data Excel Dashboard.xlsx
```

## Future Improvements

-   Add interactive filters for city, restaurant, category, and date.
-   Include visual comparisons for ratings and prices.
-   Add a documented data-cleaning and refresh process.
-   Validate whether AOV should be calculated from order-level data
    rather than dish-level records.

## Disclaimer

This project is for learning, portfolio, and analytical demonstration
purposes. KPI values describe the workbook's current calculations and
should be validated before being used for business decisions.
