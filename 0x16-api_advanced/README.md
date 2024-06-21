0x16. API advanced
This module focuses on advanced concepts related to APIs (Application Programming Interfaces). It includes practical tasks that involve interacting with the Reddit API to understand how to query endpoints, handle pagination, parse JSON responses, and implement recursive functions.


Tasks Overview
0. How many subs?
Write a function number_of_subscribers(subreddit) that queries the Reddit API and returns the number of subscribers for a given subreddit. Returns 0 if the subreddit is invalid.

1. Top Ten
Write a function top_ten(subreddit) that queries the Reddit API and prints the titles of the first 10 hot posts for a given subreddit. Prints None if the subreddit is invalid.

2. Recurse it!
Write a recursive function recurse(subreddit, hot_list=[]) that queries the Reddit API and returns a list of titles of all hot articles for a given subreddit. Returns None if the subreddit is invalid.
