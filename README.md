# Frequently Purchased Together Analysis

## Project Overview

This project analyzes customer purchase behavior to identify products that are frequently purchased together. The analysis uses order-level transaction data from the Online Retail II dataset and applies association-style analysis using product pairs.

## Objective

The main objective is to identify product combinations that commonly occur in the same order and use these patterns to understand customer purchasing behavior.

## Dataset

Dataset: Online Retail II

The analysis uses:

* Invoice Number
* Customer ID
* Product Description
* Order-level product combinations

## Tools Used

* Python
* Pandas
* itertools
* Collections

## Analysis Steps

1. Loaded the Online Retail II dataset.
2. Removed cancelled transactions.
3. Removed records with missing Customer ID and Product Description.
4. Grouped products by Invoice Number.
5. Removed duplicate products within the same order.
6. Generated unique product pairs using combinations.
7. Excluded self-pairs.
8. Counted how many orders contained each product pair.
9. Calculated the support percentage for each pair.
10. Sorted product pairs by order frequency.
11. Identified the top 20 frequently purchased-together products.
12. Exported the final results to a CSV file.

## Key Metrics

### Order Count

The number of orders in which a particular product pair appeared together.

### Support %

The percentage of total orders containing a particular product pair.

Formula:

```text
Support % = Order Count / Total Orders × 100
```

## Results

The analysis identified the most frequently purchased product combinations based on their occurrence across customer orders.

The top product pairs included combinations involving:

* Jumbo Bags
* Lunch Bags
* Regency Teacups and Saucers
* Alarm Clocks
* Gardener-related products
* Retrospot products

## Key Insights

1. Several lunch bag and retrospot products frequently appear together in customer orders.
2. Regency Teacup and Saucer products show repeated purchasing patterns.
3. Frequently paired products can be considered for product bundling.
4. Product-pair frequency can support cross-selling and recommendation strategies.
5. Support percentage helps identify how common each combination is across all orders.

## Output

The results are also saved as:

```text
frequently_purchased_together.csv
```

## Conclusion

This project demonstrates how transaction-level purchase data can be used to discover products that customers commonly buy together. These patterns can help businesses with cross-selling, product recommendations, and bundle planning.
