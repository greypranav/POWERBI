### Key MEASURES involved

```
Average_Revenue = average(financials[ Sales])
```

```
Discount_offered = sum(financials[Discounts])
```

```
Profit Margin = (DIVIDE([total_Profit], [total_Sales], 0))*100
```
***
# Top N Function explained
***

```
Top3 = CALCULATE([total_Sales],topn(3,ALLSELECTED(financials[Product]),
[total_Sales],DESC),VALUES(financials[Product]))
```

## Breakdown of Components

### CALCULATE:
This function changes the context in which data is evaluated. It allows you to modify the filter context and perform calculations based on that modified context.

### [total_Sales]:
This is a measure that calculates the total sales amount. It is the value that you want to calculate for the top three products.

### TOPN(3, ALLSELECTED(financials[Product]), [total_Sales], DESC):
- **TOPN**: Returns the top N rows of a table based on a specified expression.
- **3**: Specifies that you want the top 3 products.
- **ALLSELECTED(financials[Product])**: Retrieves all products currently selected in the context of the report or visual, respecting any filters applied to the `financials[Product]` column.
- **[total_Sales]**: The expression used to rank the products, based on their total sales.
- **DESC**: Specifies that the ranking should be in descending order, meaning products with the highest sales will be at the top.

### VALUES(financials[Product]):
Returns a one-column table containing the distinct values from the `financials[Product]` column. It ensures that the context of the calculation is limited to the products being evaluated.

## Overall Logic
The entire expression calculates the total sales for the top three products based on their sales figures. It does this by:

1. Using `TOPN` to identify the top three products based on total sales.
2. Modifying the filter context with `CALCULATE` to ensure that total sales are calculated only for those top three products.
3. The use of `ALLSELECTED` allows the calculation to respect any filters applied to the product selection in the report while focusing on the top three products based on their sales.

## Summary
This DAX expression dynamically calculates and displays the total sales for the top three products in a given context, making it useful for performance analysis and reporting in business intelligence scenarios.












