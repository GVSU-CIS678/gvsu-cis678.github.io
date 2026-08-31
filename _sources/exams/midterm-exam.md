# Midterm Exam

---

1. A data analyst is trying to predict the popularity of movies based on past data. The dataset below classifies movies as either "Hit" or "Flop" based on their box office performance and ratings:

   | Movie | Box Office Revenue ($M) | IMDb Rating | Popularity |
   | ----- | ----------------------- | ----------- | ---------- |
   | 1     | 500                     | 8.5         | Hit        |
   | 2     | 390                     | 6.7         | Hit        |
   | 3     | 190                     | 5.8         | Flop       |
   | 4     | 60                      | 4.9         | Flop       |

   Compute the minimum, maximum, mean, median, and interquartile range (IQR) for the `IMDb Rating`.

   **Your Answer:**

2. Perform min-max normalization on both the `Box Office Revenue` and `IMDb Rating`.

   **Your Answer:**

3. Given a new movie (Movie 6) with a box office revenue of \$280M and an IMDb rating of 7.3, predict whether it will be a "Hit" or a "Flop" by finding its most similar movie from the historical dataset using the Euclidean distance formula.

   **Your Answer:**

4. Based on your previous analysis, will Movie 5 be a "Hit" or a "Flop"?

   - [ ] Hit
   - [ ] Flop

5. A food delivery company wants to know if the choice of cuisine affects customer satisfaction. Below is the data showing customer satisfaction ratings for three different cuisines:

   | Cuisine | Satisfied Customers | Dissatisfied Customers |
   | ------- | ------------------- | ---------------------- |
   | Italian | 50                  | 30                     |
   | Mexican | 60                  | 20                     |
   | Chinese | 70                  | 10                     |

   Calculate the χ² statistic for the given data.

   **Your Answer:**

6. Using the critical values in Table 1 for the χ² distribution and a significance level of 0.01, determine whether there is a significant relationship between the choice of cuisine and customer satisfaction.

   - [ ] Yes
   - [ ] No

   **Table 1: Upper-tail critical values of χ2 distribution with ν degrees of freedom**

   | **degree of freedom $\nu $** | **0.1** | **0.05** | **0.025** | **0.01** | **0.001** |
   | :-: | :-: | :-: | :-: | :-: | :-: |
   | 1 | 2.706 | 3.841 | 5.024 | 6.635 | 10.828 |
   | 2 | 4.605 | 5.991 | 7.378 | 9.210 | 13.816 |
   | 3 | 6.251 | 7.815 | 9.348 | 11.345 | 16.266 |
   | 4 | 7.779 | 9.488 | 11.143 | 13.277 | 18.467 |

7. You are given two probability distributions for user preferences between four online video platforms:

   | Platform | True Probability (p) | Predicted Probability (q) |
   | -------- | -------------------- | ------------------------- |
   | YouTube  | 0.25                 | 0.5                       |
   | Netflix  | 0.25                 | 0.03125                   |
   | Hulu     | 0.5                  | 0.25                      |
   | Disney+  | 0                    | 0.2185                    |

   **Calculate the Cross-Entropy** between the true distribution and the predicted distribution using the formula:

   $$H(p, q) = - \sum_i p(i) \log_2 q(i)$$

   **Your Answer:**

8. **Calculate the KL Divergence** (Kullback-Leibler Divergence) between the true distribution \(p\) and the predicted distribution \(q\) using the formula:

   $$D_{KL}(p||q) = \sum_i p(i) \log_2 \frac{p(i)}{q(i)} $$

   **Your Answer:**

9. A sound engineer is analyzing a signal represented by the amplitude values below, recorded at equal intervals of time:

   | Time (ms) | Amplitude |
   | --------- | --------- |
   | 1         | 24        |
   | 2         | 20        |
   | 3         | 18        |
   | 4         | 26        |
   | 5         | 30        |
   | 6         | 28        |
   | 7         | 22        |

   Apply **Discrete Wavelet Transform (DWT)** to compress the signal into \_\_

   **Your Answer:**

10. You are given the following dataset representing **Monthly Salary** and **Years of Experience** for employees at a tech company. Calculate **Spearman's rank correlation** to determine whether there is a relationship between salary and years of experience.

    | Employee | Monthly Salary (\$) | Years of Experience |
    | -------- | ------------------- | ------------------- |
    | 1        | 4500                | 3                   |
    | 2        | 6000                | 1                   |
    | 3        | 3500                | 2                   |
    | 4        | 3000                | 4                   |
    | 5        | 7000                | 10                  |

    **Your Answer:**

11. The following data show the term-frequency information for two classes of text documents:

    $$
    \text{Class A} = \{\text{apple}: 4, \text{banana}: 4, \text{cherry}: 2, \text{pear}: 2\}
    $$

    $$
    \text{Class B} = \{\text{apple}: 6, \text{banana}: 2, \text{cherry}: 2, \text{orange}: 1\}
    $$

    Assume that both classes share the same vocabulary. To address the **zero-probability problem**, apply Add-1 (Laplace) smoothing to obtain the smoothed probability distributions for the two classes. After applying Add-1 smoothing, what are the smoothed probability distributions of the words in Class A and Class B?
