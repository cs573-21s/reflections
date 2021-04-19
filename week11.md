Reflection 11
===
    
link:http://diglib.eg.org/bitstream/handle/10.2312/eurovisshort20161168/097-101.pdf    

When we program, sometime we will lose ourself in the massive code. To solve this problem, author of this paper wants to present the characters of relationships and hierarchies of source code through tree map. Author choose Icicle tree to visualize source code hierarchies’ character as it portrays the structure of a hierarchy through juxtaposition, which is more suitable for overview visualizations.      
<img src="11-1.png">   
<br>
Although the way how to generate Icicle tree map have not been detailed explained in paper, we can still have an overview of what it looks like.     
<img src="11-2.png">   
<br>
On the right side is the source code writing by html 5 and left side is its structure shown by Icicle tree map. To figure out whether Icicle tree map is helpful to people to understand source code’s hierarchy. the question in experiment can be categorized into two types, which are counting and locating, The questions are looked like, How many child/descendant/leaf nodes does node “X” contain and what node is the closest common ancestor of nodes “X” and “Y” .     
<br>
The result shows that text editor with Icicle tree map visualization has a higher accuracy than text editor without visualization. The author explain that the possible reason is that visualization fundamentally encodes structural elements of source code making them easier to count.      
<br>
However, the result of locating is quite surprise us. Accuracy seemed to decrease when the overview visualization was present. This is an interesting finding, as it suggests that using an inappropriate visualization can actually have a detrimental effect on task performance, while at the same time giving participants false confidence that they are performing well.   
<img src="11-3.png">   
<br>
This paper is interesting for me. I learned that Icicle tree map is suitable to encode the hierocracy character as it portrays the structure of a hierarchy through juxtaposition and have more information density than the standard tree map. The idea of encode hierocracy character of source code using tree map is also innovative. I am looking forward this technology can be used in our daily life one day.
