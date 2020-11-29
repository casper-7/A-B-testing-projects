## CASE2: Matched Pair design Test for stores 
### Case2-1 
`Background`: There is a set of treatment stores in California where the cherry flavor of the product will be sold.

`Question`: Matching 2 control stores to each of the stores for the set of the treatment stores for cherry flavor

### Before selecting `Treatment Unit`:
* identify outliers
  * remove stores that has oulier value for sales
  * any stores in states with very few stores
* descide on number of treatment units
* randomly select the treatment units

### `Control Unit`:
* sales volume
* number of product sold
* the state where the store is located


![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case2-1.png)

### Case2-2 
`Background`: We already have the results of our new candy product introduction experiment. The data we have: Treatment stores; The matched pairs of control and treatment stores;The data from the experiment(contains store id, date, spend cust). The experiment was run from October 15th 2011 and ended on March 17th 2012.

`Question`: Compare the treatment and control stores to the past data to see the impact during the treatment period.

![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case2-2.png)

## Result

![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case2-3.png)

## Analyzing the Result
![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case2-2-1.png)

The total sales amount in 2010 was $1.3 million.
After we introduced the new candy line, the total spend increased to $1.38 million or an increase of $83.462.
