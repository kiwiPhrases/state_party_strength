# Data on party strength in each US state
The repository contains data on party strength for each state as shown on each state's corresponding party strength Wikipedia page.

Each state has a table of a detailed summary of the state of its governing and representing bodies on Wikipedia but there is no data set that collates these entries. I scraped each state's Wikipedia table and collated the entries into a single dataset. The data are stored in the **state_party_strength.csv** and **state_party_strength_cleaned.csv**. The code that generated the file can be found in Python notebook. 

### Data contents:
The data contain information from 1980 on each state's:
  1. governor and party
  2. state house and senate composition
  3. state representative composition in congress
  4. electoral votes
 
### Clean Version
Data in the clean version has been cleaned and processed substantially. Namely:
- all columns now contain homogenous data within the column
- names and Wiki-citations have been removed
- only the party counts and party identification have been left
The notebook that created this file is [here](https://github.com/kiwiPhrases/state_party_strength/blob/master/Cleaning_Party_Strength_per_state.ipynb)

### Uncleaned Data Version
The data contained herein have not been altered from their Wikipedia tables except in two instances:
- Forced column names to be in accord across states
- Any needed data modifications (ie concatenated string columns) to retain information when combining columns

This means that you will likely have to perform further data wrangling prior to doing any substantive analysis. The notebook that has been used to create this data file is located [here](https://github.com/kiwiPhrases/state_party_strength/blob/master/party_strength_per_state.ipynb)

## Raw scraped data
The raw scraped data can be found in the [pickle](https://github.com/kiwiPhrases/state_party_strength/blob/master/df_dict_raw.pkl). This file contains a Python dictionary where each key is a US state name and each element is the raw scraped table in Pandas DataFrame format.

Hope it proves as useful to you as it proved to me. 
