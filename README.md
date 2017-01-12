# Data on party strength in each US state
The repository contains data on party strength for each state as shown on each state's corresponding party strength Wikipedia page.

Each state has a table of a detailed summary of the state of its governing and representing bodies on Wikipedia but there is no data set that collates these entries. I scraped each state's Wikipedia table and collated the entries into a single dataset. The data are stored in the **state_party_strength.csv** and the code that generated the file can be found in Python notebook. 

### Data contents:
The data contain information from 1980 on each state's:
  1. governor and party
  2. state house and senate composition
  3. state representative composition in congress
  4. electoral votes
 
The data contained herein have not been altered from their Wikipedia tables except in two instances:
- Forced column names to be in accord across states
- Any needed data modifications (ie concatenated string columns) to retain information when combining columns

This means that you will likely have to perform further data wrangling prior to doing any substantive analysis. 

Hope it proves as useful to you as it proved to me. 
