SQL questions used to confuse me a lot. I would look at a question and freeze, not knowing where to start.

Then I developed a simple method that makes any SQL question manageable. Here’s how I approach it:

Step 1: Translate the question into simple English
Example:

“What is the most purchased item and how many times was it ordered?”
Simple version:
	•	Across all customers → which product was ordered the most?
	•	And how many times?

Step 2: Design the result table → what should the final answer look like

Step 3: Map columns → figure out which table each piece of data comes from

Step 4: Ask yourself → what do we need to calculate?
Example: “How do I know what’s most purchased?” → Count how many times each product appears

Step 5: Build the logic slowly → step by step

Example:

SELECT product_id, COUNT(*) 
FROM sales
GROUP BY product_id;

Step 6: THEN write the full SQL query

Pro tip: You’ll get better and faster every day if you practice this method, you won’t get it right once, practice makes perfect.

If SQL has been giving you a headache, try this method on your next practice question and let me know how it goes!
