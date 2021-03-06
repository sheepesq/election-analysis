# election-analysis
**Overview of Election Audit: Explain the purpose of this election audit analysis.**
  The purpose of this election audit was to calculate the total votes casted in this election and determine a winner. The audit also tabulated the total of votes in each of the three counties.

**Election-Audit Results: Using a bulleted list, address the following election outcomes. Use images or examples of your code as support where necessary.**
-How many votes were cast in this congressional election?
  *Total Votes: 369,711, this was determiend by 
  *Initialize a total vote counter. by total_votes = 0 and then opening up the csv and   Add to the total vote count via total_votes = total_votes + 1, this way *the code will go through each row of data and total it. 

-Provide a breakdown of the number of votes and the percentage of total votes for each county in the precinct.
County Votes:
Jefferson: 10.5% (38,855) 
Denver: 82.8% (306,055)
Arapahoe: 6.7% (24,801)
This was calculated by the following lines of code:
    for county_name in county_votes:
        cvotes = county_votes.get(county_name)
        cvote_percentage = float(cvotes) / float(total_votes) * 100
        county_results = (f"{county_name}: {cvote_percentage:.1f}% ({cvotes:,})\n")
 We created a loop to run through each county name and take the vote total of each county and divide it by 100. The last row of code displays the results to be read by the user.       

-Which county had the largest number of votes?
  *
-Provide a breakdown of the number of votes and the percentage of the total votes each candidate received.
  *
-Which candidate won the election, what was their vote count, and what was their percentage of the total votes?
  *
-Election-Audit Summary: In a summary statement, provide a business proposal to the election commission on how this script can be used—with some modifications—for any election. Give at least two examples of how this script can be modified to be used for other elections.
  *
