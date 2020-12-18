## CASE4: Facial price VS store's gross margin
`Background`: A marketing team works in a chain of spas and they look for ways to increase the gross margin. We decided to experiment with the price of facial. Currently, the stores offer facials for $98.99. We need run a A/B test with different prices of facials, assuming that the average customer visits a store about once every ten weeks. 

`Goal`:We'd like to predict whether a change in price would yield greater gross margin if the facials were $87.99 or $76.99.  

### Set up a `Randomized Design`:
`Units`: Stores

### `Treatment Groups`
two treatment groups
1. stores offering facials for $87.99. 
2. stores offering facials for $76.99.

### `Control Units`
other stores with $98.99.

### `Prepare the test`
![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case4-1.png)

This is the data we have.

**continuous control variables：**
1. Average sales per store per month
2. Average number of invoices per month per store 
3. SKU Category

**data we need：**
1. 1 year plus minimum of 6 periods (if measure weekly, then may need 12 periods). To use the A/B Trend tool in Alteryx, we need to have a minimum of one year plus 12 periods (weeks) of historical data, so we’ll need a total of 64 weeks of data.
2. length of the experiment (For this case, since the average customer visits a store about once every ten weeks, so the experiment at least last 10 week.)

### `Run the test`
We need 3 data files:
1. Weekly store traffic - to see seasonality and trend -> use A/B trend tool
2. Store list data - to match control and treatment stores -> use A/B trend tool
3. Sales data - to see the final result  -> use A/B analysis tool
![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case4-3.png)
![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case4-4.png)
![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case4-2.png)

**Create Discrete Data Table:**

In this experiment, we have three variants(control stores $98.99, stores with $87.99, stores with $76.99 )

To properly match our control and treatment units, we need to create data table shows

1. Stores
2. Region
3. Group: ①control
          ②treatment

![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case%204-5.png)

Create Sales Data Table

![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case%204-6.png)

**Preparing Control and Treatment Units**

![](https://github.com/casper-7/A-B-testing-projects/blob/master/case1_image/case4-7.png)

### `Analyze the result` 
