# UEFA Champions League Data Analysis

## Overview
This project delves into the UEFA Champions League from 2016 to 2022, capturing essential details about teams, stadiums, players, and match outcomes. It offers a rich view of the competition's landscape, helping us explore patterns, standout performances, and significant moments in European football.

## Contents
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Key Analyses](#key-analyses)
  - [Teams and Stadiums](#teams-and-stadiums)
  - [Player Positions](#player-positions)
  - [Player Contributions](#player-contributions)
  - [Match Participation](#match-participation)
  - [Wins in UCL](#wins-in-ucl)
  - [Assists Analysis](#assists-analysis)
  - [Top Goal Scorers](#top-goal-scorers)
- [Conclusion](#conclusion)
- [Technologies Used](#technologies-used)

## Data Cleaning and Preprocessing
The dataset consists of several sheets, each containing specific information about the tournament:

- **Teams DataFrame (`df_teams`)**: Retains the columns `team_name`, `country`, and `home_stadium`. No need to drop any columns, as duplicates are not an issue.

- **Stadiums DataFrame (`df_stadiums`)**: Contains `name`, `city`, `country`, and `capacity`. The `city` and `country` columns can be dropped. We can merge this sheet with `df_teams` by changing the stadium names to connect them with their respective teams.

- **Players DataFrame (`df_players`)**: The `first_name` and `last_name` columns can be merged into one column called `player_name`. The `weight` and `height` columns will be dropped since we focus on performance statistics.

- **Managers DataFrame (`df_managers`)**: Similar to players, the `first_name` and `last_name` columns will be merged into `manager_name`.

- **Matches DataFrame (`df_matches`)**: The `date_time` column will be dropped for analysis.

- **Goals DataFrame (`df_goals`)**: Merged with `df_matches` based on `match_id` for comprehensive insights.

## Key Analyses

### Teams and Stadiums
The analysis showcases the largest stadiums of Europe's iconic football clubs, each a fortress for their loyal fans.

**Top Stadiums:**
- **Camp Nou** (FC Barcelona): 99,354 spectators
- **Signal Iduna Park** (Borussia Dortmund): 81,365 spectators
- **Santiago Bernabeu** (Real Madrid): 81,044 spectators

This highlights Spain's passion for football with two of the top three stadiums.

### Player Positions
The distribution of players across positions is balanced:
- **Midfielders**: 32.20%
- **Defenders**: 31.24%
- **Forwards**: 25.40%
- **Goalkeepers**: 11.16%

This distribution emphasizes the need for a well-rounded team structure.

### Player Contributions
The dataset illustrates the global reach of football, with France leading with 190 players, followed by Spain (168) and Brazil (161).

### Match Participation
In the UCL from 2016 to 2022:

**Most Played Matches:**
- **Real Madrid**: 66 matches
- **Bayern München**: 59 matches
- **Manchester City**: 59 matches

### Wins in UCL
**Most Wins:**
- **Bayern München**: 44 wins
- **Real Madrid**: 41 wins
- **Manchester City**: 40 wins

### Assists Analysis
Assists are crucial in football, with top players showcasing their playmaking abilities:
- **Cristiano Ronaldo**: 36 assists
- **Robert Lewandowski**: 33 assists
- **Karim Benzema**: 32 assists

### Top Goal Scorers
From 2016 to 2022, the top goal scorers were:
- **Robert Lewandowski**: 54 goals
- **Cristiano Ronaldo**: 47 goals
- **Lionel Messi**: 42 goals

## Conclusion
This analysis provides a comprehensive overview of the UEFA Champions League, showcasing key statistics and insights from the matches played from 2016 to 2022. The findings highlight trends in goal scoring, player performance, and team strategies, contributing to a deeper understanding of this prestigious football competition.

## Technologies Used
- Python
- Pandas
- Matplotlib
- Seaborn
