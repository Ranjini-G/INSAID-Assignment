# Letter Recognition
[![ltr1](https://github.com/Ranjini-G/INSAID-Assignment/blob/master/Images/ltr1.jpg "ltr1")](https://github.com/Ranjini-G/INSAID-Assignment/blob/master/Images/ltr1.jpg "ltr1")

### Problem statement
The objective is to **identify each of a large number of black-and-white rectangular pixel displays as one of the 26 capital letters in the English alphabet**. The character images were based on 20 different fonts and each letter within these 20 fonts was randomly distorted to produce a file of 20,000 unique stimuli. Each stimulus was converted into 16 primitive numerical attributes (statistical moments and edge counts) which were then scaled to fit into a range of integer values from 0 through 15. We typically train on the first 16000 items and then use the resulting model to predict the letter category for the remaining 4000.

### Data description
| Column Name  | Description  |
| ------------ | ------------ |
| letter  | capital letter (26 values from A to Z)  |
| x-box  | horizontal position of box  |
| y-box  | vertical position of box  |
| width  | width of box  |
| high  | height of box  |
| onpix  | total # on pixels  |
| x-bar  | mean x of on pixels in box  |
| y-bar  | mean y of on pixels in box  |
| x2bar  | mean x variance  |
| y2bar  | mean y variance  |
| xybar  | mean x y correlation  |
| x2ybr  | mean of x * x * y  |
| xy2br  | mean of x * y * y  |
| x-ege  | mean edge count left to right  |
| xegvy  | correlation of x-ege with y  |
| y-ege  | mean edge count bottom to top  |
| yegvx  | correlation of y-ege with x  |

### Summary

Various classifier models were used to predict the letters.   These models were evaluated on different metrics to  know their performance.  Listed here are the results:

| Algorithm  | Accuracy  | f1_Score  |
| ------------ | ------------ | ------------ |
| DecisionTree  | 0.999875  | 0.999876  |
| NaiveBayes  | 0.651125  | 0.646085  |
| RandomForest  | 0.999812  | 0.999816  |
| KNN  | 0.960187  | 0.960086  |
| SVM  | 0.860625  | 0.859713  |
| SGD  | 0.602125  | 0.600893  |
| EnsembleVotingClassifier  | 0.999812  | 0.999816  |

**Decision tree** model has got the highest score in all the metric test and with **99.9% accuracy**. This model is used to predict the test observations.

