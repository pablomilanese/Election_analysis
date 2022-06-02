## Overview of Election Audit
The purpose of this analysis was to use python in order to determine the outcome for a local congressional election in Colorado. The goal was to determine the winning candidate and the largest voter turnout by county. This was accomplished by using a dataset provided with ballot ID, county and candidate selected.

## Election-Audit Results

##### · HOW MANY VOTES WERE CAST IN THIS CONGRESSIONAL ELECTION?
> There were 369,711 votes cast in this congressional election.
##### · PROVIDE A BREAKDOWN OF THE NUMBER OF VOTES AND THE PERCENTAGE OF TOTAL VOTES FOR EACH COUNTY IN THE PRECINCT.
> Denver — 82.8% (306,055 votes)<br/>
> Jefferson — 10.5% (38,855 votes)<br/>
> Arapahoe — 6.7% (24,801 votes)<br/>
##### · WHICH COUNTY HAD THE LARGEST NUMBER OF VOTES?
> Denver had the largest number of votes, accounting for 82.8% of the total.
##### · PROVIDE A BREAKDOWN OF THE NUMBER OF VOTES AND THE PERCENTAGE OF THE TOTAL VOTES EACH CANDIDATE RECEIVED.
> Diana DeGette — 73.8% (272,892)<br/>
> Charles Casper Stockham — 23.0% (85,213)<br/>
> Raymon Anthony Doane — 3.1% (11,606)<br/>
##### · WHICH CANDIDATE WON THE ELECTION, WHAT WAS THEIR VOTE COUNT, AND WHAT WAS THEIR PERCENTAGE OF THE TOTAL VOTES?
> Diana DeGette won the election with 272,892 votes, accounting for 73.8% of the total votes casted.

## Election-Audit Summary
The code written for this analysis is a tool that can be easily repurposed for future elections.
Given that every election will include 'candidates', 'counties' (or other territorial divisions) and 'votes casted' as variables, there is not a lot of re-work needed to guarantee that it gets the job done. This code is meant to identify these variables and calculate results accordingly. 

 - The most important modification this code needs will be identifying the location of the starting dataset at the beginning of the code:

<img width="484" alt="Screen Shot 2022-06-01 at 11 35 24 PM" src="https://user-images.githubusercontent.com/105120795/171554347-f52e64f0-2c7d-42d9-9f0d-ec599b0dd13b.png">


The code above tells Python to find the file "election_results.csv" inside the "Resources" folder in order to read it. It is crucial for the code to work that the correct path is identified at the beginning. It would be good practice to keep the original datasets for each election in the same folder to streamline the code each time.
 
- Another chore the code does is exporting the results in a new file. In the example above the file is called "election_analysis.txt". I also propose that every future election audit has a specific name tied to each election. For example "analysis_06012022". In this example we add the date to the output document. By doing so the board can streamline their work by keeping the results for every election in the same folder.

- Like I mentioned above, this code can also easily work for elections that will cover bigger territorial areas such as cities.

<img width="708" alt="image" src="https://user-images.githubusercontent.com/105120795/171555477-1035d3e1-10ca-4ee3-9424-4aef2d77e55a.png">

In the code above we can see how Python analyses county outcomes. For clarity purposes the code can be adjusted by changing the names of variables such as county_name to city_name. Because the clarity of code is only as good as the person that edits it, it's important to keep details like this in mind to ensure that somebody in the future can also repurpose it for another type of election.
