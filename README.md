# LITA_Project

### Project Topic
**Data Analysis Training Project** - *Analysis of International Breweries Sales Record from 2017-2019*

-----------------------

### Project Overview
This is to analyze International Breweries Sales from 2017 till 2019, determining the Sales
- Per Year
- Per Brand
- 
putting into use some of the things learnt during my data analysis class with **'Incubator Hub'**   [Check them out](https://theincubatorng.org/)

 ------------------------
### Table of Content
- [Data source](#Data-source)

- [Tools Used](#Tools-Used)

- [Data Extraction, Transformation, and Loading](#Data-Extraction-Transformation-and-Loading)

- [Data Analysis](#Data-Analysis)

- [Data Visualization](#Data-Visualization)

-------------------------------------------------------------

### Data Source
This data set is an open data made availabilty by my trainer during the cause of the training.

-----------------------------------------------------------------

### Tools Used
The following tools where used

- **SQL** (Structed Query Language) for:

    1. Data Storage
    2. Data Querying and Manipulation

[Download SQL](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)

 - **Microsoft Excel** for:

    1. Data Analysis
    2. Data Visualization

[Download Microsoft Excel](https://microsoft-excel-2016.en.download.it/#google_vignette)

------------------------

### Data Extraction, Transformation, and Loading
- **Data Extraction**
Our data was extracted from **SSMS (SQL Server Management Studio)** using the query below:

Input:
```SQL 
Select * from [dbo].[InternationalBreweries]
```

Output:

![Image](https://github.com/A-Odunayo/LITA_Project/blob/main/International%20Brewery%20Data%20Output.PNG)

afterwhich, the needed field was created to **View** using the query below:

Input:
```SQL 
Create View VW_International_Breweries
as
Select SALES_ID, SALES_REP, BRANDS, QUANTITY, COUNTRIES, REGION, MONTHS, YEARS
from [dbo].[InternationalBreweries]
```

```SQL
Select * from [dbo].[VW_International_Breweries]
```

Output:

![image](https://github.com/user-attachments/assets/746da6e6-d8c9-4f2d-a491-0afa1ae3ebb2)

> [!Note]
> **View** was created in order to conceal confidential fields

- **Data Transformation**

The data require no tranformation as it was already structured

- **Data Loading**

The view data was loaded on excel for **Analysis** and **Visualization**

### Data Analysis



### Data Visualization





