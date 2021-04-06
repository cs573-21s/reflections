# CS 582 Data Vis Week 9 Reflection

Matthew St Louis

## The Effect of Uncertainty Visualizations on Decision Making in Weather Forecasting
- [Source](https://journals.sagepub.com/doi/pdf/10.1518/155534308X284354)

For this week's reflection, I wanted to read through a paper that relates to one of the ideas my team is considering for our final project. We are considering trying to visualize the uncertainty in precipitation to help people make decisions and pitting different visualizations against each other to see which is most effective.

The goal of this paper is to compare different methods of visualizing uncertainty in wind speed data. Participants were presented with box and whisker plots and maps showing the median case, worst case, and variability of wind speed in different areas. I initially thought that this study would be more interesting, but the maps were designed pretty terribly. They used a hue-based color scale to encode all values on the maps, which is not nearly as readable as a saturation- or luminance-based color scale. 

The researchers found that participants were more accurate and consistent when using the box and whisker plots. The color maps meanwhile made participants more aware that there was uncertainty and less confident in their decisions. They reported that the color maps were harder to read precisely. This makes a lot of sense and would be expected with something as ugly and unusable as the color maps they chose.

My takeaway from this paper is that it is not enough to make the user aware of the uncertainty that exists in a problem. I find it really interesting that uninformative design like the maps makes users more aware of the problem by giving them insufficient tools to reason past it, while a more informative design that makes the problem more manageable makes the problem itself less noticeable. It's interesting to think about how much attention should be brought to the difficulty or weight of the problem a vis is trying to solve. One parallel I see is from the paper I looked into last week, When (ish) is my bus?. They noted a tradeoff between "glanceability" and informative design. If they made the point estimate stand out too much, the researchers were afraid that the visualization would go ignored. It's interesting to think that uncertainty research aims to increase awareness of the problem of uncertainty, but that it should check that this isn't being accomplished through obfuscation. If my group goes with an uncertainty-based visualization, we will take this into account.

It's interesting to me how little this paper deals with visualization theory. It makes sense that being an older paper, there was less interesting visualization literature from which to draw. Next week I'll try to find something more recent, novel, and notable.