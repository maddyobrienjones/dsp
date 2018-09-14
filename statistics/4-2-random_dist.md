[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

```python
import math
import numpy as np
import random
import thinkstats2
import thinkplot

randomlist = [random.random() for i in range(1000)]

random_pmf = thinkstats2.Pmf(randomlist)
thinkplot.Pmf(random_pmf)
thinkplot.show(xlabel='number', ylabel='probability')
```

``` python
random_cdf = thinkstats2.Cdf(randomlist)
thinkplot.Cdf(random_cdf)
thinkplot.Show(xlabel='number', ylabel='CDF')
```

> The distribution does seem to be uniform. The PMF seems to show that the probability is uniform for each number in the list. The CDF is not a completely straight line but it does look to almost have a perfect slope of 1. 
