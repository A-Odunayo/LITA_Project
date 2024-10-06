# LITA_Project

### Project Topic
**Data Analysis Training Project** - *Analysis of International Breweries Sales Record from 2017-2019*

-----------------------

### Project Overview
This is to analyze International Breweries Sales from 2017 till 2019, determining the some Sales Parametersputting into use some of the things learnt during my data analysis class with **'Incubator Hub'**   [Check them out](https://theincubatorng.org/)

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

With the use of Pivot table in excel, our large dataset was summarised and the table below was extracted for visualization

**Quantity Sold Per Brand Per Country from 2017-2019**					

|     |Beta Malt|Budweiser|Castle Light|Eagle Lager|Grand Malt| Hero |Trophy|
|-----|---------|---------|------------|-----------|----------| ---- |------|
|**Benin**|23902|25156|25639|24876|24967|26126|25658|176324|
|**Ghana**|25408|24419|25806|25829|25615|25654|25524|178255|
|**Nigeria**|25381|26153|25681|25872|24666|25811|25743|179307|
|**Senegal**|25625|25923|25974|25771|25428|26632|25575|180928|
|**Togo**|24747|24623|25074|25455|25613|24837|25559|175908|
|**Grand Total**|**125063**|**126274**|**128174**|**127803**|**126289**|**129060**|**128059**|


**Quantity Sold Per Brand Per Sales Representatives**		

|     |Beta Malt|Budweiser|Castle Light|Eagle Lager|Grand Malt| Hero |Trophy|
|-----|---------|---------|------------|-----------|----------| ---- |------|
|Andrews|	13197|	14310|	11180|	12313|	13294|	12888|	12716|	
|Gill| 14612|	14570|	15565|	15279|	13677|	13544|	14042	|
|Howard|	6078|	5899|	5877|	4879|	6733|	7088|	5033	|
|Jardine|	14656|	14572|	18009|	15118|	17146|	17508|	17734	|
|Jones|	23388|	22933|	22417|	22655|	21108|	22046|	23333|	
|Kivell|	8185|	7704|	8317|	8721|	7408|	8279|	9641	|
|Morgan|	9240|	9275|	9610|	11123|	9224|	9046|	10045|	
|Parent|	9148|	7601|	8687|	7916|	8913|	8823|	8148|	
|Smith|	7340|	8258|	8769|	7716|	8381|	8824|	9658	|
|Sorvino|	12525|	13350|	12591|	14702|	13247|	14221|	10877	|
|Thompson|	6694|	7802|	7152|	7381|	7158|	6793|	6832	
|**Grand Total**|**125063**|**126274**|**128174**|**127803**|**126289**|**129060**|**128059**|


### Data Visualization





