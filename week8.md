[When (ish) is My Bus? User-centered Visualizations of Uncertainty in Everyday, Mobile Predictive Systems](https://idl.cs.washington.edu/files/2016-WhenIsMyBus-CHI.pdf)
===
Jyalu Wu

Paper Summary
---
In this paper, Matthew Kay, Tara Kola, Jessica R. Hullman, and Sean A. Munson describe how they developed several candidate ways to visualize the uncertainty of when a bus will arrive at a given bus stop, all on mobile devices. In many predictive apps (weather, transportation arrival times, etc.), a point estimate is given because it is easy to read and understand in the short amount of time it takes to glance at your phone screen. However, real-world events can be unpredictable and when an app is wrong, the user can lose their trust in it. Thus, there is a big need for uncertainty visualizations in a way that's easy to understand.

After conducting a literature overview and surveying users of an existing bus app, the authors had the following design requirements:
- Point estimate of time to arrival
- Probabilistic estimate of time to arrival
- Probabilistic estimate of arrival status
- Data freshness

They considered multiple uncertainty visualizations in their design process, including *quantile dotplots*, which are made from drawing samples from a Normal distributed probability density using the quantile function (inverse CDF).

![quantile plots](screenshots/quantile-plots.png)

Eventually, they settled on 4 designs: the original density probability plot, a dotplot with 20 dots, a dotplot with 100 plots, and a stripeplot.

![final candidates](screenshots/final-candidate-vizzes)

One of their biggest findings was that discrete outcomes work best in small numbers. For example, dotplot-20 was much better than dotplot-100 because the variation in the dots didn't look as continuous. 


Thoughts
---
I read this paper for background information for my group's final project. This experiment reminded me a lot of A3, when we tried to see which viz out of 3 candidate ones was easiest to read. However, the authors of this paper did not choose the best visualization in the end, nor did they rank the candidate vizzes in their conclusions, though the quantile dotplot seemed to be easier to read since users were more precise when reading it.




Paper Citation
---
M. Kay, T. Kola, J. R. Hullman, and S. A. Munson, “When (ish) is my bus? user-centered  visualizations  of  uncertainty  in  everyday,  mobile  predictive systems,”  in Proceedings  of  the  2016  chi  conference  on  human  factors  in computing systems, 2016, pp. 5092–5103.


