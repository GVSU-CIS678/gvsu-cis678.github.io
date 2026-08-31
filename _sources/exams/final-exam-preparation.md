# Exam Review Exercises

1. Consider a dataset D containing two classes, A and B, with the following distribution:

   - 40 instances belong to class A
   - 60 instances belong to class B.

   Calculate the Gini impurity for the dataset D:

   $$Gini(D) = ... $$

   <!-- 1 - (40/100)^2 - (60/100)^2 = 0.48 -->

2. Given the following dataset with two categorical attributes (Weather and Time of Day) and a class label, use the Naïve Bayes classifier to predict the class label of a new sample (Weather = Sunny, Time of Day = Evening).

   | **Weather** | **Time of Day** | **Class Label (Go Outside)** |
   | ----------- | --------------- | ---------------------------- |
   | Sunny       | Morning         | Yes                          |
   | Rainy       | Afternoon       | No                           |
   | Cloudy      | Evening         | Yes                          |
   | Sunny       | Evening         | No                           |
   | Cloudy      | Morning         | Yes                          |
   | Rainy       | Night           | No                           |
   | Sunny       | Afternoon       | Yes                          |

   <!-- $$
   P_{Yes} &= \frac{4}{7}, P_{No} = \frac{3}{7}\\
   P(Sunny|Yes) &= \frac{2}{4}, P(Evening|Yes) = \frac{1}{4}\\
   P(Sunny|No) &= \frac{1}{3}, P(Evening|No) = \frac{1}{3}\\
   P(Yes|Sunny,Evening) &= P(Sunny|Yes) \times P(Evening|Yes) \times P_{Yes} \\
   &= \frac{2}{4} \times \frac{1}{4} \times \frac{4}{7} = \frac{1}{14}\\
   P(No |Sunny,Evening) &= P(Sunny|No) \times P(Evening|No) \times P_{No} \\
   &= \frac{1}{3} \times \frac{1}{3} \times \frac{3}{7} = \frac{1}{21}\\
   $$ -->

3. Given the following confusion matrix, calculate Precision, Recall, and F1 Score.

   |                 | Predicted Positive | Predicted Negative |
   | --------------- | ------------------ | ------------------ |
   | Actual Positive | 20                 | 5                  |
   | Actual Negative | 10                 | 30                 |

4. A probabilistic classifier has been applied to a test set of 10 tuples. Below are the probability values of these tuples belonging to the positive class, sorted in decreasing order. Based on these probabilities and the actual class labels, calculate the True Positive Rate (TPR) and False Positive Rate (FPR) at each threshold, and then sketch the ROC curve.

   | Probability | Actual Class |
   | ----------- | ------------ |
   | 0.90        | Positive     |
   | 0.85        | Positive     |
   | 0.80        | Negative     |
   | 0.75        | Positive     |
   | 0.70        | Negative     |
   | 0.65        | Negative     |
   | 0.60        | Positive     |
   | 0.55        | Negative     |
   | 0.50        | Positive     |
   | 0.45        | Negative     |

5. Given a dataset with 5 tuples {A, B, C, D, E} and their distance matrix as shown below, perform two rounds of Agglomerative Clustering.

   |       | **A** | **B** | **C** | **D** | **E** |
   | ----- | ----- | ----- | ----- | ----- | ----- |
   | **A** | 0.00  | 2.24  | 4.12  | 7.07  | 7.00  |
   | **B** | 2.24  | 0.00  | 3.16  | 5.00  | 6.32  |
   | **C** | 4.12  | 3.16  | 0.00  | 4.12  | 3.26  |
   | **D** | 7.07  | 5.00  | 4.12  | 0.00  | 5.39  |
   | **E** | 7.00  | 6.32  | 3.26  | 5.39  | 0.00  |

   - **Round 1:** Merge the closest pair A and B into a cluster.
   - **Round 2:** Apply Single Linkage, Average Linkage, and Complete Linkage to determine the next merge. For each linkage method, identify the next cluster merge and explain how the choice of linkage affects the clustering result.

     <!-- **Single Linkage**:

     - After merging A and B, we calculate the minimum distance between the new cluster (AB) and other clusters.
     - Distances: (AB)-C: 3.16, (AB)-D: 5, (AB)-E: 6.32, CD: 4.12. CE:3.26, DE: 5.39
     - Result: Merge (AB) and C.

     - **Average Linkage**:

       - For average linkage, calculate the average distance between the new cluster (AB) and other clusters.
       - Distances: (AB)-C: (4.12 + 3.16) / 2 = 3.64, (AB)-D: (7.07 + 5.00) /2 =6.035, (AB)-E: (7.00 + 6.32)/2 = 6.66, CD: 4.12. CE:3.26, DE: 5.39
       - Result: Merge C and E.

     - **Complete Linkage**:
       - For complete linkage, calculate the maximum distance between the new cluster (AB) and other clusters.
       - Distances: (AB)-C: 4.12, (AB)-D: 7.07, (AB)-E: 7.00, CD: 4.12. CE:3.26, DE: 5.39
       - Result: Merge C and E. -->

6. Consider a Convolutional Neural Network (CNN) layer that receives an input volume of size 128x65x3 (width x height x depth). If this layer uses 12 filters of size 5x5x3 with a stride of 3 and padding 3.

   - Calculate the output volume size of this layer.
   - The number of parameters in this layer.

   <!-- - Calculate the output volume size of this layer.

     $$
     &\frac{128+6-5}{3}+1 = 44\\
     &\frac{65+6-5}{3}+1 = 23\\
     $$

     output volume size = $44\times 23\times 12$.

   - Calculate the number of parameters in this layer, considering both the weights and biases.

     number of parameters = $\left((5\times 5\times 3)+1\right)\times 12 = 912$ -->
