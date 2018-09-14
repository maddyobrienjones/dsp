[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

```python
import math
import numpy as np
import thinkstats2
import thinkplot
import nsfg

resp = nsfg.ReadFemResp()
pmf3_1 = thinkstats2.Pmf(resp['numkdhh'], label = 'numkdhh')
thinkplot.Pmf(pmf3_1)
thinkplot.show()

def BiasPmf(pmf, label):
    new_pmf = pmf.Copy(label=label)
    
    for x, p in pmf.Items():
        new_pmf.Mult(x, x)
        
    new_pmf.Normalize()
    return new_pmf

biased = BiasPmf(pmf3_1, 'numkdhh')
thinkplot.Pmf(biased)
thinkplot.show()

print(pmf3_1.Mean()) #1.024205155043831
print(biased.Mean()) #2.403679100664282
```
> In comparing the biased and unbiased distributions, there is clearly a large difference. In the unbiased, the mean number of children per household is around 1, while in the biased distribution, it is around 2.4. 
