# Twitch Analytics
Looking at Twitch channel analytics with pandas and matplotlib in Python. For funsies.

The data used in this project spans from May 1, 2020, to May 15, 2022.

### Data Prep

First, we dropped columns that have no data. These were multi-year gift subs and advertisement minutes (yay, no ads for my viewers!).

Next, we dropped all rows where `Minutes Streamed` = 0. 

Finally, we added a new date column, `New Date`, to format the date given by Twitch.

### Visualizations

To start, we graphed average viewers over time as a line graph. Next, we created a scatter plot of minutes streamed versus the total unique viewers of that stream. Interestingly, this looks more linear than I expected.