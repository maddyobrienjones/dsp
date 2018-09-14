[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

```python
import math
import numpy as np
import nsfg
import thinkstats2

preg = nsfg.ReadFemPreg()
live = preg[preg['outcome'] == 1]
print(live.head())

first = live[live['birthord'] == 1]
others = live[live['birthord'] != 1]

effect = thinkstats2.CohenEffectSize(first['totalwgt_lb'], others['totalwgt_lb'])
print(effect)
```

>> The effect size of birth order on birth weight is -0.089. This is slightly more significant than the effect size of birth order on pregnancy length (0.029). This effect size means that the average difference in birth weight is 0.089 standard deviations.
