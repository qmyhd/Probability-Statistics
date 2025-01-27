# Convergence of Binomial Distribution to Normal Distribution

This demonstrates how the Binomial distribution converges to the Normal distribution as \( N \) becomes large.

## Introduction

The Central Limit Theorem states that as the number of trials \( N \) in a Binomial distribution increases, the distribution approaches a Normal distribution with mean \( \mu = Np \) and variance \( \sigma^2 = Np(1-p) \).

## Methodology

We generated Binomial distributions for various values of \( N \) and compared them to the corresponding Normal distributions using histograms.

### Parameters

- Probability of success, \( p = 0.5 \)
- Number of trials, \( N \) values: 10, 50, 100, 1000

## Results

### For \( N = 10 \)
![Binomial vs Normal for N=10](binomial_vs_normal_N10.png)

### For \( N = 50 \)
![Binomial vs Normal for N=50](binomial_vs_normal_N50.png)

### For \( N = 100 \)
![Binomial vs Normal for N=100](binomial_vs_normal_N100.png)

### For \( N = 1000 \)
![Binomial vs Normal for N=1000](binomial_vs_normal_N1000.png)

## Conclusion

As we can see from the histograms, as \( N \) increases, the Binomial distribution starts resembling the Normal distribution more closely. This visual demonstration confirms the theoretical convergence of the Binomial distribution to the Normal distribution in the large \( N \) limit.
