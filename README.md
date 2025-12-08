Predicting Traffic and Vehicle Dynamics in New York City

- Research Question: To what extent can a recurrent neural network (RNN), trained on several years of NYC hourly traffic volume counts, predict short-term traffic for individual streets across New York City?

- New York City has a reputation as one of the most congested cities in the world. Understanding how traffic fluctuates hourly across different streets is essential for sustainable mobility planning, intersection design, and emergency response. Hourly traffic counts reveal strong temporal patterns—rush-hour peaks, nighttime drops, weekday/weekend differences—that are ideal for time-series modeling.

- We use the NYC Open Data Traffic Volume Counts dataset, which provides traffic volume per street segment at hourly resolution.
    Each record includes: street segment (SegmentID), date, 24-hour traffic measurements, direction, and roadway name
  
- We restructure the dataset from wide to a long format to reshape for each hourly count. This allows us to treat each street segment as a time series.

- Main objective is to demonstrate whether deep learning models can reliably predict short-term traffic volumes in NYC and to explore the viability of expanding such models toward larger tasks
