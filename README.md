# cleveland-mlb-games

Cleveland MLB (Guardians) game duration forecast.

This project is composed of three parts:

* Step 1: Get the data. [step_1_get_games.R](./step_1_get_games.R) is an R script that pulls the data.
* Step 2: Explore the data. [step_2_exploration](https://mpfoley73.github.io/cleveland-mlb-games/step_2_exploration.html) is a web page that explores the data. I look at game duration, but also attendance and other features. The data is just too rich to stop at game duration!
* Step 3: Forecast. Using time-series analysis techniques I project game durations over the next few seasons.
  * [Linear Regression](https://mpfoley73.github.io/cleveland-mlb-games/step_3_linear.html),
  * [Exponential Smoothing](https://mpfoley73.github.io/cleveland-mlb-games/step_4_ets.html), and 
  * [ARIMA](https://mpfoley73.github.io/cleveland-mlb-games/step_5_arima.html)

## What the project does

This project forecasts average game duration for the Cleveland Guardians using historical data. Major League Baseball games last nearly twice as long as they did in 1901. Using data from [Baseball-Reference.com](https://www.baseball-reference.com/), I compiled individual game statistics for the Cleveland Guardians all the way back to their inception in 1901.

![](./img01_duration_trend.png)

I used three time-series forecasting methods to project game durations into the next decade. The average Cleveland baseball game during the 2021 season was 3 hours and 5 minutes. My linear regression model predicted game times will increase to 3 hours 15 minutes by 2031. My exponential smoothing model and my ARIMA model predicted 3 hours 12 minutes.

## Why the project is useful

Time-series forecasts *could* be exercises in prediction based on scenarios and measured past responses to conditions that change in the scenarios. But it seems most time-series forecasts are bounded projections of past data based on the underlying trend and seasonal patterns in the historical data. That is what I have done here. Baseball game times have increased over time, but not steadily and their have been periods of decline. 

From the perspective of a practicing data analyst, this project presented interesting challenges. Game logs are conveniently stored in html tables on Baseball-Reference.com, but there is one web page per season, so I had to scrape 100 web pages to get the data (see [step_1_get_games.R](./step_1_get_games.R)). The exploratory phase is almost always a creative discovery exercise, and historical baseball events are great for this. For example, I discovered a precipitous *drop* in game duration shortly after the steroid era ended. Of course, that was also a period where the Tribe tanked in the standings. [step_2_exploration](https://mpfoley73.github.io/cleveland-mlb-games/step_2_exploration.html) has several neat discoveries like this. The analysis steps [step_3_linear](https://mpfoley73.github.io/cleveland-mlb-games/step_3_linear.html),  [step_4_ets](https://mpfoley73.github.io/cleveland-mlb-games/step_4_ets.html), and [step_5_arima](https://mpfoley73.github.io/cleveland-mlb-games/step_5_arima.html) are semi-tutorial styled exercises in time series analysis. I included some methodological detail so I can refer to this project later. Most of what I know about time series analysis is from Rob Hyndman's [Forecasting: Principles and Practice](https://otexts.com/fpp3/), and my notes are compiled [here](https://bookdown.org/connect/#/apps/67b5716a-6cdd-4892-935c-d6860310432b/access).

## Who maintains and contributes to the project

I worked on this project independently. I may revisit it after learning more about time series methods, but I consider this project closed.

