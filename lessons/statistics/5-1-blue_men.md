[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

>> mu = 178
sigma = 7.7
dist = scipy.stats.norm(loc=mu, scale=sigma)
type(dist)
A normal continuous random variable. ?
dist.mean(), dist.std()

low = dist.cdf(177.8)    # 5'10"
high = dist.cdf(185.4)   # 6'1"
low, high, high-low
(0.48963902786483265, 0.8317337108107857) => these are the values we get for 5'10 and 6'1 respectively converting these values to percentile  = 0.48.. * 100 = 48th percentile and 0.83*100 = 83 rd percentile now the percent of people born between 5'10 and 6'1 is    
83 - 48 = 35% of people between 5'10 and 6'1 
