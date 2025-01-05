# Comparing classical formula and Monte Carlo for Sample Size Estimation in A/B Testing (for conversion metrics)
This repo explores how the classical statistical formula and Monte Carlo simulation method differ in estimating sample sizes for A/B tests. Special focus is given to the impact of baseline conversion rates (
𝑝 and minimum detectable effects (𝑀𝐷𝐸).

# Insights

### 1) Impact of  𝑝:

- Higher baseline 𝑝 = 0.5 leads to greater variance 𝑝 (1 − 𝑝), increasing the influence of random fluctuations.

- This variance is more pronounced in the Monte Carlo method, leading to larger sample size requirements compared to the classical formula.


### 2) Effect of 𝑀𝐷𝐸:

- Larger 𝑀𝐷𝐸 values reduce the relative impact of variability, which can lead to convergence between methods.

- However, at higher  𝑝, even large 𝑀𝐷𝐸 values may not guarantee alignment due to increased sensitivity to fluctuations.


# Key Findings

### Small MDE:

Monte Carlo suggests significantly larger sample sizes, capturing real-world variability.

### High MDE:

The methods converge, especially when  𝑀𝐷𝐸≥3 %

![Screenshot 2025-01-05 at 12 38 17 pm](https://github.com/user-attachments/assets/6aa146e4-e09e-4c4f-a2d8-75cbff3b224f)



# Convergence Visualization

![Screenshot 2025-01-05 at 12 33 09 pm](https://github.com/user-attachments/assets/118e8c82-af3c-45bf-8d6c-0e2275d8e311)


![Screenshot 2025-01-05 at 12 33 34 pm](https://github.com/user-attachments/assets/6afd7d28-ef68-44f6-8e82-c9cff41d504f)

