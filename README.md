Overview:

Market Basket Analysis (MBA) is a method of data mining used in various ‘recommender’ systems. These systems contain algorithms that determine patterns in users' purchasing/browsing activity, which MBA uses to recommend products and services as effectively and accurately as possible. One of the most common algorithms associated with market basket analysis is the Apriori algorithm, which gathers a very large set of association rules (which are essentially “if-then” statements) in order to create a more efficient market, resulting in more sales. However, a crucial aspect of creating a successful market basket analysis is to distinguish ‘interesting’ association rules from the ‘uninteresting’ and potentially misleading ones.

This project includes a classic implementation of Apriori in Python, however modified to allow efficient hashing for candidate itemset frequency counting. The program also includes code to find association rules between the itemsets determined to be frequent. MBA is performed on a publicly available dataset of websites visited in a day by anonymous microsoft users. More informantion regarding the dataset is available [here](https://archive.ics.uci.edu/ml/datasets/Anonymous+Microsoft+Web+Data).

Apriori - An Overview:

The basic idea behind the Apriori algorithm is to use a bottom-up approach, where frequent subsets of items are used to generate candidate sets of higher itemsets until no more frequent itemsets can be found. The algorithm uses a support threshold to determine the minimum frequency of an itemset to be considered frequent. 

Here are the main steps of the algorithm:

Scan the database to determine the frequency of each item.

Use the frequent items to generate candidate sets of size 2.

Scan the database to determine the frequency of each candidate set.

Use the frequent candidate sets to generate candidate sets of size 3.

Repeat steps 3 and 4 until no more frequent itemsets can be found.

Use the frequent itemsets to generate association rules.

Use a confidence threshold to determine the minimum confidence of an association rule to be considered strong.

Output the strong association rules.





