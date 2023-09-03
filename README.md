## [The Dashboard](https://public.tableau.com/app/profile/tigran.hakobyan/viz/SportsIndustryBenchmarks/Story1)

### Project Goal

The aim was to have all the digital and social performance data of sports organizations (around 500 in total) in one centralized place, that would allow us to benchmark them against each other across various metrics (~ around 50).

### Areas

- Facebook

- Instagram

- Twitter

- TikTok

- YouTube

- Google Play Market App

- Squad Values (applicable only for Football Clubs)

- Stadium Capacity & Attendance (applicable only for Sports Clubs)

- On-Pitch Performance (applicable only for Football Clubs)

### Organizations Featured

- All the football clubs from top european leagues (Premier League, La Liga, Bundesliga, Serie A, Ligue 1)

- UEFA national football teams

- All the main football tournaments and governing bodies (FIFA, UEFA, CONCACAF etc).

- All the clubs from top US sports leagues (MLS, NBA, NFL, MLB)

- Tennis, Golf, Equestrian, Motorsport organization & events.



### Data Collection

- Different data collection methods have been used for each of these areas.

- Some of these are collected via scraping, some of the data is collected via public free APIs, and some of the data is being exported as a csv from external tools. And then it all gets merged together into one big dataset that is being used for the Tableau dashboard.

- All has been done in Python/Jupyter Notebook.


### Data Visualization

The collected and merged data has been then imported to Tableau as csv to build the dashboard with visualizations.

#### 1. League Tableau View

This allows us to see how each organization ranks across each metric by sorting the table on that specific metric. It’s sorted by the first column by default.

This view can be also useful for filtered search.

![Screenshot_9](https://github.com/hakobiant/Spots-Industry-Benchmarking/assets/58417428/6fee05b2-a630-42a9-94cb-830bcb72b089)

#### 2. Tableau View

This is a more simplified table where we have 7 columns with 7 metric selectors.

This view is useful when the user wants to build his own table with certain metrics in a certain order.

![Screenshot_8](https://github.com/hakobiant/Spots-Industry-Benchmarking/assets/58417428/2a514b93-8763-410c-a19b-baa57b137dc2)

#### 3. Averages View

Horizontal bar charts with the average line have been used in this view.

This is more of a visual representation of a table, where users can quickly grasp where each account stands compared to the average for the selected set of organizations.

![Screenshot_7](https://github.com/hakobiant/Spots-Industry-Benchmarking/assets/58417428/64ea4cc2-a694-47d1-83a1-fde033b6fc90)

#### 4. Scatter View

Scatter plot with adjustable axes is one of the most useful visualizations, and I don’t see this often elsewhere.

Users can choose any kind of combination for horizontal and vertical axis with metric selectors on the right hand side.

We also have a ‘Highlighter’ section/feature for users to be able to quickly find and highlight a certain desired organization in the sea of dots.

![Screenshot_6](https://github.com/hakobiant/Spots-Industry-Benchmarking/assets/58417428/6b79d30d-664a-4a6a-b6b7-a53057651fae)

#### 5. Head to Head View

A radar chart has been used in this view.

Inverse Rankings have been used to standardize and put all the variables on the same scale to range from 1 to 284 (which is the total number of sports clubs used for this radar chart). 

The higher the score the better. E.G. IG Followers score of 220 means that the team is doing better than the other 220 teams below it and has only 64 teams doing better.

The chart is best when comparing 2 or 3 teams, as it becomes hard to read with too many teams.

![Screenshot_5](https://github.com/hakobiant/Spots-Industry-Benchmarking/assets/58417428/6b181732-b92f-47f2-9ae3-c34aae870a4e)


