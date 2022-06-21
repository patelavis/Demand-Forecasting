{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "8c506923",
   "metadata": {},
   "source": [
    "# Demand Forecasting"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "69eb78e4",
   "metadata": {},
   "source": [
    "**Demand Forecasting :-**\n",
    "_You are working as a data scientist in a CPG firm. The company holds warehouses in various cities across the country. Different items are sent to these warehouses on a weekly basis and from where they are distributed to various small stores on a daily basis._\n",
    "\n",
    "_To increase the efficiency of this process, the management has decided to build software that can forecast weekly and daily demand in advance._"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "f6843e8a",
   "metadata": {},
   "source": [
    "**Task :-** You are given a relevant dataset about the demand for products in the warehouses. You are required to build a machine learning model that can forecast weekly as well as daily demand. \n",
    "\n",
    "* **Notes:-** \n",
    " * Your model will be evaluated on the basis of predicted weekly_dispatch_count, However, you are also required to analyze and forecast the daily_dispatch_count for the test data. \n",
    " * You must create an ipython notebook containing your analysis and approach for the given task and upload it by clicking the Upload Source Code button. \n",
    "\n",
    "* _Dataset description The dataset folder contains the following files:_\n",
    "   * train.csv. 16644 x 12 \n",
    "   * test.csv: 4900 x 10 \n",
    "   * submission_weekly.csv: 700 x 2 "
   ]
  },
  {
   "cell_type": "markdown",
   "id": "f443ec0c",
   "metadata": {},
   "source": [
    "**The columns provided in the dataset are as follows:**\n",
    "\n",
    "|Column name |Description|\n",
    "|:----------:|:-----------|\n",
    "|ID |Represents the unique identification of each entry| \n",
    "|date |Represents the date in \"yyyy-mm-dd\" format| \n",
    "|warehouse_ID|Represents the unique identification of a warehouse|\n",
    "|Latitude |Represents the latitude of the warehouse| \n",
    "|Longitude |Represents the longitude of the warehouse| \n",
    "|Product Type |Represents the type of a product ( Type_A or Type_B)|\n",
    "|year |Represents the current year| \n",
    "|month |Represents the current month of the year| \n",
    "|is_weekend |Represents whether the day is weekend or not| \n",
    "|is_warehouse_closed |Represents whether the warehouse is closed or not|\n",
    "|daily_dispatch_count |Represents the number of items of a specific product type that are dispatched (in thousands) from a specific warehouse on a specific day| \n",
    "|weekly_dispatch_count |Represents the number of items of a specific product type that are dispatched (in thousands) from a specific warehouse in the corresponding week, **Note:** The weekly_dispatch_count is calculated on Sundays.|"
   ]
  },
  {
   "cell_type": "markdown",
   "id": "d462cb4b",
   "metadata": {},
   "source": [
    "**Evaluation metric :-** \n",
    "_**The evaluation metric for this challenge will be mean_absolute_percentage_error.**_  \n",
    "`score = max( 0 , 100*(1 metrics.mean_absolute_percentage_error (actual ,predicted)))`"
   ]
  }
