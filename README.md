# Election_Analysis
Module 3 Challenge
## Overview of Project
### Purpose
The Colorado Board elections were made and it is needed to audit all numbers and analysis. That's why we need to explore all votes in 3 counties.
### Information
In election_results.csv is the information of all votes with:
- Ballot ID - ID for each vote
- County - 3 counties: Jefferson, Denver and Arapahoe
- Candidates to be voted

In order the audit is complete, these analysis need to be calculated:

- Total of votes

- Votes per county (we alreday know there are 3)
- Percentage of votes per county
- Largest county of votes

- Candidates who received votes
- Votes per candidate
- Percentages of votes per candidate
- Winner candidate based on popular vote

## Election-Audit Results
The results of the audit are the following:

The total of votes are 369,711 in 3 counties, distribuited (vs total):
> County of Jefferson had 10.5% of votes (38,855)
> 
> County of Denver had 82.8% of votes (306,055)
> 
> County of Arapahoe had 6.7% of votes (24,801)
> 
**First conclusion: Denver is the county with the most votes cast.**

```
Technical Notes:
- The code audits all rows in the csv file
--- with a for loop for each row
--- during the for it counts every row with a counter 'total_votes'
--- it makes a list to keep the county 'county_name', making a comparison if it was read or not in previous lines
--- it counts the vote for each county
```

![image](https://user-images.githubusercontent.com/85086918/125145606-76323080-e0e7-11eb-9f8c-714fac3a5e8a.png)

![image](https://user-images.githubusercontent.com/85086918/125145615-877b3d00-e0e7-11eb-9557-aa3b0e7b7c95.png)

```
Technical Notes:
- Then, the code makes a text file where
--- it makes a variable to keep the results of counting 'county_votes'
--- it makes a variable to calculate the percentage of votes per county
--- it makes comparisions to know wich county is the largest
--- it writes every result in the txt file
```
![image](https://user-images.githubusercontent.com/85086918/125145752-30c23300-e0e8-11eb-8ab2-fae81ec90a05.png)


There are 3 candidates that received votes:
> Charles Casper Stockham: 23.0% (85,213)
> 
> Diana DeGette: 73.8% (272,892)
> 
> Raymon Anthony Doane: 3.1% (11,606)
> 
**Second conclusion: Diana DeGette is the winner in this election based on popular vote.**

```
Technical Notes:
- The code audits all rows in the csv file
--- with a for loop for each row
--- during the for it counts every row with a counter 'total_votes'
--- it makes a list to keep the candidate 'candidate_name', making a comparison if it was read or not in previous lines
--- it counts the vote for each candidate
```

![image](https://user-images.githubusercontent.com/85086918/125145802-74b53800-e0e8-11eb-8842-c821bbb98cad.png)

Technical Notes:
- Then, the code makes a text file where
--- it makes a variable to keep the results of counting 'candidate_votes'
--- it makes a variable to calculate the percentage of votes per candidate
--- it makes comparisions to know wich candidate is the winner and writes why
--- it writes every result in the txt file

![image](https://user-images.githubusercontent.com/85086918/125145849-aa5a2100-e0e8-11eb-961d-50b9aa0b8382.png)

## Election-Audit Summary

In this exercise we noticed we can expand the analysis for more states, counties and all kind of elections.
The reason why is because the code is not limited for these 3 counties, or candidates or votes.
The code count itself, find the names (counties and candidates) itself and make all calculations for each one (it doesn't matter how much are).

If it's necessary, the adjustments to use this code in the future are:
> To add one procedure to clean data or find missing values
> To add calculations to know winners for each county in order to find out the winner based on number of counties and not just for popular vote
> If there is historical information, make comparisons between years or periods of elections.

Finnally, we can aggregate a module to make graphics and make visualization even better than just tables.

By Raquel Valdez



