PROFITABILITY OF HUDCO
INTRODUCTION
HUDCO was set up in 1970 by the Government of India to accelerate the pace of housing and urban
development in the country. Apart from the financing operations, HUDCO offers consultancy
services, promotes research and studies and help propagate use of local building materials, cost-
effective and innovative construction technologies.
HUDCO is a unique institution with its motto of &quot;Profitability with Social Justice&quot;.
A Public Sector Company, under the Ministry of Housing and Urban Affairs (MoHUA), HUDCO has
been a key partner with the Government in building assets for the Nation. In its operations, HUDCO
lays a considerable emphasis on the housing need of the &quot;deprived&quot; that is Economically Weaker
Sections (EWS) and Low-Income Groups (LIG).
In the course of fulfilling its objectives, HUDCO has successfully demonstrated its capabilities to
attain profitability in spite of social equity. However, HUDCO’s margins are very thin and per capita
contribution of employees to the profitability of the organisation is low.
It could be observed that the rates of growth of sanctions and releases have also been increasing
steadily over the past 30 years.
This project report analyzes the various factors that affect/determine the profit after tax of HUDCO using 2 Machine Learning models ie Linear Regression and Log Linear Regression and comparing the results with the traditional approach to the problem- ie calculation using Compound Annual Growth Rate. 

Following table shows the required data:


Year	PAT
2011-12	630.33
2012-13	700.56
2013-14	726.34
2014-15	777.63
2015-16	783.79
2016-17	841.81
2017-18	1,010.18
2018-19	1,180.15
2019-20	1,708.42
2020-21	1,578.58
2021-22	1,716.60












PROJECTING THE PROFITABILITY OF HUDCO USING CAGR TILL 2030








By using the CAGR approach we only take into consideration the initial and final values ie 2011-12 and 2021-22:




Here;
Vbegin = PAT2011-12  = 630.33 CR
Vfinal  = PAT2021-22 = 1716.60
t = 10

INTERPRETATION
Here the CAGR theoretically comes out to be:
(1716.60/630.33)*(1/10) - 1 = 10.537 

Thus, using the obtained CAGR we are able to calculate the PAT for 2022-23 using the following formula:

FV : Future value
PV: Previous value
CAGR : Calculated Compound Annual Growth Rate
n: Time duration in years

So, for predicting the PAT2022-23:
PV = PAT2011-12
CAGR = 10.537
n = 10
Thus, it is predicted that HUDCO will incur a profit after tax of Rs.1897.48880054 crores

Similarly, we are able to predict the Future PATs of HUDCO as follows:
2022-23	1897.488801
2023-24	2097.438977
2024-25	2318.459145
2025-26	2562.769581
2026-27	2832.824524
2027-28	3131.336834
2028-29	3461.305239
2029-30	3826.044463
2030-31	4229.218525
2031-32	4674.87754



PROJECTING THE PROFITABILITY OF HUDCO USING LINEAR REGRESSION
This form of analysis estimates the coefficients of the linear equation, involving one or more independent variables that best predict the value of the dependent variable. Linear regression fits a straight line or surface that minimizes the discrepancies between predicted and actual output values. There are simple linear regression calculators that use a “least squares” method to discover the best-fit line for a set of paired data. You then estimate the value of X (dependent variable) from Y (independent variable).


The correlation coefficient measures the relationship between two variables. The correlation coefficient can never be less than -1 or higher than 1. 1 = there is a perfect linear relationship between the variables. Here we calculate the correlation coefficient with respect to the actual PAT from 2011-2022(ie our training data) and the Linearly Regressing line which will be used for prediction.




INTERPRETATION
Here r2 =  0.8593492829618616
This means that since we are fairly close to 1, the Linear Regression model is a considerable choice for out prediction.





Here:
Slope( m ) = 11746.41203
Intercept( c ) =  -235748.17706766922
Eqn: y = mx + c













Thus, predicted values as per our Linear Regression Machine Learning Model is:

2022-23	1764.27
2023-24	1881.74
2024-25	1999.2
2025-26	2116.67
2026-27	2234.13
2027-28	2351.59
2028-29	2469.06
2029-30	2586.52
2030-31	2703.99






































PROJECTING THE PROFITABILITY OF HUDCO USING LOG LINEAR REGRESSION TILL 2030
A log-linear model is a mathematical model that takes the form of a function whose logarithm equals a linear combination of the parameters of the model, which makes it possible to apply (possibly multivariate) linear regression. 





Here
Slope ( m ) =  0.10829 
Intercept ( c ) = -211.43
Eqn = log(y) = mx + c

INTERPRETATION
Correlation coefficient: 
Here r2 = 0.905040032261127
This value closer to 1 than the r2 obtained in Linear regression which means that the  the discrepancies between predicted and actual output values are lesser than that in Linear regression thus making it a better fit for our training dataset.












Predicted output as per Log Linear model is:
2022-23	1897.48
2023-24	2097.43
2024-25	2318.45
2025-26	2562.76
2026-27	2832.82
2027-28	3131.33
2028-29	3461.3
2029-30	3826.04
2030-31	4229.21
2031-32	4674.87









































CONCLUSION:
Year		CAGR	      Linear Regression      Log Linear Regression
2022-23	1897.4888	1764.27	1867.54
2023-24	2097.438977	1881.74	2081.13
2024-25	2318.459145	1999.2	2319.15
2025-26	2562.769581	2116.67	2584.4
2026-27	2832.824524	2234.13	2879.98
2027-28	3131.336834	2351.59	3209.37
2028-29	3461.305239	2469.06	3576.42
2029-30	3826.044463	2586.52	3985.46
2030-31	4229.218525	2703.99	4441.28


Comparative Analysis 



i welcome further optimizations in the machine learning models for improved predictions thus improved decision making by the company
