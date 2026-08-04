# OLS-Equity-Risk-Premia
Multi-factor OLS regression examining macroeconomic drivers of monthly S&amp;P 500 equity risk premia; identifies unemployment rate as sole significant predictor (β=0.79, p&lt;0.01).

The goal of this project is to look at several macroeconomic drivers, including yield spread and inflation change, and determine which ones have a significant impact on equity risk premia from the S&P 500. 

For this project, I used monthly data from 2000–2026, pulling S&P 500 returns from Yahoo Finance and macroeconomic indicators from FRED.

The methodology involved first running appropriate diagnostic tests to assess compliance with OLS assumptions. A Breusch-Pagan test confirmed heteroskedasticity, and Breusch-Godfrey and Durbin-Watson tests confirmed the presence of autocorrelation. A Variance Inflation Factor test found no evidence of multicollinearity. Due to the confirmation of the presence of both heteroskedasticity and autocorrelation, a Newey-West correction was applied, which confirmed that unemployment rate was the only statistically significant driver (β = 0.79, p < 0.01). 

In the end, the results suggested that business cycles are a key indicator of equity risk premia - rising unemployment, which is a proxy for economic downturns, is associated with investors demanding higher premia.
