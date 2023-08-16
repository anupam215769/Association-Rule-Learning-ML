# Association Rule Learning

Association rule learning is a type of [Unsupervised learning](https://en.wikipedia.org/wiki/Unsupervised_learning) technique that checks for the dependency of one data item on another data item and maps accordingly so that it can be more profitable. It tries to find some interesting relations or associations among the variables of dataset. It is based on different rules to discover the interesting relations between variables in the database.

Association rule learning works on the concept of If and Else Statement, such as if A then B.

![association](https://static.javatpoint.com/tutorial/machine-learning/images/association-rule-learning2.png)

Here the If element is called **antecedent**, and then statement is called as **Consequent**. These types of relationships where we can find out some association or relation between two items is known as single cardinality. It is all about creating rules, and if the number of items increases, then cardinality also increases accordingly. So, to measure the associations between thousands of data items, there are several metrics. These metrics are given below:

- **Support :** Support is the frequency of A or how frequently an item appears in the dataset. It is defined as the fraction of the transaction T that contains the itemset X. If there are X datasets, then for transactions T, it can be written as:

     ![img](https://static.javatpoint.com/tutorial/machine-learning/images/association-rule-learning3.png)
     
 
- **Confidence :** Confidence indicates how often the rule has been found to be true. Or how often the items X and Y occur together in the dataset when the occurrence of X is already given. It is the ratio of the transaction that contains X and Y to the number of records that contain X.

     ![img](https://static.javatpoint.com/tutorial/machine-learning/images/association-rule-learning4.png)
     
     
- **Lift :** It is the strength of any rule, which can be defined as below formula:

     ![img](https://static.javatpoint.com/tutorial/machine-learning/images/association-rule-learning5.png)
     
     It is the ratio of the observed support measure and expected support if X and Y are independent of each other. It has three possible values: If
     
     - Lift = 1: The probability of occurrence of antecedent and consequent is independent of each other.
     
     - Lift > 1: It determines the degree to which the two itemsets are dependent to each other.
     
     - Lift < 1: It tells us that one item is a substitute for other items, which means one item has a negative effect on another.



### Apriori [Code](https://github.com/anupam215769/Association-Rule-Learning-ML/blob/main/Apriori/apriori.ipynb) OR <a href="https://colab.research.google.com/github/anupam215769/Association-Rule-Learning-ML/blob/main/Apriori/apriori.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>

### Eclat [Code](https://github.com/anupam215769/Association-Rule-Learning-ML/blob/main/Eclat/eclat.ipynb) OR <a href="https://colab.research.google.com/github/anupam215769/Association-Rule-Learning-ML/blob/main/Eclat/eclat.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"></a>

> Don't forget to add Required Data files in colab. Otherwise it won't work.


## Apriori

The Apriori algorithm uses frequent itemsets to generate association rules, and it is designed to work on the databases that contain transactions. With the help of these association rule, it determines how strongly or how weakly two objects are connected. This algorithm uses a **breadth-first search** and **Hash Tree** to calculate the itemset associations efficiently. It is the iterative process for finding the frequent itemsets from the large dataset.

![img](https://i.imgur.com/nt3V6WG.png)

![img](https://i.imgur.com/EChIZR6.png)

![img](https://i.imgur.com/athxaW5.png)


## Eclat

Eclat algorithm is data mining algorithm which is used to find frequent items. As we already know, some association rule mining algorithm uses horizontal data format and some of them uses a vertical data format for generation of frequent itemsets. Eclat can not use horizontal database. If there is any horizontal database, then we need to convert into vertical database.

This vertical approach of the ECLAT algorithm makes it a faster algorithm than the Apriori (but sometimes when intermediate results of vertical tid lists become too large for memory, thus affecting the algorithm scalability). In Apriori algorithm we need to scan database again and again for finding frequent itemsets, this limitation is reduced by using vertical dataset in Eclat. Eclat needs to scan the database only once.

![img](https://i.imgur.com/rIVRLxD.png)

## Related Repositories

### [Data Preprocessing](https://github.com/anupam215769/Data-Preprocessing-ML)

### [Regression](https://github.com/anupam215769/Regression-ML)

### [Classification](https://github.com/anupam215769/Classification-ML)

### [Clustering](https://github.com/anupam215769/Clustering-ML)

### [Reinforcement Learning](https://github.com/anupam215769/Reinforcement-Learning-ML)

