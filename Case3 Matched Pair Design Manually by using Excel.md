## CASE3: Matched Pair Design Manually by using Excel

`Background`: I have sales data for both control stores and treatment stores. And, the matched pairs of control and treatment stores.

`Goal`: Calculate Lift and Significance Stage

### `Before you start:Data Cleanup`
remove outliers, missing data,matching control stores to treatment stores

### `Step 1`: Calculate Growth
1. Use PivotTable to Calculate 'Avg Gross Sales for Entire Comp Period', then use VLOOKUP to filled in the sheet. 
2. Calculate 'Gross Sales Growth'= ('Sum_Gross_Sales'-'Avg Gross Sales for Entire Comp Period') / 'Avg Gross Sales for Entire Comp Period'

### `Step 2`: Calculate the average of the growth by testing and comparable period
1. Use PivotTable

### `Step 3`：Create a list that shows each store along with the appropriate treatment pairing and treatment stores.

### `Step 4`: Calculate the 'Avg Growth Comparative Period' and 'Avg Growth Test Period'
1. Copy the content of 'Step 3'
2. Use VLOOKUP to find the information in 'Step 2'

### `Step 5`: Calculate Significance
1. Copy the content of 'Step 4'
2. Calculate 'Growth Difference'
3. Calculate P-value between 'Treatment Growth Difference' and 'Control Growth Difference'
Formular: `=T.TEST(range_of_test_group,range_of_control_group,2,3)`

  4. Significance Level=1 - p-value

### `Step 6`: Calculate Lift
1. Calculate each stores' Lift
`Lift = (Growth_Diff_Treatment_Store - Growth_Diff_Control_Store) / (1 + Growth_Diff_Control_Store)`
2. Use VLOOKUP to find each store's 'Avg Sales from Comp Period'(which is from 'Step 1')
3. Calculate 'Expected Sales Impact'
Formular: `Expected Sales Impact=Avg Sales from Comp Period * Lift`
4. Calculate 'Avg Lift' and 'Avg Expected Sales Impact'

## Result
The average lift is -1.6% and the average sales impact is -$122.4

