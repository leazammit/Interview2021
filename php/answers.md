# Tillo Technical Test
## PHP Task 1 - Answers in plain English

> :information_source: Edit this Markdown file and in plain English, briefly describe how you would:

1. Count the total number of orders?

> Answer: by performing a count on the original json array

2. Count the number of orders that were FREE?

> Answer: By filtering over the json array where price is 0, and then performing a count

3. Count the number of orders that were placed in GBP?

> Answer: similar to the above, but considering instead where currency is GBP

4. Count the number of orders that were shipped to Essex?

> Answer: Filtering the order array where shipping county is listed as "Essex" (note that this is nested within 'shipping_address' and again in 'customer') and then perform a count on the resulting array

5. Sum the cost of orders that were placed in GBP and were £100 or more?

> Answer: as previously, the array is filtered on the given criteria (currency = GBP and price >=100), then a sum is performed on the price column of the resulting array. Finally this is rounded to 2dp to reflect currency

6. Sum the cost of orders that were placed in GBP?

> Answer: Similar to above, the orders are filtered on currency = GBP alone, and then a sum is performed on the price value of each remaining item, then rounded to 2dp.

7. Sum the cost of orders that were placed in GBP and were shipped to Essex?

> Answer: The order array is filtered on currency = gbp and county = Essex (nested as mentioned previous), after which a sum on the price value is performed and rounded off to 2dp.
