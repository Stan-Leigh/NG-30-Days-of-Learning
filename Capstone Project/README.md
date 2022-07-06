# Analysis of Flight Delays in Airlines

## Introduction
This is the capstone project for the #30DaysOfLearning program organized by Microsoft for Nigerian University students during the ASUU strike. This project was done solely with Microsoft PowerBI.

The dataset was collected from [Kaggle](https://www.kaggle.com/datasets/jimschacko/airlines-dataset-to-predict-a-delay) and can also be found in this [repository](https://aka.ms/30DLDATGitHubRepo). It contains 539383 rows and 8 columns that talks about different flights and their features. The columns consists of:
* Airlines (Different types of commercial airlines)
* Flight (Types of Aircraft)
* AirportFrom (Source Airport)
* AirportTo (Destination Airport abbreviation)
* DayOfWeek (Numerical values of days of the week)
* Time (Number of minutes from start of day to flight time)
* Length (Length of the flight in minutes)
* Delay (Whether the flight was delayed or not, 1 for delayed and 0 for not delayed)

## Data Wrangling
The dataset was cleaned from the get-go but some minor modifications were made in Power Query:
* Convert the numerical values for days of week to their actual values (Monday, Tuesday, etc).
* Converted the minute values in the Time column to their hour equivalent for easier visualization.
* Created a new column from the Delay column that converted the numbers (1 and 0) to text (Delayed and Not Delayed) for easier visualization.

## Observations
Analysis of the Airlines Flight delay dataset produced a lot of interesting insights. The insights that were garnered are listed below:
* **44.54%** of Flights in this dataset were delayed. This is almost half of the data that contained over 500,000 flights. Upon further [research](https://en.wikipedia.org/wiki/Flight_cancellation_and_delay#:~:text=A%20flight%20delay%20is%20when,all%20for%20a%20certain%20reason.), it is discovered that according to the Federal Aviation Administration (FAA), a flight is said to be delayed when it is 15 minutes later than its scheduled time. This is a small amount of time given that there are a lot of external factors that can cause more than a 15 minute delay.
* **Wednesday**, **Tuesday** and **Thursday** has significantly higher number of flights compared to the other days of the week. The number of Flights on Fridays are also significantly lower than the rest.
* Of the three weekdays that have the highest number of Flights, **Tuesday** has more Delayed flights and **Thursday** has the higher number of non-delayed flights.
* SouthWest Airlines, **WN** recorded an abnormally high number of delayed flights, **66K**, compared to the number of non-delayed flights, **28K**.
* Most of the flights occur between 7am and 8pm.
* The bulk of the delayed flights occurred later in the day, between 12pm and 8pm.
* Most of the non-delayed flight occurred at the beginning of the day, between 7am and 9am.

## Limitations
* The dataset does not contain a column that specifies the date these flights happened, so it is difficult to combine it with another dataset in order to drill down and check if these delayed flights are a result of external factors such as weather.
