## Week 10

The research article I've found for this week is located here, DOI: 10.1109/VISUAL.2002.1183821 , link: https://ieeexplore.ieee.org/document/1183821

I thought this article was particularly interesting because the researchers explore techniques for visualizing flow structures efficiently to avoid problems regarding the industrial applications (vortex rope of a water turbine).

## Discussion

It is difficult to come up with new ways for visualizing moving particles, especially to express information in a meaningful way. Many ways that people want to express this data is with path lines, but that should be reserved for static visualizations, leaving us with streak lines (discretized into a series of particles).
This data is time-sensitive, therefore the vis has to be constrained to a region of flow in order to remain informative, else the data would lack detail.
One approach this team uses is to randomly spread particles so they can present a uniform density rather than showing patterns and clusters. 
I was interested to read about the inkling of using 3D textures to visualize flow, but unfortunately the team did not delve into this topic due to lack of hardware support and loading time issues.
They mention the need for injecting new particles into the vis during the time evolution, which is a common problem for particle-based flow visualizations, especially sinec the goal is to maintain a uniform density.


Section 2 of the article focuses on flow regions of interest, but I would like to dive straight into section 3 which actually explains their visualization technique.
In order to visualize their regions of interest within vortex tubes, the team thinks about visibility, particle seeding, particle tracing, conservation of mass, and particle rendering, to achieve smooth fading of particles, medium particle density, and a random distribution of particles. I found that the most interesting parts to this research were conservation of mass and particle rendering.
They found that 1-5% of mass is "numerically lost" due to trilinear interpolation of node data, but that this loss can be reduced using a dual grid, so they decide to use special interpolation only in cells next to solid boundaries because this is where most numerical error occurs, so this error can be reduced.
For particle rendering, they show two examples, rendering spheres and the alternative of streamlets, which interestingly gives the illusion of 3D vis rather than a flat object. 
I found this most interesting because even though the team decided against 3D texture vis in the beginning, ultimately they came up with a non-obvious technique to give a similar illusion.

All in all, this article was slightly confusing, especially when they got into details about turbines and velocity  data, but I really enjoyed learning about the experiment. 
It was especially nice to read about the techniques they chose and why, because even if I don't know a lot about vortex ropes, I was able to visualize the flow of water through one.

The image below is taken from this paper and show the use of streamlets.
![image](week10.PNG)
