# Debt Levels and the Non-linear Effect of Inflation on Public Debt

## Authors
Oscar M. Valencia, Juan Camilo Díaz, Jorge Guerra, Gustavo Sánchez

## Description
This repository contains the quantitative analysis based on quantile regression models that examine the interaction between inflation and public debt in the context of recent global economic shocks and the COVID-19 pandemic. Governments worldwide are facing challenges related to soaring public debt levels and high inflation rates, making the understanding of their interplay crucial for fiscal policy.

### Document Structure
The analysis is divided into two main sections:
1. **Quantitative Analysis of Inflation and Public Debt:** Examines how inflation affects public debt across its entire distribution, highlighting the threshold beyond which inflation exacerbates debt levels.
2. **Impact of Inflation on Debt Sustainability:** Explores the mechanisms through which inflation influences debt sustainability, focusing on the role of investor expectations and debt service costs.

### Methodology
Our study employs a two-pronged methodological approach:
- **Quantile Regression Models:** To analyze the impact of inflation across different levels of public debt, uncovering the nonlinear effects.
- **Instrumental Variables:** To address the potential endogeneity between inflation and public debt, using unexpected inflation as an exogenous instrument.

#### Quantile Regression Equation

The $q^{th}$ conditional quantile regression of Debt-to-GDP ratio ($Debt_{i,t}$) for country $i$ and year $t$ is represented as follows:

$$Q_q(Debt_{i,t}|\pi_{i,t-1}, X_{i,t-1}, \varepsilon_{i,t}) = \beta(q)\pi_{i,t-1} + \Omega(q)X_{i,t-1} + \alpha(q,\varepsilon_i)$$

Where:
- $\pi_{i,t-1}$ represents the inflation of consumer prices at the end of the period.
- $\varepsilon_i$ is a country unobserved random vector with $E[\alpha(\tau,\varepsilon_i)]=0$.
- $X_{i,t-1}$ includes control variables such as real GDP growth, depreciation, primary balance, interest payment, trade openness, world governance indicators average, and a democracy index.
- $\beta(q)$ and $\Omega(q)$ adjust the inflation and control variables' impact at the q-th quantile, respectively.
- $\alpha(q,\varepsilon_i)$ adjusts for country-specific unobserved heterogeneity.


> **Note:** Specific data points and results will be continuously updated and discussed within this repository.

## Data and Sources

This project utilizes data from several reputable sources to ensure the accuracy of our analysis and simulations:

- **Macroeconomic and Fiscal Indicators:** Data is gathered from the International Monetary Fund’s World Economic Outlook (IMF-WEO) as of April 2023 and includes variables such as real GDP growth, inflation, and debt levels. Available at [IMF - World Economic Outlook Databases](https://www.imf.org/en/Publications/WEO/weo-database/2023/April).

- **Institutional Variables:** Information regarding political institutions and governance is taken from the World Bank’s World Governance Indicators database and Scartascini et al. (2021). These are crucial for our control variables in the regression models. Accessible at [World Bank - World Governance Indicators](https://info.worldbank.org/governance/wgi/).

- **Unexpected Inflation Data:** For the instrumental variable approach, unexpected inflation data is calculated based on the deviation between IMF-WEO forecasts and actual inflation rates, serving as an exogenous shock in our analysis.

These sources provide the foundational data necessary for a comprehensive understanding of the dynamics between inflation and public debt, critical for our study's insights into fiscal policy challenges.

## License
This project is licensed under the MIT License, allowing for usage, modification, and distribution under certain conditions.

### Contact
For questions or collaborations, please contact [Jorge Guerra](mailto:ja.guerrae@uniandes.edu.co)
