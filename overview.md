# Formulas and descriptions
## Expected Value $\mathrm{E}(X)$
### Linearity
$\mathrm{E}(X+Y) = \mathrm{E}(X) + \mathrm{E}(Y)$
$\mathrm{E}(aX) = a \mathrm{E}(X)$

### Normal distribution
$\mathrm{E}(X) = \mu$
$\mathrm{E}(X^2) = \mu^2 + \sigma^2$

## Variance $\mathrm{Var}(X)$
$\mathrm{Var}(X) = \mathrm{E}((X-\mu)^2)$
$\mathrm{Var}(X) = \mathrm{E}(X^2) - {\mathrm{E}(X)}^2$

## Mean
For $\forall i, 1 \le i \le n : X_i$ the mean is $\bar{X} := \frac{1}{n}\sum_{i=1}^{n}X_i$

If all $X_i$ have the same $\mathrm{E}(X_i)=\mu$, then $\bar{X}$ is a unbiased estimator of $\mu$.

## Quantile
$Q_p = X_{\lfloor{np}\rfloor+1} \quad 0 < p < 1$
Median: $\mathrm{med} = Q_{0.5}$
Quartiles: $Q_{0.25}, Q_{0.5}, Q_{0.75}$
Percentiles: $Q_{0.1}, Q_{0.2}, \ldots Q_{0.9}$

## $\alpha$-trimmed mean
$\bar{X}_\alpha$ for $\alpha \in (0,0.5)$

$\bar{X}_\alpha = \frac{1}{n - 2\lfloor{n\alpha}\rfloor}
\sum_{k=\lfloor{n\alpha}\rfloor+1}^{n -\lfloor{n\alpha}\rfloor}X_{(k)}$

## Mode
The value that is most frequent.

## Statistical Dispersion
### Standard Deviation
$S = {\left(\frac{1}{n-1} \sum_{k=1}^{n}(X_k -\bar{X})^2\right)}^2$
##### Unbiased Estimator
If $X_1,\ldots,X_n$ is a i.i.d. random sample with $\mu = \mathrm{E}(X_1)$
and $\sigma^2 = \mathrm{Var}(X_1)$, then $S^2$ is an unbiased estimator for
the true variance $\sigma^2 = \mathrm{E}(S^2)$.

### Likelihood Standard Deviation
$S_L = {\left(\frac{1}{n} \sum_{k=1}^{n}(X_k -\bar{X})^2\right)}^2$
### iqr-Standard Deviation
iqr = interquantile range
$S_q = \frac{\mathrm{iqr}}{1.349} = \frac{Q_{0.75} - Q_{0.25}}{1.349}$
### mad-Standard Deviation
mad = median absolute deviation
$S_{mad} = \frac{1}{0.675}\mathrm{mad}(X_1,X_2,\ldots, X_n) =
\frac{1}{0.675}\mathrm{mad}(\{|X_k-Q_{0.5}|, 1 \le k \le n\})$

