# Final Exam: Calculation Questions

---

1. Consider a dataset $D$ with a categorical attribute $A$ that can take on values $a_1$ and $a_2$. Each value of $A$ corresponds to a subset of the dataset with various instances of classes $X$ and $Y$. You are required to calculate the Gini impurity of dataset $D$, denoted as $Gini(D)$, and the Gini impurity for attribute $A$, denoted as $Gini_A(D)$.

   Given the following distribution of classes within the subsets of attribute $A$:

   | Attribute $A$ | Instances of Class $X$ | Instances of Class $Y$ |
   | ------------- | ---------------------- | ---------------------- |
   | $a_1$         | 20                     | 30                     |
   | $a_2$         | 15                     | 35                     |

   - Calculate $Gini(D)$ using the provided data.

     $Gini(D) = ...$

   - Calculate $Gini_A(D)$ using the provided data.

     $Gini_A(D) = ...$

2. Given the following dataset with two categorical attributes (**Food Type** and **Meal Time**) and a class label, use the Naïve Bayes classifier to predict the class label of a new sample (**Food Type = Dessert, Meal Time = Dinner**). Which class label (Yes or No) is more probable for the sample (**Dessert, Dinner**)?

   | **Food Type** | **Meal Time** | **Class Label (Preferred)** |
   | ------------- | ------------- | --------------------------- |
   | Dessert       | Breakfast     | No                          |
   | Main Course   | Lunch         | No                          |
   | Snack         | Evening       | Yes                         |
   | Dessert       | Dinner        | No                          |
   | Main Course   | Dinner        | Yes                         |
   | Snack         | Breakfast     | No                          |
   | Dessert       | Lunch         | Yes                         |

3. Given the following confusion matrix, calculate the following metrics: Error rate(misclassification rate), specificity (True negative rate), Recall, Precision, and F1.

   |                     | **Predicted Positive** | **Predicted Negative** |
   | ------------------- | ---------------------- | ---------------------- |
   | **Actual Positive** | 48                     | 16                     |
   | **Actual Negative** | 12                     | 8                      |

4. A probabilistic classifier has been applied to a test set of 10 tuples. Below are the probability values of these tuples belonging to the positive class, sorted in decreasing order. Based on these probabilities and the actual class labels, calculate the TP, FP, TN, FN, True Positive Rate (TPR), and False Positive Rate (FPR) at each threshold, and then sketch the ROC curve.

   | Tuple ID | Prob. | Actual Class | TP  | FP  | TN  | FN  | FPR | TPR |
   | -------- | ----- | ------------ | --- | --- | --- | --- | --- | --- |
   | 1        | 0.95  | Positive     |     |     |     |     |     |     |
   | 2        | 0.81  | Positive     |     |     |     |     |     |     |
   | 3        | 0.88  | Positive     |     |     |     |     |     |     |
   | 4        | 0.72  | Negative     |     |     |     |     |     |     |
   | 5        | 0.68  | Positive     |     |     |     |     |     |     |
   | 6        | 0.77  | Positive     |     |     |     |     |     |     |
   | 7        | 0.63  | Positive     |     |     |     |     |     |     |
   | 8        | 0.46  | Negative     |     |     |     |     |     |     |
   | 9        | 0.51  | Negative     |     |     |     |     |     |     |
   | 10       | 0.56  | Negative     |     |     |     |     |     |     |

5. Consider a dataset consisting of 5 tuples {A, B, C, D, E} and their corresponding distance matrix provided below. Your task is to perform the first two rounds of Agglomerative Clustering using three different linkage methods: Single Linkage, Average Linkage, and Complete Linkage.

   **Distance Matrix**

   |       | **A** | **B** | **C** | **D** | **E** |
   | ----- | ----- | ----- | ----- | ----- | ----- |
   | **A** | 0.00  | 2.24  | 2.13  | 2.27  | 2.28  |
   | **B** | 2.24  | 0.00  | 1.16  | 5.12  | 2.32  |
   | **C** | 2.13  | 1.16  | 0.00  | 1.12  | 3.26  |
   | **D** | 2.27  | 5.12  | 1.12  | 0.00  | 4.34  |
   | **E** | 2.28  | 2.32  | 3.26  | 4.34  | 0.00  |

6. Consider a Convolutional Neural Network (CNN) layer that receives an input volume of size $509\times246\times64$. If this layer uses 28 filters of size $7\times5\times64$ with a stride of 3 and padding 4. What is the output volume size of this layer, and how many parameters (including weights and biases) are there in total?

7. If the input size is $509\times246\times64\times1$, and the layer uses 8 3D filters of size $5\times4\times6\times1$ with a stride of 2 and padding 4, what would be the output volume size and the number of parameters of this layer?
