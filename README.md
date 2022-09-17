# Citi Bike Analytics: Ride and User Data from Fall 2019 and Fall 2020

For this assignment, I was tasked with aggregating the data found in the Citi Bike Trip History Logs and finding two unexpected phenomena.

I chose to look at the months of September, October, and November in 2019 and 2020 to see how fall ridership changed with the COVID-19 pandemic. To get started, I downloaded the six separate CSV files (one for each month), read them into Pandas as DataFrames, and then concatenated them into one new CSV file. The headers in the Citi Bike CSVs were all still consistent during this time frame, but have since changed.

**The first unexpected phenomenon was that rider trends during the day, and month to month, remained relatively similar despite the change in lifestyle that affected New Yorkers with the arrival of COVID-19.** While total rides increased from Fall 2019 to Fall 2020, the trend of decreasing ride numbers from September to October, and from October to November, remained pretty similar (as shown in the top right visualization on page 2 of my [Tableau Story](https://public.tableau.com/views/Fall2019-2020CitiBike/Overview?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)). 

One marked difference between the two datasets was the peak of morning commuters in Fall 2019. In Fall 2020 ride numbers still increased rapidly to the 8am hour, but did not reach as high as the 2019 numbers. This could be explained by the rise in remote work during the pandemic. However, ride numbers in both datasets continued a steady increase throughout the rest of the workday, with both peaking around 5pm (as shown in the bottom visualization on page 2 of my Tableau Story). With so many people working remotely in 2020, I had anticipated more variation within the 2020 dataset and was surprised to see so many similarities with the data from 2019.

This phenomenon can also be noticed in the next page of my Tableau Story in the visualizations showing the average ride distance and duration. During the fall months of both years, the average ride distance slightly decreases from month to month. You can also see that average ride duration follows similar trends in both years.

While people's jobs and lifestyles changed during the pandemic, there were still people still commuting to their places of work in Fall 2020. Even those working remotely were probably keeping the same hours, so this could explain the similar patterns in ride start times from year to year. 

**These visualizations also show another phenomenon: rides in Fall 2020 were longer in both time and distance (on average) than rides in Fall 2019.** One hypothesis for this could be that people traveling in 2020 were more averse to using public transportation like the subway or buses due to the pandemic, so Citi Bike rides were potentially providing transportation for travelers who would have been using public transit for that same journey in 2019.

Another unexpected finding was that rides by subscribers did not increase from Fall 2019 to Fall 2020 (as shown on page 4 of my Tableau Story). I had assumed that since overall rides had increased in 2020, then rides by subscribers and customers would have both increased as well. Thinking more about this, I could see this number being impacted by the pandemic. If users were no longer regularly commuting to their place of work, a subscription might not have seemed worth it in 2020 versus 2019. Assuming that Citi Bikes took the place of some people's use of the subway or buses during the pandemic, that could explain an increase in one-off rides from customers rather than subscribers.

The final two pages of my Tableau Story looks at bike station popularity. In looking at rides overall (from both datasets), I was surprised to see an almost complete overlap in the top 20 used stations for both starting and ending a ride. The treemap below the station map shows the most popular start and end station combinations for all rides in Fall 2019 and Fall 2020. I was not expecting to see so many of these results (12 of the 32 pairings) with rides using the same station to start and end. After seeing this, I was curious to see if that was a similarly popular occurance in both years so I created treemaps for each dataset in order to compare (as shown on the final page of my Tableau Story). 

**When comparing the two treemaps (top shows 2019, bottom shows 2020), you can see the increase in popularity of using the same station to start and end a journey.** In Fall 2019, only 2 of the 29 station pairings feature the same start and end locations. In Fall 2020, 21 of the 33 pairings use the same start and end locations. This change in the data shows that more users were keeping the same bike with them for the duration of their trip, rather than docking the starting bike upon arrival to their destination and then selecting a new bike (or other form of transportation) for their return journey. This could be for a multitude of reasons. One could be that Citi Bikes were used for more out-and-back trips in 2020 than in 2019 (like errands, rather than commuting for example). If this was the case, it could also explain the increased ride duration averages mentioned above. Another reason could even be that users were more concerned about the potential transfer of germs after the arrival of COVID-19 and were more inclined to keep one bike rather than use any additional ones for their journey.