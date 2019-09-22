[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

>> #dividing the births to use it later in the qurestion 
firsts = live[live.birthord == 1]
others = live[live.birthord != 1]



question here the first thing i did was to define a function to calculate cohen's d  


def cohen_effect(group1,group2):
   
   diff_mean = group1.mean() - group2.mean()
   
    var1 = group1.var()
    
    var2 = group2.var()
    
    len1 = len(group1)
    
    len2 = len(group2)
    
    grouped_var =(len1*var1 + len2*var2) / (len1 + len2)
    
    d= diff_mean / np.sqrt(grouped_var)
    
    return d 


cohen_effect(firsts.totalwgt_lb, others.totalwgt_lb)
-0.088672927072602
with a negative cohen's d this indicates that the second group will have a negative effect on the group 
