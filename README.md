# Friend-Recommendations-Using-Mutual-Friends
Generated friend recommendations for users in a dataset using Spark based MapReduce algorithm.

### Notes:
The recommendations are based on the number of mutual friends. For example, if users X and Y are not yet friends but have a large number of mutual friends, then we recommend them to each other.

The dataset used contains data in the following format for each line:
UserID List of friends’ UserIDs separated by commas.

There is a tab character after the UserID. Also, note that the friendship relationship is undirected i.e.
if X is a friend of Y, then Y is also a friend of X.

For a random subset of 10 users, I generated an ordered list of the top 10 friend recommendations based on the count of mutual friends.
It may not be possible to generate 10 recommendations for some users. In that case, the output is fewer than 10 recommendations.

### Instructions for running the code:
1. Sign up for a free account on Databricks Community Edition.
2. Import the notebook containing the code (.ipynb).
3. Set up a Spark cluster.
4. Execute the code.
