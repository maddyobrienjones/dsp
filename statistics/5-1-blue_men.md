[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> 5'10" = 177.8cm, 6'1" = 185.42cm

```python
import scipy.stats

heights = scipy.stats.norm(loc=178, scale=7.7)

min_height = heights.cdf(177.8)
max_height = heights.cdf(185.42)

print(max_height-min_height)
```
>> From the CDFs of the function at the maximum and minimum acceptable heights for the Blue Man Group, we can take the difference and figure out the percentage of men between the two heights. In this case, the answer is that approximately 34.27% of men are in the range where they could apply to be part of Blue Man Group.
