[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

Exercise 1   In the BRFSS (see Section 5.4), the distribution of heights is roughly normal with parameters µ = 178 cm and σ = 7.7 cm for men, and µ = 163 cm and σ = 7.3 cm for women.
In order to join Blue Man Group, you have to be male between 5’10” and 6’1” (see http://bluemancasting.com). What percentage of the U.S. male population is in this range? Hint: use scipy.stats.norm.cdf.

>> import scipy.stats

>> mu = 178

>> sigma = 7.7

>> dist = scipy.stats.norm(loc=mu, scale=sigma)

>> low = dist.cdf(177.8)    # 5'10"

>> high = dist.cdf(185.4)   # 6'1"

>> print(low, high, high-low)

>> (0.48963902786483265, 0.8317337108107857, 0.3420946829459531)
