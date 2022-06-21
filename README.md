**Demand Forecasting :-**
_You are working as a data scientist in a CPG firm. The company holds warehouses in various cities across the country. Different items are sent to these warehouses on a weekly basis and from where they are distributed to various small stores on a daily basis._

_To increase the efficiency of this process, the management has decided to build software that can forecast weekly and daily demand in advance._

**Task :-** You are given a relevant dataset about the demand for products in the warehouses. You are required to build a machine learning model that can forecast weekly as well as daily demand. 

* **Notes:-** 
 * Your model will be evaluated on the basis of predicted weekly_dispatch_count, However, you are also required to analyze and forecast the daily_dispatch_count for the test data. 
 * You must create an ipython notebook containing your analysis and approach for the given task and upload it by clicking the Upload Source Code button. 

* _Dataset description The dataset folder contains the following files:_
   * train.csv. 16644 x 12 
   * test.csv: 4900 x 10 
   * submission_weekly.csv: 700 x 2 

**The columns provided in the dataset are as follows:**

|Column name |Description|
|:----------:|:-----------|
|ID |Represents the unique identification of each entry| 
|date |Represents the date in "yyyy-mm-dd" format| 
|warehouse_ID|Represents the unique identification of a warehouse|
|Latitude |Represents the latitude of the warehouse| 
|Longitude |Represents the longitude of the warehouse| 
|Product Type |Represents the type of a product ( Type_A or Type_B)|
|year |Represents the current year| 
|month |Represents the current month of the year| 
|is_weekend |Represents whether the day is weekend or not| 
|is_warehouse_closed |Represents whether the warehouse is closed or not|
|daily_dispatch_count |Represents the number of items of a specific product type that are dispatched (in thousands) from a specific warehouse on a specific day| 
|weekly_dispatch_count |Represents the number of items of a specific product type that are dispatched (in thousands) from a specific warehouse in the corresponding week, **Note:** The weekly_dispatch_count is calculated on Sundays.|
