---
layout: post
section-type: post
title: Plotting distributions
category: R
tags: [ 'R', 'Plots' ]
---

In case you need to plot distributions using R, the following code should do the trick.

{% highlight r %}

plot(function(x) dnorm(x, 30, 15), -20, 80, ylab="Density", xlab="Size", col="dark green", lwd=2)

{% endhighlight %}

if for some reason you need to change the scale of the x axis:

{% highlight r %}

plot(function(x) dnorm(x, 30, 15), -20, 80, ylab="Density", xlab="Size", col="dark green", lwd=2, xaxt="n")

axis(side=1, at=seq(-20,80,20), labels=(seq(-20,80,20)))

{% endhighlight %}

the sequences used for *at* and *labels* need to be of the same lenght.

