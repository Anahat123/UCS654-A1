# Learning Probability Density Function using NO₂ Data

## Dataset
India Air Quality Dataset  
Feature used: NO₂ concentration

## Aim
To learn the parameters of a probability density function after applying a roll-number-based non-linear transformation on NO₂ values.

## Methodology
1. The NO₂ column was extracted from the dataset and missing values were removed.
2. A non-linear transformation was applied to each value:

   z = x + aᵣ sin(bᵣ x)

   where aᵣ and bᵣ were calculated using the given roll number formula.
3. The transformed values were assumed to follow a Gaussian-shaped probability density function.
4. Parameters were estimated using Maximum Likelihood Estimation (MLE).

## Parameter Estimation
- Mean (μ) was computed as the average of transformed values.
- Variance (σ²) was computed using the mean squared deviation.
- λ and c were derived from σ².

## Results
Parameter | Estimated Value |
|---------|----------------|
| μ | 23.2883 |
| λ | 0.0019896 |
| c | 0.0251657 |

## Conclusion
The non-linear transformation slightly altered the NO₂ distribution, and the transformed data was successfully modeled using a Gaussian probability density function.
