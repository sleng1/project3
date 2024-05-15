# project3
<iframe src="visualization.html" width="1100" height="750"></iframe>\

  Perhaps being quite an opportune time amidst this year’s NBA playoffs, the dataset we selected to base our interactive visualization off of was a large, statistical database of the ongoing 2024 playoffs consisting of all the quantifiable metrics used by the league office to record individual player activity. This dataset was of considerable size with over 200 rows and 20 columns and contained all the relevant statistics perused by basketball fanatics to judge player performance.\

	As we intended on performing a rigorous EDA on the dataset to identify trends and correlations between certain variables, we soon noticed that we already had much familiarity with the data on-hand as we all watch basketball and frequently browse references containing the same statistics. As we were certainly aware of basic positive relationships in data such as higher shooting percentages being correlated with more wins, we wanted to use our interactive visualization to explore variables that didn’t immediately have apparent trends between them. That is why the intention for this interactive visualization was to explore how the variables of “Average Plus-Minus Per Game”, “Average Fantasy Points Per game”, “Points Per Game”, and “First Round Exits” measured up against each other.\
 

For some basic background, the statistic of “Average Plus-Minus Per Game” records the average, absolute difference in the amount of points scored by the team when the player is on the floor and by the opposing team when the player is on the floor. If this value is positive, that means the team the player is on outscored the opposition when the player was playing; otherwise goes the opposite way. The “Average Fantasy Points Per game” is a contrived number created by gaming websites to assign point values to players in a trading card-esque game where spectators of the sport attempt to gather a roster of as many virtual instances of players to play against their friends. When this number is high, the player performed well; low, not so much. Points per Game and first round exits are numbers that are quite self-explanatory. The rationale behind our selection of these features mainly can be attributed to our curiosity in the visual spacing between these variables as it was not immediately apparent.\

“Would higher plus-minus equate to higher fantasy points?”\

“Not always because role players who perform vital roles in a backseat position may not have higher individual statistics.”\

This was a conversation we had in our initial stages and although we all came to a conclusion on uncertainty, we were interested in spatially mapping out the data and utilizing interaction to further anatomize the qualities.\

After scraping the dataset from the web and performing the necessary cleaning procedures in regards to formatting, we filtered out the first three of our relevant columns and applied a function using the “teams” column of each row to add additional data about whether the player was on a team that lost a series in the first round.\

To describe the design choices we made for our visualization, we decided to create a scatter plot of the individual data entries (players) and map each observation to a correctly scaled point on the plot. We decided a circle would be the best visual encoding for our purposes as we wanted to create a mapping between the radius of each circle and the “Points Per Game” statistic for each player with a larger circle corresponding to a higher PPG value. As already at this stage of the design, much insight was unearthed about the relevant data, and adding the interactive elements further complemented the visualization as we focused on brushing and details on demand to emphasize the features of each point. Hovering over each data point reveals a box containing all the individual statistics we left out of our axis and hovering over a certain value in the ‘first round exit” key blurs out all the data points of the other value in the plot. The reason behind why we focused quite solely on details on demand for our visualization was because we believed interaction would be most effective at supplementing the existing encodings of the visualization and carrying the additional columns of the original dataset we did not deem most relevant to our exploration. A viewer of our visualization would first be engrossed by our static communications of the data fields and then when interested in further information such as who each value represents would then be met with the interactive qualities containing the answers to all those questions.\

Speaking on how we worked as a team, us three members truly contributed to every part of the project and were instrumental in coming to a consensus about all the design choices. In terms of how long we spent on the development process, we spent about <10 hours in total but in reality, much of that time was us messing around with the stats while watching the games. The actual time spent developing the application was much shorter (2-3 hours).

