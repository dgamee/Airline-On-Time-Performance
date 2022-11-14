# Airline On-Time Data Exploration

## by Aniekan Inyang


## Dataset

This dataset reports flights in the United States, including
carriers, arrival and departure delays, and reasons for delays,
from 2004 to 2008. The data is packaged in yearly chunks. Variable descriptions are the Year 2004-2008, Month from 1-12, DayofMonth from 1-31, DayOfWeek is 1 (Monday) - 7 (Sunday), DepTime is actual departure time (local, hhmm), CRSDepTime is scheduled departure time (local, hhmm), ArrTime is actual arrival time (local, hhmm), CRSArrTime is scheduled arrival time (local, hhmm), UniqueCarrier is unique carrier code, FlightNum is flight number, TailNum is plane tail number, ActualElapsedTime in minutes, CRSElapsedTime in minutes, AirTime in minutes, ArrDelay is arrival delay, in minutes, DepDelay is departure delay, in minutes, Origin is origin IATA airport code, Dest is destination IATA airport code, Distance in miles, TaxiIn is taxi in time, in minutes. TaxiOut is taxi out time in minutes, Cancelled was the flight canceled? CancellationCode is reason for cancellation (A = carrier, B = weather, C = NAS, D = security), Diverted 1 = yes, 0 = no, CarrierDelay in minutes, WeatherDelay in minutes, NASDelay in minutes, SecurityDelay in minutes, LateAircraftDelay in minutes. The dataset and documentation can be found [Here](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/HG7NV7)


## Summary of Findings

The Airline's on-time performance datasets, as obtained from the extraction of 2004 to 2008 monthly data contain 31,254,220 records and 29 features. Most cancellation is due to the carrier, followed by weather, with security being the least of all cancellation causes. It's clearly the visible year 2007 had the most cancellation, followed by the year 2005, and the least period is the year 2008. The distribution of departure and arrival delays was all unimodal and skewed to the right. A look at cancellations by carriers and weather, with respect to month and years, was determined, shows MQ(Envoy Air) to be the highest with carrier cancellation, followed by WN (Southwest Airlines), and UA (United Airlines, Inc)) are the top three carriers with highest cancellations. The least is f9 (Frontier Airlines, Inc.). It is interesting to note that the first two months see the most cancellations, i.e January and February, followed by December being the third month with the most cancellation for the 5 years study period due to weather. Arrival and departure delays appear to have a strong relationship of about 91%. Further analysis, shows that both carrier and aircraft-related delays contribute more to maximum overall delays as compared to other delays over per month, from 2004 to 2008.


## Key Insights for Presentation

During the course of analysis, major focus was centered on delays and cancellations using graph, comparison was established between delay factors, detecting cascading failures in departure delays at the origin airport, and creating arrival delays destination airport. lastly, we detected higher delay duration are caused by carriers and security reasons are the least common with less variation.