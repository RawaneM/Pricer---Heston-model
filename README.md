# Pricer---Heston-stochastic-volatility-model
Throughout the years, since the publication of the famous Black-Scholes Merton (BSM) model (1973), 
the financial industry has made a breakthrough on options pricing matter. But it also appears that 
this model has its limits. The most prominently bias of the BSM model is that prices of out-of-the-
money put and in-the-money call, observed on the market are more expensive than prices given by the 
BMS model. This problem is known as volatility smile or volatility smirk. We also noticed that local 
volatility models like BSM cannot explain the term structure of implied volatility (smile shape for 
example) because in their framework they assume that volatility is constant.

Researchers and academicians suggest the use of stochastic volatility models that gives a better 
explanation of the term structure of the implied volatility. The reason is that stochastic volatility 
models allow for negative correlation between the stock return and its variance, capturing an important 
feature of the equity market named as the leverage effect.

A second important feature is that stochastic volatility models can also address term structure effects 
by modeling mean reversion in the variance dynamic. Consequently many papers use a single factor stochastic 
volatility model as the starting point for more complex models, lets mention one of the most famous single 
factor stochastic volatility model : Heston model.
