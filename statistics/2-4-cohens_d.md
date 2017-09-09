[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>> My answer is `-0.088672927072602`. So first born will weigh slightly less than others. Code is below.

```python
import nsfg
import thinkstats2

preg = nsfg.ReadFemPreg()
live = preg[preg.outcome ==1]

firsts = live[live.birthord == 1]
others = live[live.birthord != 1]

diff = thinkstats2.CohenEffectSize(firsts.totalwgt_lb,others.totalwgt_lb)
print(diff)
```
