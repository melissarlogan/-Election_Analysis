# Election Analysis
## Background
This project reviews the election results of three Colorado counties: Jefferson, Denver, and Arapahoe to determine the overall county statistics and individual candidate results.
## Purpose
This analysis is an audit of the election results that were provided in a csv. file to present to the election committee. This analysis reviews all the votes that were cast and calculates how many votes each candidate had, how many votes were cast in each county, and the overall winner of the election. This report reviews the  over 300,000 votes that were cast in these counties and summarises them quickly for the election committee to review. 
## Results
Below are the overall results from the Jefferson, Denver, and Arapahoe county elections. Please refer to the below image of the txt file results.
* There were 369,711 votes cast in this congressional election.
* Jefferson county received 38,855 votes (10.5%), Denver county received 306,055 votes (82.8%) and Arapahoe received 24,801 votes (6.7%).
 * Denver county had the largest number of votes at 306,055, or 82.8% of all the votes.
* Charles Casper Stockham received  23.0%  (85,213) of the votes, Diana DeGette  received  73.8% (272,892)  of the votes, and Raymon Anthony Doane received  3.1% (11,606)  of the votes.  
* Diana DeGette  won the election having received  73.8% or 272,892 total votes .
![election_analysis_txt_output](https://user-images.githubusercontent.com/85718354/125200361-bc4ad980-e238-11eb-96c0-28c4108bc3b5.JPG)
## Election Audit Summary
This script is written in a way that allows for growth making it possible to be used for any election results in any state. Once the csv. is updated, or a new csv is added- it will comb through the data to review and will present the same results as the above (results by the total countifies and candidates) . This would be done in the below section of the script.
```
import csv
import os
file_to_load = os.path.join("Resources", "election_results.csv")
file_to_save = os.path.join("analysis", "election_analysis.txt")

```
### Potential Modifications for Other Elections
1. You could go into further depth across counties and look at regions within those counties to review where majority of the votes are coming from (rural or urban locations). This would be done in a similar fashion to the current script by initializing an additional for loop and the appropriate variables once the information is added into the csv. data file
2. You could also review the method in which the individual voters voted (in-person, mail-in etc., at early voting stations). This could be done by adding the source of the vote within the csv. file, and again writing another for loop with different variables to review what % of voters voted early as a total and by candidate. 
