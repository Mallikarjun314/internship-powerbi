# 1 / August / 2025
---------------------------------
# Pivot Tables
1. First Convert Range data to Tabular Data
2. Then Create a Pivot Tables from it
3. Main Concepts in Pivot Table
3.1. Filters  : Criteria Columns
3.2. Rows     : Criteria Columns
3.3. Columns  : Criteria Columns
3.4. Values   : Important Columns to Aggregate
-----------------------------------------------
4. Sorting
4.1. Sorting by Label
4.2. Sorting by Value
5. Filtering
5.1. Filtering by Label
5.2. Filtering by Value
6. Show and Summarizing values by different Criteria: 
6.1. Summarize: Sum, Max, Min, Avg, Count, Product
6.2. Show: 
6.2.1. Percentage of Grand Total
6.2.2. Percentage of Column Total
6.2.3. Percentage of Row Total
7. Nested Rows and Columns
7.1. Broad categories should be at top
7.2. Narrow categories should be at the bottom
====================================================
# Video Games Sales Dataset
1. Name	
2. Platform
3. Year
4. Genre
5. Publisher
6. NA_Sales
7. EU_Sales
8. JP_Sales
9. Other_Sales
10. Global_Sales

# Students Marks Dataset
1. Id
2. Student Name
3. Gender
4. Age
5. Section
6. Science
7. English
8. History
9. Maths
====================================================
# Charts (Data Visualization)
1. Column Chart
2. Bar Chart
3. Pie Chart
4. Line Chart
5. Scatter Plot
====================================================
# Formulas
### MATH
```
=SUM(range / value, ...)
=PRODUCT(range / value, ...)
=ROUND(value)
=ROUNDUP(value)
=ROUNDDOWN(value)
=INT(value)
=MOD(val1, val2)
=POWER(val1, val2)
=SQRT(val1)
```
### Logical
```
=IF( condition, val1, val2 )
=IFERROR ( val1,  val2)
=AND( c1, c2, c3 ...)
=OR( c1, c2, c3, ...)
=NOT( condition )
=IFS( c1, v1, c2, v2, c3, v3 ...)
```

### Date & Time
```
=TODAY()
=NOW()
=DATE( yyyy, mm, dd)
=DAY(date)
=MONTH(date)
=YEAR(date)
```

### Lookup & Reference ***
```
=VLOOKUP(val, table-range, pos ,FALSE)
=HLOOKUP(val, table-range, pos ,FALSE)
=INDEX(pos, range)
=MATCH(val, range, FALSE)
=CHOOSE(pos, val1, val2, val3, ...)
```

### Statistics
```
=AVERAGE( range / values )
=MEDIAN( range / values )
=MODE( range / values )
=MAX( range / values )
=MIN( range / values )
=COUNT( range / values )
=COUNTBLANK( range / values )
=COUNTIF( range / values )
=COUNTIFS( range / values )
```

### Text Functions
```
CONCAT
TEXTJOIN
LEFT
RIGHT
MID
LEN
FIND
SEARCH
TRIM
UPPER
LOWER
PROPER
REPLACE
SUBSTITUTE
```

### Arrays
```
UNIQUE
SORT
FILTER
SEQUENCE
RANDARRAY
```