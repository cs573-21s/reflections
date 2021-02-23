# CS 582 Data Vis Week 3 Reflection
Matthew St Louis

## Hypothetical Outcome Plots (HOPs) Help Users Separate Signal from Noise
- [Source: UW Interactive Data Lab](https://medium.com/@uwdata/hypothetical-outcome-plots-hops-help-users-separate-signal-from-noise-870d4e2b75d7)
- Contents
  - [Summary](#article-summary)
  - [Analysis](#analysis)

### Article Summary

This week, I read a Medium post by the blog UW Interactive Data Lab about summarizing noise and trends through animated images. The idea is to help a user tell what kind of trend noisy data is likely to have. The example scenario given was whether a given set of jobs numbers were more likely to signal economic stagnation or economic growth.

![Still Image of Economic Data](https://miro.medium.com/max/900/1*TH3fpOznbSe4rDOOlXGpKA.png)

The researchers presented some subjects with animated visuals that showed some potential outcomes for economic stagnation and economic growth, while other participants were given static graphs with error bars.

![Static Error Bars Experiment Setup](https://miro.medium.com/max/1260/1*a5ZmRtmZ1ipMxR2IGwjxMQ.png)

![Animated Experiment Setup](https://miro.medium.com/max/902/1*xyWUfvNxUygoKDiSfHSrrQ.gif)

The researchers found that the animated data helped participants make better calls about the data they were presented. They also found this same increase in effectiveness for reasoning about line graphs versus static line graphs and dynamic bars versus error bars or violin plots.

![Static Aggregated Lines](https://miro.medium.com/max/589/1*Y6u_bP1aN7hfdRcSClJ7Og.png)

![Animated Uncertainty Line](https://miro.medium.com/max/605/1*dkLIiMMTIFU8hkhDr5J6Pw.gif)

![Static Violin Plot](https://miro.medium.com/max/569/1*auBmaPfjWo0MmUnGu45Btw.png)

![Dynamic Bars for Violin Plot](https://miro.medium.com/max/599/1*iuRlIE2_jSkg-iP1ujdsMA.gif)

### Analysis
I found incredibly interesting that showing many examples of possible outcomes can help users understand a trend better than a static aggregate. It makes a lot of sense. Graphic representations of probability are so abstract and hard to hold onto, especially for people without a background in statistics who may not be able to read these plots. Visual frequencies are so much easier to hold onto and to interpret. The article talks quite a bit about how good our eyes are at aggregating simple visual data when presented with it in a way that feels natural, and these frequency graphs play to those strengths.

I've found that when I personally look at a graph of probability in a situation of chance where I'm hoping for a certain outcome, the fact that the graph has a physical representation of success, however slim, gives me more hope than it necessarily should. To use the violin plots as an example, if I were in a game of chance where I would win if the left bar were higher than the right using a draw from the given distributions, I think I would overestimate my odds with the static graph and assess them more accurately with the dynamic graph. I feel like the sheer area of the static graph gets in the way of emphasizing the relative heights.

The most interesting part of this dynamic method is how dead simple it is to read. It takes a bit of explanation for what the dynamic graph represents, but if a user understands what distribution it mimics, the visuals do so much of the heavy lifting. It relies so much on the brain's understanding of frequency and vision that it can offload a lot of explanation on the graph's part, in a way that transcends statistics backgrounds and language. I'd be really interested to see more examples of how frequency could encode uncertainty to help with decision making.