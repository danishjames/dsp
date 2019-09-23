[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

Exercise 4   Using the variable totalwgt_lb, investigate whether first babies are lighter or heavier than others. Compute Cohen’s d to quantify the difference between the groups. How does it compare to the difference in pregnancy length?

Code below: 
>> CohenEffectSize(rich.parity, not_rich.parity)


>> This gives a value of -0.1251185531466061, which would put the effect at around 10 times the effect of the difference in pregnancy length.
