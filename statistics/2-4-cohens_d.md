[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

Cohen's d is one of the metrics used to quantify difference between two groups. In this exercise, Cohen's d is used to measure **weight** differences between two groups of babies.

```python
'''Please run on thinkstats2/code folder'''
import first
import numpy as np
import math
```

*1. Using the variable totalwgt_lb, investigate whether first babies are lighter or heavier than others.*

```python
live, firsts, others = first.MakeFrames()
firsts_meanw = firsts.totalwgt_lb.mean()
others_meanw = others.totalwgt_lb.mean()
others_meanw > firsts_meanw
```
Returns **True**, first babies are lighter than others

*2. Compute Cohen’s effect size to quantify the difference between the groups. How does it compare to the difference in pregnancy length?*

```python
thinkstats2.CohenEffectSize(firsts.totalwgt_lb,others.totalwgt_lb)
```
-0.089 (babies weight) vs. 0.029 (pregnancy length). Difference is relatively small.


