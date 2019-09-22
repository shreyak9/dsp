[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

>> REPLACE THIS TEXT WITH YOUR RESPONSE
in this question there are two variables  to consider the first one is numkdh(respondents) and the other one is the biased variable here i have calculated the pmf for to both these variables to compare them and then calculated the code as follows 
resp = nsfg.ReadFemResp()

pmf = thinkstats2.Pmf(resp.numkdhh, label='numkdhh')

thinkplot.Pmf(pmf)

thinkplot.Config(xlabel='Number of children', ylabel='PMF')

biased = BiasPmf(pmf, label='biased')

thinkplot.PrePlot(2)

thinkplot.Pmfs([pmf, biased])

thinkplot.Config(xlabel='Number of children', ylabel='PMF')

pmf.Mean()

biased.Mean()
