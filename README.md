# Pricer---Stochastic-volatility-models
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

The use of single factor stochastic volatility model is relevant to generate smiles and smirk but these 
models appear to be highly restrictive to model the relationship between the volatility level and the 
slope of the smirk. The data suggest that the shape of the smile is largely independent of the volatility 
level. To explain this, Christoffersen said the following :“There are low volatility days with a steep 
volatility slope as well as a flat volatility slope, and also high volatility days with steep and flat 
volatility slopes. A single factor stochastic volatility model can generate steep smirks or flat smirks 
at a given volatility level, but cannot generate both for a given parameterization. In a purely 
cross-sectional analysis, this is not a problem, because we can estimate different parameter values for 
the one factor model to calibrate the time-varying nature of the cross-section”. 
However, the use of  multiple cross sections of options contracts by a one factor model has a structural 
problem. If its parameters are adapted to explain a slope of the smirk that is high on average over the 
sample, it will result in large model error on those days where the slope of the smirk is relatively flat,
and vice versa. 
Another way to understand this restrictiveness is that in a single factor stochastic volatility models, 
the correlation between variance and stock returns is constant over time, and this limits the model’s 
ability to capture the time variation nature of the smirk. 

The paper of Christoffersen, Heston and Jacobs (2009) introduce a straightforward way to incorporate a 
stochastic correlation by using multiple stochastic volatility factors. They demonstrate that two factors 
models have much more flexibility in controlling the level and slope of the smile (and the smirk). They 
also showed that additional advantage is that two factor models also provide more flexibility to model 
the volatility term structure. 

In order to provide more insight into the differences in pricing performance, we test an extension of 
the double Heston model. We formulate the idea to add jumps to the dynamic of the stock. During our research 
we also notice that Bates (2000) had conducted an extensive empirical analysis of a large class of option 
pricing models using S&P500 futures option data in the nineties. Among other things, he compares the performance of stochastic volatility models with the performance of stochastic volatility models augmented with Poisson-normal jumps. He evaluates the empirical performance of a two-factor stochastic volatility model, and investigates whether jumps and additional stochastic volatility factors are substitutes. Bates concludes that stochastic volatility models cannot reconcile return data and option data, even with two stochastic volatility factors, and that jumps are needed. That make our idea of adding jumps more valuable 
and we will see it during the numerical analysis.



