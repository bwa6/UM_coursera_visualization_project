# UM_coursera_visualization_project
Final course project: create a visualization based on sports near Ann Arbor, Michigan

In this notebook, I combined three datasets (links in notebook) relating to: <br>
1) all players drafted in the NFL <br>
2) all players drafted in the NFL that attended University of Michigan <br>
3) geographic data of the top 1000 cities in the U.S. <br>
<br>
I cleaned the datasets of nfl teams that are no longer around and players with missign values for their birth states.  I determined the geographic distances in kilometers of each of the top 1000 cities from Michigan.  I then averaged the cities within the same state to get an approximate distance of each state from Michigan.  For Hawaii and Alaska, I reduced their distance to that of California to remove large outliers in plots.  I cleaned the datasets so that I could merge the values based on both name and draft team (since there are multiple people with the same name).  I added features for the distance from Michigan of the player's birth state and the state of the NFL team that drafted the player.
<br>
<br>
I am interested in the hypotheses that 1) a player is more likely to attend University of Michigan if they were born closer to Michigan, and 2) NFL teams closer to Michigan are more likely to draft players from the University of Michigan since their scouting network will be more robust closer to their facilities.
<br>
<br>
I developed a visualization with four plots.  The top plots show scatter plots of players based on the distance from Michigan of their birth state and the state of the team that drafted them.  Plots on the left are for players that attended University of Michigan (the color scheme matches the colors of University of Michigan).  Plots on the right are for players that did not attend the University of Michigan.  The size of the markers correspond to the number of players that were born in the same state and drafted by a team in the same state.  These top plots are very informative but also quite dense.  To improve interpretability, I included the bottom plots.  These plots show the density of players in four quadrants of the plots in the top row.  Importantly, a user can interactively click on a location to adjust the quadrants.  This is a useful tool to compare the plots of players that did vs. did not attend the University of Michigan.
<br>
<br>
For example, a user can click on the point: (750, 0) and see that the left side of the left plot contains 58% of players while the left side of the right plot has only 48% of players.  Indeed, this agrees with the hypothesis that teams are biased towards selecting players that are closer to their facilities.  Furthermore, a user can click on the point: (0, 1000) and see that the bottom of the left plot contains 77% of players while the bottom of the right plot has only 41% of players.  This shows quite a large bias of players attending University of Michigan if they were born closer to Michigan.
<br>
<br>
This notebook demonstates a dense, interactive visualization that offers an opportunity to explore other potential hypotheses and provides a framework to potentially explore similar analyses with other schools or add other features to explore, such as player position, what number they were picked in the draft, etc.
