I wrote the perfect SQL query… and still got the wrong answer


I'm currently working through Case Study 2 of Danny Ma's 8 Week SQL Challenge (Pizza Runner), and the first real challenge had nothing to do with writing clever queries, it was about cleaning messy data.

Here's what the raw tables actually looked like:
- The same "no value" was stored 3 different ways, empty strings, the word 'null', and 'NaN'
- Distance had values like '20km', '23.4 km', and just '10', all in the same column
- Duration had '32 minutes', '20 mins', '15 minute', and '15', no consistency at all 

If you run queries on data like that, you either get errors or wrong answers. Either way, your analysis is broken before it starts.

So the first thing I did was build cleaned versions of the problem tables, preserving the original raw data and creating clean ones to query from.

The functions that made it possible where these:
- CASE WHEN to catch every variation of a missing value
- REPLACE() to strip units like 'km' from numbers
- Type casting to convert text columns into proper numbers and timestamps

Real datasets are messy and cleaning them is a skill.

Case Study 2 questions are next
