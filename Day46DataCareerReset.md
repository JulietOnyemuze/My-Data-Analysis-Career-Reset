A SQL question asked for just One number:

"What was the maximum number of pizzas delivered in a single order?"

Sounds simple right? It wasn't, because you can't jump straight to the answer.

You first count how many pizzas were in each order, then find the MAX from those counts. Two steps, not one.

The real catch is this only works if your data is clean, because cancelled orders had to be excluded, and that filter only worked correctly because I had already replaced messy text 'null' values with proper NULLs in my cleaning step.

So data cleaning isn't optional, it's the foundation of every analysis.

On to question 7 🍕

#SQL #DataAnalytics #DataCleaning #BuildingInPublic #120DaysOfDataWithTina #DataAnalyticsLockedIn
