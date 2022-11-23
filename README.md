
# Business Insight

 A Guided Project by code Basics. The Project revolves around a 
 fictitous company called AtliQ hardware. it is a consumer goods electronics company having operations in various countries. Their business is growing rapidly and they still rely on excel files for data analytics. Excel files are hard to consume and not effective in generating insights. Also due to the lack of effective analytics the company faced a major loss in Latin America.

Senior executives of this company have decided to invest in a data analytics project and have assigned a team for this work.


## requirements

product owner required from the data analytics team 5 different dashboards in powerBI.

The  Dashboard  is designed to meet stakeholders requirements,adding along with that relevant insights that are not provided by the stakeholders.

Each sector depends on certain KPI's in order to  identify their gap and forte.My role as data analyst is to gather,clean and interpret the data provided. My job is to transform this data into a story that can be easily understood by my stakeholders while providing key insights that would help solve business problems.

## Data journey

Here is listed some of the important steps in each process

**Data transformation** (Power Query)

1. Generate a table containing both our actual and estimate stakeholders( by appending forecast sales table and actual sales table )
2.  fact_actual_estimates(table created) Left Join gross price table
3. Create calculated columns for gross sales amount and net sales amount 

    ***additional important steps***
 Fiscal year in AtliQ begins from september, we add calculated columns 
 1. fy_month_num= MONTH(DATE(YEAR(dim_date[date]),MONTH(dim_date[date])+4),1)
 2. quarters= ROUNDUP(dim_date[fy_month_num]/3,0)

 
  **Data modelling**

  in the model view i have established relationships between subdimension, dimension  and facts tables eventually forming a 
  *Snowflake schema*.

  To better analyze and answer some of the most important business questions we must use DAX to create measures in order to be able to build dynamic visuals and gather insight .

* measures for analysis 
1. COGS(costs of goods sold)
2. net profit%
3. net margin %
4. abs error %
5. forecast accuracy %

* measures for dynamic visuals/titles
1. Selected P&L Row (finance View )
2. top/bottom title (executive View)
3. Variance % filter (Sales View)
4. BM Title (Executive View) for  LY and Target




## DASHBOARD 


**homepage**






**Finance View**



**Sales View**


**Marketing View**

**Supply Chain**

**Executive View**





 







    







