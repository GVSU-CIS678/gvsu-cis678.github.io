# KL-Divergence

With Add-1 Smoothing

---

Given the sample distributions:

$P = \{a: 1/2, c: 1/4, d: 1/4\}$

$Q = \{a: 2/5, b: 1/5, e: 2/5\}$

## [KL-Divergence](https://en.wikipedia.org/wiki/Kullback%E2%80%93Leibler_divergence):

$$D_{KL}(P|| Q) = \sum_{i \in \{a, b, c, d, e\}} P(i) \times \ln \left( \frac{P(i)}{Q(i)} \right)$$

If we calculate this KL-Divergence, for any value $i$ where $Q(i) = 0$, the value becomes infinite (since dividing by zero is undefined).

To handle this case, we apply smoothing. I described a simple method for smoothing in the lecture, which introduces the idea of accounting for unseen events when calculating KL-Divergence. In practice, more refined smoothing techniques are often employed. One such technique is `add-one smoothing` (also known as `Laplacian correction` or `Laplace smoothing`). This method is a popular solution to the `Zero-Probability problem`. More details are available on the [Wikipedia page](https://en.wikipedia.org/wiki/Additive_smoothing).

### Add-1 Smoothing

For $P$, there are 4 samples: two a's, 1 c, and 1 d, but it's missing b and e. Considering a total of 5 values {a,b,c,d,e}, we add 1 for each:

- $P'(a) = \frac{(1/2 \times 4) + 1}{4 + 5} = \frac{1}{3}$
- $P'(b) = \frac{1}{9}$
- $P'(c) = \frac{(1/4 \times 4) + 1}{4 + 5} = \frac{2}{9}$
- $P'(d) = \frac{(1/4 \times 4) + 1}{4 + 5} = \frac{2}{9}$
- $P'(e) = \frac{1}{9}$

For $Q$, we follow the same smoothing process:

- $Q'(a) = \frac{(2/5 \times 5) + 1}{5 + 5} = \frac{3}{10}=0.3$
- $Q'(b) = \frac{(1/5 \times 5) + 1}{5 + 5} = \frac{1}{5}=0.2$
- $Q'(c) = \frac{1}{10}=0.1$
- $Q'(d) = \frac{1}{10}=0.1$
- $Q'(e) = \frac{(2/5 \times 5) + 1}{5 + 5} = \frac{3}{10}=0.3$

### KL-Divergence Calculation

$$
D_{KL}(P' || Q') = \sum_{i \in \{a, b, c, d, e\}} P'(i) \times \ln \left( \frac{P'(i)}{Q'(i)} \right)\\
% = P'(a)\times \ln\left(\frac{P'(a)}{Q'(a)}\right) + P'(b)\times \ln\left(\frac{P'(b)}{Q'(b)}\right) + P'(c)\times \ln\left(\frac{P'(c)}{Q'(c)}\right) + P'(d)\times \ln\left(\frac{P'(d)}{Q'(d)}\right) + P'(e)\times \ln\left(\frac{P'(e)}{Q'(e)}\right)\\
= \frac{1}{3}\times \ln\left(\frac{\frac{1}{3}}{0.3}\right) + \frac{1}{9}\times \ln\left(\frac{\frac{1}{9}}{0.2}\right) + \frac{2}{9}\times \ln\left(\frac{\frac{2}{9}}{0.1}\right) + \frac{2}{9}\times \ln\left(\frac{\frac{2}{9}}{0.1}\right) + \frac{1}{9}\times \ln\left(\frac{\frac{1}{9}}{0.3}\right)
$$
