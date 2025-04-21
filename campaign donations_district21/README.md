Analysis of New York City Campaign Finance data for City Council race of District 21 — 01/15/2022 to 03/13/2025
This repository contains data, analytic code, and findings that support portions of the article, “In a highly competitive City Council race, donations are mounting,” published April 21, 2025. Please read that article, which contains important context and details, before proceeding.

Data
This analysis uses New York City Campaign Finance Board (NYCCFB) data for the campaigns of each candidate in District 21.

The spreadsheets come from the following sources:

Compiled Google Sheets:
https://docs.google.com/spreadsheets/d/1-pSUtpd-dWTGKDhvYMGhpDPdQjWNvDZkB3P7i_22gpM/edit?usp=sharing: Raw data of https://www.nyccfb.info/FTMSearch/Home/FTMSearch
Each of the compiled data sets contain, among others, the following columns relevant to the analysis:

RECIPNAME - The name of a candidate that recieved a donation for their campaign. As of publishing, there are seven candidates: David Aiken, Yanna M. Henriquez, Hiram Monserrate, Erycka Montoya, Sandro S. Navarro, Diane Rose and Shanel Thomas-Henry. 
RECIPID — Each candidate has a unique identification number that is between 3-4 characters long. 
OCCUPATION — This title is self-reported by donors and is not verified by the NYCCFB. 
AMNT - The amount donated by each donor. 

Methodology
The notebook campaigndonations_district21.ipynb performs the following analysis:

Part 1: Importing Data 
In this section, I imported my csv to the notebook "campaigndonations_district21.ipynb." Then I made sure the dtype of the relevant columns were accurately read by python. 
Part 2: Total Campaign Donations per Candidate
Using the groupby function, I was able to sort the number of total donations each candidate recieved from highest to lowest. I then found the total sum of donations for each candidate, organizing it from hgihest to lowest as well. 
Part 3: Donors by Occupation
Finally, to see which donors were donating the most in each campaign, I used grouby and aggregation functions. Doing so enabled me to see that retirees were the highest occupation group to donate for two candidates with the highest total amount of campaignn donations: Shenal Thomas-Henry and Hiram Monserrate. 

Outputs
The notebooks output this spreadsheet which contains donors organized by self-reported occuption title, sorted from greatest to least sum of their donations per candidate: output/tktktk.csv.

Running the analysis yourself
You can run the analysis yourself. To do so, you'll need the following installed on your computer: ("../output/donations_by_occupation_amount")

Python 3
Pandas, a library in Python

Licensing
All code in this repository is available under the MIT License. The data file in the output/ directory is available under the Creative Commons Attribution 4.0 International (CC BY 4.0) license. All files in the data/ directory are released into the public domain.

Feedback / Questions?
Contact Gabriela Flores at Gabriela.Flores07@journalism.cuny.edu.