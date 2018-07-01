[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

When comparing two different sets of distribution, it is usually preferred to visualize the data in **PMF (probability mass function)** which unlike histogram, PMF displays the probability for each value. This way, the difference of sample size will not be emphasized. 

In this exercise we're comparing *actual distribution of children <18* vs. *biased (class size paradox) distribution of children <18*.

*1. Plot the actual and biased distributions, and compute their means.*
```python
'''Please run on thinkstats2/code folder'''
import nsfg
import thinkstats2
import probability
import thinkplot

resp = nsfg.ReadFemResp()
actual = resp.numkdhh

pmf_actual = thinkstats2.Pmf(actual, label='actual')
pmf_biased = probability.BiasPmf(pmf_actual, label='biased')

thinkplot.Pmfs([pmf_actual, pmf_biased])
thinkplot.Config(xlabel='# of children', ylabel='Probability')
```

![alt text](https://github.com/ridhars/dsp/blob/master/statistics/pmf-actual-biased.png)

```python
pmf_actual.Mean(), pmf_biased.Mean()
```
(1.024205155043831, 2.403679100664282)
