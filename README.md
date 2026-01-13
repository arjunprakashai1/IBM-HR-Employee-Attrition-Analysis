# IBM HR Employee Attrition Analysis

## Overview

This project analyzes the IBM HR Analytics Employee Attrition dataset to investigate the relationship between job satisfaction and employee attrition (turnover). Using statistical analysis, we determine whether job satisfaction levels are a significant predictor of whether employees stay with or leave the company.

## Research Question

**Is there a significant relationship between JobSatisfaction and Attrition?**

## Dataset

- **Source**: IBM HR Analytics Employee Attrition Dataset
- **Size**: 1,470 employees × 35 features
- **Key Variables**:
  - `Attrition`: Whether the employee left the company (Yes/No)
  - `JobSatisfaction`: Employee's job satisfaction level (1-4 scale)
    - 1 = Low
    - 2 = Medium
    - 3 = High
    - 4 = Very High

## Methodology

### Statistical Test: Chi-Square Test for Independence

We employed the Chi-Square test to determine whether there is a statistically significant association between job satisfaction levels and employee attrition.

**Hypotheses:**
- **Null Hypothesis (H₀)**: There is no significant association between job satisfaction and attrition
- **Alternative Hypothesis (H₁)**: There is a significant association between job satisfaction and attrition

**Significance Level**: α = 0.05

## Key Findings

### Statistical Results

- **Chi-Square Statistic**: 17.505
- **P-Value**: 0.000556
- **Conclusion**: **Reject the null hypothesis** — there is a statistically significant relationship between job satisfaction and employee attrition.

### Contingency Table Analysis

| Attrition | Satisfaction Level 1 | Satisfaction Level 2 | Satisfaction Level 3 | Satisfaction Level 4 |
|-----------|---------------------|---------------------|---------------------|---------------------|
| No        | 223                 | 234                 | 369                 | 407                 |
| Yes       | 66                  | 46                  | 73                  | 52                  |

### Insights

1. **Low Satisfaction Drives Turnover**: Employees with the lowest satisfaction (Level 1) showed 66 actual attritions versus approximately 46 expected, indicating low satisfaction is a primary driver of employee exits.

2. **High Satisfaction Reduces Attrition**: Employees with the highest satisfaction (Level 4) had only 52 actual attritions compared to approximately 74 expected, demonstrating that high job satisfaction is effective for retention.

3. **Highly Significant Relationship**: The extremely low p-value (0.000556) provides strong evidence that job satisfaction is a reliable predictor of employee retention.

## Requirements

```python
pandas
scipy
```

## Usage

1. Ensure the dataset `HR-Employee-Attrition.csv` is in the project directory
2. Open and run `Analysis.ipynb` in Jupyter Notebook or JupyterLab
3. Execute cells sequentially to reproduce the analysis

## Files

- `Analysis.ipynb`: Jupyter notebook containing the complete analysis
- `HR-Employee-Attrition.csv`: Dataset (not included in repository)
- `README.md`: This file

## Recommendations

Based on the findings, organizations should:

1. **Monitor Job Satisfaction**: Regularly assess employee satisfaction levels through surveys
2. **Address Low Satisfaction**: Prioritize interventions for employees reporting low satisfaction
3. **Retention Strategies**: Invest in programs that enhance job satisfaction to reduce turnover costs
4. **Predictive Analytics**: Use job satisfaction as a key metric in employee retention models

## License

This analysis is for educational and research purposes.

## Contact

For questions or collaboration opportunities, please open an issue in this repository.