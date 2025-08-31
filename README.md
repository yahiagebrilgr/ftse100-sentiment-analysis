UK Market Sentiment Analysis from Financial News

Aim: 
The aim of this project is to investigate whether the sentiment of financial news headlines has a measurable correlation with the daily performance of the UK stock market. This project uses Natural Language Processing (NLP) to quantify sentiment and applies statistical analysis and visualisation techniques I've learned from my data science courses.

The strategy: 
The hypothesis is that the overall sentiment of the news on a given day could be a leading or coincident indicator of market movements.
 - Positive news sentiment might correlate with positive market returns.
 - Negative news sentiment might correlate with negative market returns.
I'll test this by scoring sentiment and comparing it against the daily returns of the FTSE 100 index.

The plan: 
The project is broken down into five main steps:

(1) Setup and Data Collection: Import libraries and get historical price data for the FTSE 100.
(2) Data Simulation: As historical news feeds are not readily available for free, I simulated daily sentiment data to build and test the analytical pipeline.
(3) Data Preparation: Merge the simulated sentiment with the market data and prepare it for analysis.
(4) Correlation Analysis: Calculate the statistical correlation between sentiment and market returns.
(5) Visualisation & Analysis: Create plots to visualise the findings and write a conclusion based on the results.

--------------------------------
Analysis of Results: 
The main goal here was to build and test a pipeline to see if financial news sentiment could predict FTSE 100 movements. As historical news feeds aren't easy to get for free, I used simulated (random) sentiment data to check if my analysis method was working correctly.

A quick look at the graphs from my simulation:
Sentiment vs. Market Returns (Scatter Plot): The first graph plots the daily sentiment score against the market's return for that day. As you can see, the points are just a random cloud. The red line, which shows the trend, is almost perfectly flat. This is what you'd expect to see when there's no real connection between two variables, and it confirms my correlation calculation of nearly zero (-0.0241).

Sentiment Over Time (Time Series): The second graph shows the rolling average of my simulated sentiment score over the two-year period. It just looks like random noise fluctuating around a slightly positive value, which makes sense because that's how I designed the simulation. There are no clear patterns that seem to line up with real-world market events.

Final Thoughts & Future Work:
My analysis correctly showed that random data has no predictive power, which means the structure of my project and my code are sound. The main limitation is obviously the data itself. 

For a real-world application, this model would need lots of upgrades to be effective. For instance, a hedge fund might use a similar framework but with much more sophisticated tools:

(1) Better sources for my data: Instead of one news feed, they would use a high-speed, paid service (like a Bloomberg Terminal feed or a dedicated news API) that provides news from thousands of global sources, timestamped to the millisecond. This would allow for a much richer and more accurate sentiment signal.

(2) Using more Advanced NLP models: Rather than a general-purpose tool like VADER, a professional team would train a custom NLP model (like a BERT or other transformer model) specifically on financial news. This would allow the model to understand the specific nuances of financial language.

(3) High-Frequency Analysis: The market reacts to news in seconds, whereas this strategy covers days. A real world strategy would need more frequent data to capture the immediate impact of a news story breaking.

This project was an  okay exercise in building an end-to-end data analysis pipeline, but turning it into a profitable, real-world trading strategy would require these more advanced, resource-intensive steps.
