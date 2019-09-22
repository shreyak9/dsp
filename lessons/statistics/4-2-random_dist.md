[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

>> 
the first thing we do here is to use random.random to generate numbers 

z = np.random.random(1000)

then we make a probability mass function graph to check the proability of each variable 

next we plot a cdf function of the random numbers (z) 


cdf = thinkstats2.Cdf(z)
thinkplot.Cdf(cdf)
thinkplot.Config(xlabel='Random variate', ylabel='CDF')
  
  
  what we get from both these graphs that the numbers are truly random ,What  figure(cdf) shows is that 10% of the sample is below the 10th percentile, 20% is below the 20th percentile, and so on, exactly as we should expect.
