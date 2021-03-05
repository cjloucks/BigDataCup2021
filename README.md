# BigDataCup2021
Hockey Passer Rating (HPR)

Tyler Allan, Marc Doucette, Connor Loucks, Christian Petrozza

What do you want to get out of your hockey related metrics? Are you looking for more information on goals, goal scoring, saves? Hockey as a sport actually has a long history of quantifying goals/saves and the events which can lead to either occurrence. But virtually all of the readily available research on the subject focuses on goals/saves and very little else. This is a stark realization to make as scoring plays in hockey though hugely important and of course decide who wins and loses the game, tell us very little about the litany of events that encompass the game of hockey.

Our analysis was based on Stathletes tracked data on the Erie Otters from the 2019-2020 season from which we pulled the following summary statistics:

pass attempts per game = 816.70
completed passes per game = 594.45
shot attempts per game = 122.18
shots on goal per game = 56.73
goals per game = 7.33

Clearly passing plays represent a significantly larger proportion of the total events that happen on the ice than goals, shots, or even shots attempts. 

Of course the current trend within the hockey analytics community is to build robust expected goals models which can and do successfully take into account a litany of factors impacting the end result of the play. These can include the level of traffic between shooter and net, type of shot, type of pass, angular information, and situational anecdotes. These models and the techniques that make them a reality (Bayesian, Machine Learning, etc..) do a very good job of contextualizing what goes into scoring and can tell us a lot about the share of offense throughout a game, they do not however help us break down specific components of a player's game for strategic purposes such as his specific passing ability. 

Why is this important? Our goal from the outset of this project was to deliver meaningful insights to a scouting staff or hockey operations team broadley which could be used to both improve team strategy and assess player performance for teaching and strategic purposes. By modeling a version of the NFLs traditional passer rating formula, we are able to take into account more factors that go into creating offense than the traditional assist while also focusing on all passing plays as opposed to the two passes that proceed a goal or even shot assists for that matter. A key takeaway from our analysis is to indicate the areas of the ice where players excel at moving the puck compared to average, and those where they do not in order to drive success for the Erie Otters, or any hockey club.  

For the next steps of our analysis, we will consider alternative approaches to assigning passer ratings to players that can take into account more factors, such as passing distance, passing type, and of course situation. Currently our model still overvalued offensive impact and thus forwards are potentially unfairly boosted above their defensive counterparts who have to do significantly more puck moving/playmaking in their own zone, an essential part of starting the offensive attack. 

The meat and potatoes of our actual coding is based around; isolating individual possessions rather than goals/shots/passes etc, creating logical variables for contextual information on a given pass such as proximity to a shot attempt, and of course significant iteration was done to create a final table of variables we deemed important to assess passing prowess and for use in our final formula. 

We hope you enjoy the work which we have produced, we certainly enjoyed the process on our end. We look forward to taking this project to the next level with your feedback. 
