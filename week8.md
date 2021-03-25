# CS 582 Data Vis Week 8 Reflection
Matthew St Louis

## When (ish) is My Bus? User-centred Visualizations of Uncertainty in Everyday, Mobile Predictive Systems
- [Source](https://dl.acm.org/doi/abs/10.1145/2858036.2858558?casa_token=xSejIUyOf0kAAAAA:SuvG-fQag9BWPgIxoqUKbPvX7orOoF_QivmqG8fQTIRXz6u3FM2x7lO27R5bRhjTomnG9trC47Pg)
- [PDF Link that was accessible from Google Scholar](https://dl.acm.org/doi/pdf/10.1145/2858036.2858558?casa_token=ImjmCt6U9UMAAAAA:4Nt24yNH7ETmU7SIwcTjC0311mDDqEk2okpu9bUookYyfV_nca_hUVNHVETmjJbw7OLpzVrs3COy)

### Summary
This week I read a paper by Kay, Kola, Hullman, and Munson on designing a visualization for a mobile app that gives information on bus schedules. The app (OneBusAway) gave point estimates for when a bus would arrive on a given route. The problem that the researchers identified is that this point estimate may not give users enough information about the uncertainty in bus arrival time to make conscious, informed decisions. Their goal is to effectively communicate this uncertainty on a mobile display so that users in a hurry can read it without extensive training.

The researchers begin with an interesting assessment of their problem space. They survey the app's existing users about how they use the app and what features and tasks are most important to them. From this survey, they came away with five highest-rated questions for their visualization to answer:

- When should I start walking toward my bus?
- If I leave now, how long will I have to wait at the bus stop?
- If I missed my bus, how long will I have to wait for the next one to come?
- Will I get to a meeting/event on time despite bus delays?
- Will I have enough time to do ___ before the bus arrives?

From these requirements, the researchers begin ideation for potential mobile visualizations to convey this information. They use sketching and paper prototyping before creating digital mockups of the best designs. One interesting consideration that they seek to incorporate into their design is the idea of a _glanceability/false precision tradeoff_. They want to make a design that still incorporates a glanceable point estimate, as this was found important to the app's users, but they did not want to make the point estimate so prominent that the uncertainty data would be overlooked. The team also considered displaying the probability that a bus has already left, but this ended up being redundant to the probability distribution for arrival times.

The final experiment tests three types of visualization to communicate the probability distribution of bus arrival time. The first is a density plot, which effectively plots the probability distribution function. The second is a stripeplot, which uses bars to represent different quantiles of the probability distribution function. The third is a novel visualization the authors created for this project that they term a __quantile dot plot__. The quantile dot plot is a dot plot where a probability distribution is represented as a given number of dots where each dot marks where a certain quantile falls, and quantiles that map to the same value stack.

The experiment found that users performed best with a quantile dot plot, particularly with 20 dots rather than 100. They theorize that this is because the quantile dot plot is the most readable of the three methods, and that a quantile dot plot with fewer dots takes advantage of subitization, where users can quickly know how many dots there are without counting them if there are less than about five.

## Analysis

I found this paper really interesting and exciting. I found it by exploring papers that cite the Hypothetical Outcome Plots paper. I found HOPs fascinating and wanted to see where else dynamic visualizations could help summarize uncertainty. This paper provided a really interesting example of a problem that may be ill-suited to HOPs. The authors explain that HOPs take time to digest, and that time doesn't fit in with the glanceability needed to make an effective mobile app.

It's cool that the designers went through so much UX design to prototype their visualizations. Before they even began designing, they needed to understand the situation domain with user surveys of what to design for. It's interesting to read about them go through all of the steps for designing a visualization with paper prototypes and user feedback. They don't actually specify how much of the final prototypes are coded vs made with simplified design software.

I was surprised that quantile dot plots were a novel visualization designed by the authors of this paper. They are intuitive, concise, and informative. They seem particularly well-suited to compact displays such as the mobile app that is the authors' use case.

One thing I found notable is that there were a few users that the designers mention in the discussion who did not want uncertainty information in the app because they did not want enough information to make a conscious, informed decision. They feared that they may be responsible for the consequences of their decision and would rather be able to blame the app for being imprecise. This was fascinating and utterly bizarre to me. Their reasoning makes sense in a way, but it's really interesting to hear about users who want a less usable app. Although I don't agree with these users' lifestyle, it would probably make the app better overall to accommodate their preferences by allowing some option to show just the point estimate. I'm curious about other cases where some users may specifically want a less functional app for the sake of it being less functional.

Overall, this paper was a fun read and had some really interesting ideas. Designing visualizations for mobile apps that are meant to be glanced at while walking somewhere has such different requirements and constraints from designing visualizations for the web, and it's interesting to see what compromises and adaptations the authors make to make it work. One of the most interesting small details to me is that the authors chose to scale down graphs with tall peaks. This is because these peaks represent very certain and consistent arrival times, so less resolution is necessary for the user's purposes. This is a choice that would be entirely inappropriate in so many contexts, but it works seamlessly and efficiently in this one. This paper makes me curious about other practical domains that may wildly change what characteristics a visualization must have to be effective.