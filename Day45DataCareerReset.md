Day 45 of building in public

I continued working on Danny Ma's 8 Week SQL Challenge, Case Study 2 and two questions this week looked straightforward on the surface but had some real thinking behind them.

Question 5: How many Vegetarian and Meat Lovers pizzas did each customer order?

The result table is what made this interesting. The answer needed both pizza counts sitting side by side on a single row per customer, not stacked on separate rows.

To do that, you use a technique called pivoting. Instead of a simple GROUP BY and COUNT, you wrap CASE WHEN inside COUNT to create two separate columns from one:

COUNT(CASE WHEN pizza_name = 'Meat Lovers' THEN 1 ELSE 0 END)
COUNT(CASE WHEN pizza_name = 'Vegetarian' THEN 1 ELSE 0 END)

Little tricks like this are why I love SQL because it forces you to think like an analyst.

It's as though the learning in SQL never ends
