# CS 573 Week 11 Reflection
Matthew St Louis

## In Pursuit of Error: A Survey of Uncertainty Visualization Evaluation
[Source](https://doi.org/10.1109/TVCG.2018.2864889)

This week I read a really interesting meta-analysis of different uncertainty studies by Jessica Hullman, Xiaoli Qiao, Michael Correll, Alex Kale, and Matthew Kay. They start by discussing the importance and difficulty of studying uncertainty. As a growing number of sectors rely more and more on data collection for problem solving, decision-makers may not be able to separate the signal from the noise in their data. Uncertainty visualizations can help this, but the research effort around uncertainty visualization is fractured and disparate. Different research teams have different ideas of what aspects of uncertainty visualizations are important. This paper (Hullman et al.) seeks to create a unified taxonomy framework in which to analyze uncertainty visualization studies. The end goal of this is to allow more rich discussion around uncertainty visualization and to make future visualization uncertainty research more productive and thorough.

The taxonomy that the researchers design has six levels:
- __Behavioral Targets__: The studied impacts that the uncertainty visualizations have on behavior
- __Expected Effects__: How a study defines the success or failure of an uncertainty visualization
- __Evaluation Goals__: Study design (e.g. uncertainty vs uncertainty, uncertainty vs point estimates, something else)
- __Measures__: Directly elicited measures and derived measurements
- __Elicitation__: How users' responses were gathered
- __Analysis__: How an evaluator uses responses to determine if the expected effects were achieved.

The researchers designed flow diagrams to show the different evaluation paths that different studies took through this taxonomy. It's interesting how chaotic this diagram looks and how well this diagram highlights how differently different researchers conceptualize uncertainty and how to study it. 

After describing some of the paths through this diagram, Hullman et al. make a series of recommendations for how to study uncertainty better. One that is so easy to implement that I'm surprised it wasn't standard earlier is to include a text-based baseline to compare to the uncertainty visualization. Another proposal is that more studies should test how well an uncertainty visualization helps with users' decision-making, as this is currently far more rare than assessing how readable the visualization is. Hullman et al. also discuss an interesting effect they observed in user confidence that they termed the "hard-easy effect": people are over-confident on very hard uncertainty tasks and under-confident on very easy uncertainty tasks. This is a bit counterintuitive, but it sort of makes sense because data can sometimes be so hard to interpret accurately that the responsible decision can be not to make one. That leads into another recommendation: researchers should allow participants to express that they do not feel they have enough information to make a decision based on an uncertainty visualization.

These recommendations and so many more that the paper make are fascinating and invaluable. My final project team is doing work on uncertainty, and we definitely plan to incorporate at least some of these recommendations into our final project. This gives us a well-defined framework within which to work and make informed, conscious decisions. This paper was an ambitious effort to create a standard for the disparate uncertainty visualization community to rally behind, and I hope that it catches on, allowing for more thoughtful and comprehensive research.