---
layout: post
section-type: post
title: Multiple plots per page
category: R 
tags: [ 'R', 'Plots' ]
---

if you need to plot different figure on the same page use the following syntax.


{% highlight R %}

par(mfrow=c(1,2))

plot(function(x) dnorm(x, 30, 15), -20, 80, ylab="Density", xlab="Size", col="dark green", lwd=2)

plot(function(x) dlnorm(x, log(30), 1.5), 0, 80, ylab="Density", xlab="Size", col="blue", lwd=2)

{% endhighlight %}


*mfrow* will create one row with two columns.

each time you call *plot* **R** will use one of the available columns. So, in the previous example, **R** will plot a normal in the first column and a lognormal distribution in the second column.

