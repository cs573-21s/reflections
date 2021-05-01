# CS 582 Data Vis Week 4 Reflection
Matthew St Louis

## Value-Suppressing Uncertainty Pallets
- [Source: UW Interactive Data Lab](https://medium.com/@uwdata/value-suppressing-uncertainty-palettes-426130122ce9)
  - [Paper](https://idl.cs.washington.edu/files/2018-UncertaintyPalettes-CHI.pdf)
  - [D3 Module](https://github.com/uwdata/vsup)

### Article Summary
This week, I read a Medium post by the blog UW Interactive Data Lab about using color pallets to represent uncertainty. They highlighted the challenge of encoding uncertainty into a visualization, especially when it needs to be done through the same channel as the statistic it's casting uncertainty on. A common use case for this is color on maps.

The article points out how it's common to encode the value as hue and its uncertainty as saturation in a grid of possible colors. The propose a cone-shaped pallet where more individual colors are given to areas of less uncertainty, and where areas of greater uncertainty are collapsed into fewer colors. This is meant to help overcome the tendency people have to overestimate the meaning of highly uncertain data.

The example they use to show this is data from the 2016 election.

![2016 Election Data Grid Pallet](https://miro.medium.com/max/914/0*jvcakoWkEDAiaScZ)

![2016 Election Value-Suppressing Uncertainty Pallet](https://miro.medium.com/max/887/0*kfu-tYcycdUcSHli)

### Analysis

I saw this article as a recommendation on my article from last week. It really stood out to me because the preview I saw only showed the first graph with the grid pallet. I was really interested in what they have to say because I thought that their map looked ineffective at best and misleading at worst. When I went to actually read the article, I found the value-suppressing uncertainty pallet's effect shocking. The map looks so much more informative and interesting. It really bothers me when visualizations will try to color the tilt on tossup states for elections because it's very difficult to reason about as a consumer. My brain wants to look for red, blue, and purple, and it's mentally exhausting trying to filter out everything below a certain saturation when there are four different hues to consider. I personally find the value-suppressing uncertainty map to be much easier to process. The paucity of uncertain colors makes them much easier to filter out when looking for decisions, and the remaining colored sections are more informative. The bottom half of the grid pallet is so noisy, and taking the colors out where they don't mean much really helps make the graph readable.

I think it's a really interesting idea to question where more colors are needed to provide greater detail and where they only serve as noise. I haven't thought about it too much, but I previously assumed that grids would be the most fair way to represent scales like this so that every potential mapping of the grid would be covered evenly, but removing some of these colors to represent uncertainty makes a lot of sense. In the future, I'll think more critically about how best to distribute the resources of a channel across the data to show.