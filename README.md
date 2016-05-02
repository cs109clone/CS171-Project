# The Meteoric Rise of Stephen Curry
*A CS171 Project by Jason Cui and Annie Hwang*

## Overview
Our interactive website describes NBA Player Stephen Curry’s basketball stats starting from college until his career now. The visualizations focus on data related to Stephen Curry’s this year’s as well as previous years’ stats (i.e. 3 point percentages, assists, rebounds, etc). The project shows other information regarding Stephen Curry (i.e. the rise in his salary level over the course of his career). The interactive visualizations will also aim to show an overview of Stephen Curry’s stats compared to those of other NBA players/averages.

## Questions We Wanted Answered
**How good was Stephen Curry in college?**

**How big is his contribution to the Warriors?**

**So how well (exactly) does Stephen Curry shoot?**

## Project Data
For most of the data, we were able to retrieve the stats from these links -- [first](http://www.sports-reference.com/cbb/players/stephen-curry-1.html) and [second](http://www.basketball-reference.com/players/c/curryst01.html) -- and export it as a CSV files. Like any other labs and homework assignments, our project aimed to create interactive visualization with graphs, charts, and other more interesting representations that may be more specific to basketball. From these websites, we will be able to gather data for his 3 point percentages, assists, rebounds, etc. We were able to find data from Curry’s college career at the same locations.

For the visualizations in the Warriors section, most of the data was found simply on ESPN and the NBA website ([link](http://espn.go.com/nba/player/stats/_/id/3975/stephen-curry)). To create the pie charts for the stats breakdown for each time, we stored all the stats for the top 15 players of each NBA team in the players.csv file.
For the more detailed data (i.e. exact distance and location of shooting), we were able to use the NBA stats API that returned a json data structure of any player given the player ID, season years, and other relevant information for shot charts. The external json data could be found on this [link](http://stats.nba.com/stats/shotchartdetail?Period=0&VsConference=&LeagueID=00&LastNGames=0&TeamID=0&Position=&Location=&Outcome=&ContextMeasure=FGA&DateFrom=&StartPeriod=&DateTo=&OpponentTeamID=0&ContextFilter=&RangeType=&Season=2015-16&AheadBehind=&PlayerID=201939&EndRange=&VsDivision=&PointDiff=&RookieYear=&GameSegment=&Month=0&ClutchTime=&StartRange=&EndPeriod=&SeasonType=Regular+Season&SeasonSegment=&GameID=). This shows Stephen Curry’s detailed shot details for the 2015-2016 season.

Overview of the data files is below:

+ `curry-college-data.csv` - FG, 3s, and FT data from college
+ `curry-college-tree.json` - json data for rewards and records in college
+ `curry-shot-chart-data.json` - shot chart data
+ `curry-warriors-data.csv` - complete warriors data
+ `map-pie-default-clicked-team.csv`, `map-pie-NBA-teams.csv`, `map-pie-players.csv`, `map-pie-teambar.csv` - data for map pie vis
+ `US-geo.json`, `US-states.csv` - geojson data for map pie vis

## File Structure
The majority of files within the project are contained within the `curry` folder. `index.html` contains the main index of the page. `index.html` will then link to `mainvis.html` which contains the bulk of the project.

Inside of `curry` we have:

+ `css` - css files
+ `data` - all data files
+ `font-awesome` and `fonts` - font files
+ `img` - image files
+ `js` - all js lib files and vis files
+ `less` - less data
+ `logo` - logos for map pie vis
+ `README.md` - this file! 

