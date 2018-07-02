[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

Apart from histogram, PMF, & CDF which are based on practical observation (known as empirical distributions), there is a mathematical alternative known as analytic distributions. This distribution can be used to model empirical distribution, commonly by using mathematical CDF function.  
  
In this exercise, given *mean* & *standard deviation* of a normal height distribution, percentage of population with certain heights can be determined by utilizing CDF (which accumulates all probabilites up to certain value)

*distribution of heights is roughly normal with parameters µ = 178 cm and σ = 7.7 cm for men, and µ = 163 cm and σ = 7.3 cm for women.
In order to join Blue Man Group, you have to be male between 5’10” and 6’1” (see http://bluemancasting.com). What percentage of the U.S. male population is in this range? Hint: use scipy.stats.norm.cdf*

```python
import scipy.stats
mu = 178
sigma = 7.7
height_max = 185.4
height_min = 177.8

CDF_max = scipy.stats.norm.cdf(height_max, mu, sigma)
CDF_min = scipy.stats.norm.cdf(height_min, mu, sigma)

CDF_max-CDF_min
```
34% of male population is within the range 177.8 cm & 185.4 cm


