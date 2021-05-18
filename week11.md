The visualization research paper I found this week is called Mapping Color to Meaning in Colormap Data Visualizations, found at: 
https://ieeexplore.ieee.org/abstract/document/8454346?casa_token=wcdFGIU4IxgAAAAA:W3YDJkGZP85MxAuhrdQAcujmWINvspHcz7YzmW_-ZAeNyWthLC__3u6YYR6sApE4S9zI6zrQ

Color is special, it brings out certain qualities in a vis, it distinguishes properties and helps users understand.
This paper is awesome because it goes into exactly how that happens. 
They investigate how inferred color-quantity mappings for colormap data visualizations were influenced by the background color.
There are certain biases that come with color because it can affect the users' perception differently, and they find that opacity is a big factor in how vis is interpreted.

The results primarily show that background color only matters if the color map varies in opacity, and inferred mappings contain what is considered an "opaque-is-more" bias.
If there is no variation to opacity, the mappings are dominated by "dark-is-more" bias.

My favorite part of the paper was actually learning about dark-is-more, contrast-is-more, and opacity-is-more biases, and I'll be sure to keep these concepts in mind for future visualizations.
"Conventional" lightness-bases choropleth maps were easier to interpret and they also reference a study that had participants interpret mappings on different backgrounds.

Overall, this group's goal was to understand when background color influenced inferred color-quantity mappings for colormap data.
Because all of the previous research this concept has a lot of conflicting conclusions. 
However, they seemed to clarify a lot of confusions that background color only really influenced users when the mappings had variations in opacity, which ultimately makes a good amount of sense. 
