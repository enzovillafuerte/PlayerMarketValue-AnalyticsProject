# PlayerMarketValue-AnalyticsProject

*See report for complete imformation*

Data Analysis

Since we are trying to predict market value of a player, it is relevant to start with some of the features that may have some importance to the target feature. A good starting point would be to see if there is any difference in market values by league. Given my domain knowledge, even though La Liga had arguably the strongest two teams for a long time (FC Barcelona & Real Madrid), the English Premier League (EPL) had elite players spread across different teams, given its bigger audience, reach and the money being invested by Arabic enterprises and millionaires that allow many clubs to invest heavily in their squad. Other factors such as the arrival of elite coaches such as Pep Guardiola or Jurgen Klopp, and their strong and offensive sporting projects also contributed to better performance, spectacle, and therefore an increase in revenue.

<img width="468" alt="image" src="https://github.com/user-attachments/assets/7ba9945a-7026-43f2-87cb-7d79957a0c31">

As depicted in Figure 1 and correctly inferred, the average market value of EPL players is considerably higher than those of their counterparts. Additionally, the more we aggregate our players, for instance by aggregating based on the TOP 20% for each league, the smaller the gap appears to be, but not considerably, which aligns with my initial empirical hypothesis.
Regardless of the reasons why this happens, I am interested in knowing what are the performance characteristics of those players with higher market values within each league. 
As stated initially, the data was gathered to contain players in midfield and attacking positions. Therefore, I’m interested in analyzing what areas of the pitch are those high value players occupying.

<img width="468" alt="image" src="https://github.com/user-attachments/assets/46eee6e9-3493-4594-937b-424b28fbd2b3">

By looking into Figure 2, we clearly visualize that Left-wingers have the highest average market value, by a considerable margin of about $4M with respect to the other positions. Many great players and known ‘ballers’ have played in this position in the latest years. Some of the most prominent ones from the 2000s decade include Ronaldinho, Robinho, Ribery, Henry, etc. These players tend to be a total spectacle on the pitch given its production ability, but most importantly their progression skills such as dribbling and pace.
Surprisingly, defensive midfielders also rank high. Defensive midfielders are probably the most misunderstood players out there, but they are super important for the overall compactness of a team. They don’t only have to offer the linkage between defense and attack in possession and progression, but also have to be the sweepers and the stoppers defensively speaking, in a position in which stakes are high and there is usually little time and space to maneuver. 

Right wingers, attacking midfielders and center forwards also follow along very closely. Since we are already diving deep into the exploration, let’s visualize the players with the highest value for a random year in our dataset.

<img width="389" alt="image" src="https://github.com/user-attachments/assets/139b6174-832a-4cbc-bc77-4d1e79166a87">

In the year 2019, a 27-year-old Neymar Jr was the player with highest valuation in the market with a worth of $175M, followed by Eden Hazard and Lionel Messi. Two years earlier (2017), PSG had broken the market with the acquisition of then FC Barcelona’s Neymar, for a total price of $263M, and he became the face of French football. 

Eden Hazard, a year before (2018), had just performed extremely well in the World Cup by leading his home country Belgium into semifinals by defeating precisely Neymar’s Brazil in the quarterfinals. 

Regarding Messi: he is the greatest of all time. Even at his advanced age he was amongst the top given his contribution to his team, which in that period was FC Barcelona, where he won the league but failed to go through the semifinals against Liverpool in Anfield. 

Additionally, notice how 5 out of the 10 players are left-wingers.

But what are these characteristics that contribute the most to a player’s market value? Let’s look at overall correlation metrics.

Feature	Correlation
ThruBalls	0.572945
ProgCarries	0.567267
GCA	0.567214
GCAPassLive	0.555344
PenAreaCmp	0.547783
CarriesToFinal3rd	0.535508
Att3rdTouch	0.535358
npxG+xA	0.526606
SCAPassLive	0.523227
PrgCarryDist	0.518252


