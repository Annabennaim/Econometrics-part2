# How can the unemployment rate and the level of a country's development explain the observed birth rate?

### Bachelor's project using Gretl

This econometrics project examines the relationship between birth rates, unemployment rates, and a country's level of development. The study focuses on 37 countries from various continents to ensure a diverse and representative dataset. The goal is to determine whether economic stability (measured by unemployment) and development (measured by the Human Development Index - HDI) significantly impact birth rates.
The project aims to understand the declining global birth rate over the past decade. Even in France, which has one of the highest fertility rates in Europe, the number of births per woman reached a historic low of 1.68 in 2024.

## Description of the variables:

1) Birth rate: it's the dependent variable (Y), measured as the number of births per 1,000 people. Data is sourced from INED and Atlasocio.
2) Unemployement rate: it's our first explanatory varibale (X1),expressed as a percentage of the working-age population. Data is obtained from the World Bank and Trading Economics. The correlation between birth rate and unemployment is very weak, suggesting minimal influence.
3) it's our second explanatory variable (X2), ranges from 0 to 1, with higher values indicating more developed countries. The correlation between HDI and birth rate is negative, meaning that as development increases, birth rates decrease.

## Model Estimation (Ordinary Least Squares - OLS) and model validation
A multiple regression model is used:
        Y= 52.26–0.073𝑿𝟏 –47.51𝑿𝟐 + ε
        
To determine if our model is significant, we are using a test of Fischer and it will allow us to determine whether all of the explanatory variables taken simultaneously can explain the variations of the dependent variable.
We obtain that the model is statistically significant, meaning at least one explanatory variable impacts birth rates.

We are then using the test of Student on all the coefficients of our explenatory variables to determine if they are significant :

- The unemployment rate (X1) is not statistically significant, meaning it does not meaningfully affect birth rates.
- The development level (X2) is highly significant, confirming its strong influence.

## Additional Tests
- Chow Test (Structural Break): Results suggest that the model should be divided into two subgroups:
countries with high birth rates (>10.73 per 1,000) and countries with low birth rates (<10.37 per 1,000), mostly Western nations

- Variable Addition Test: Adding the unemployment rate does not improve the model, reinforcing its lack of significance.

## Conclusion
- Key Findings:
Development level (HDI) significantly explains birth rate variations. Higher development leads to lower birth rates due to increased education, contraception access, and shifting societal norms.
Unemployment rate has no significant impact. Economic instability alone does not seem to affect birth rates in a meaningful way.
Model accuracy: The model explains 73.71% of birth rate variations, but 30% remains unexplained, suggesting other factors (e.g., cultural influences, government policies).

- Future Improvements:
Removing unemployment as a variable and adding new explanatory factors could refine the model further.
Expanding the dataset to consider long-term trends rather than just 2023 values.
