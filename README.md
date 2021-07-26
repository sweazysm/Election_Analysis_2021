# Election Analysis 2021
### Project Overview
The project assigned was from that of a Colorado Board of Elections employee who wished to know the results / election audit of a recently held local election. These results are to be sent to the Election Comission and they need to be accurate.

The goals set forth for this analysis were as follows: 

- Determine the total number of votes cast in the Election

- Design and create a complete list of all candidates that recieved votes during the Election

- Design code that determines the total votes recieved for each candidate during the Election

- Design code that determines the total percentage of votes recieved for each candidate during the Election

- Expand upon previous code and determine the winner of the Congressional Election 

---
# Resources
Software and Resource Files used in this project are as follows:

### Software
- Visual Studio Code (VS Code), Version 1.58.2

- Python, Version 3.9.6

### Resouce Files

- election_results.cvs

---
# Election Audit Results

The results from the Election Audit are as follows:

- The election had a large turnout, with a total of 369,711 voters coming out to vote in the counties analyzed. 

- The counties analyzed for this election were Jefferson county, Denver county, and Arapahoe county. For these counties analyzed, Jefferson county recieved 10.5% of the vote, totalling 38,855 votes; Denver county recieved a whopping 82.8% of the vote, totalling 306,055 votes; Arapahoe county recieved 6.7% of the vote, totalling 24, 801 votes. From this data it is clear that Jefferson County had the highest overall voter turnout for the three counties analyzed.

- For the Candidates, there were several candidates in the race that recieved votes: Charles Casper Stockham, Diana DeGette, and Raymon Anthony Doane. In this election's results, Charles Casper Stockham recieved 23.0% of the vote, totalling 85,213 votes; Diana DeGette recieved a whopping 73.8% of the vote, totalling 272,892 votes; Raymon Anthony Doane recieved 3.1% of the vote, totalling 11,606 votes. From this data we can see that the winner of the election was Diana DeGette.

- Overall, the data tells us that the Election winner was Diana DeGette who recieved 73.8% of the vote, totalling 272,892 votes, and the most votes were cast in Denver County.

<img width="373" alt="Screen Shot 2021-07-25 at 8 47 06 PM" src="https://user-images.githubusercontent.com/86274124/126921822-adb3a58e-8766-4b02-9bfc-4c0a84f23b77.png">
<img width="296" alt="Screen Shot 2021-07-25 at 8 16 53 PM" src="https://user-images.githubusercontent.com/86274124/126921833-c795e9ab-7e79-49fd-81a8-48f9be1b6cb2.png">

Shown above is the output from the Election Analysis code within VS Code's Interactive Terminal and the Election Analysis text file.

# Election Audit Summary

The process of creating code within Python for this project was long and tedious. Many hands were thrown up in exhaustion and many headaches were experienced. However, the following code allows one to analyze large amounts of election data in a concise and collected manner to quickly return an easy-to-understand summary of results. For an Election Commission responsible for delivering final vote results, not only do answers need to be delivered quickly - they need to be delivered fast. Not only does the following code for this Election Analysis do just that, but this code can be modified for other elections as well which would be of great use to an Election Commission.

When running this code for various other elections, only certain things need be tweaked. 

    # Add our dependencies.
    import csv
    import os

    # Add a variable to load a file from a path.
    file_to_load = os.path.join("Resources", "election_results.csv")
    # Add a variable to save the file to a path.
    file_to_save = os.path.join("analysis", "election_analysis.txt") 

For future analyses, the paths above need to be updated and declared with proper names and titles. Titles could be "2022_election_information.txt" or "final_election_results_2022.csv" or a myriad of other titles. Simple tweaking in this area will allow for information to be properly referenced.

    # Print the final vote count (to terminal)
    election_results = (
        f"\nElection Results\n"
        f"-------------------------\n"
        f"Total Votes: {total_votes:,}\n"
        f"-------------------------\n\n"
        f"County Votes:\n")
    print(election_results, end="")

    txt_file.write(election_results)
    
For future analyses, the format of the printed results can be changed around. File names will need to be updated to properly references and declare information. F-string formatting can also be modified to change how the results are outputted to the termianl and/or to any text files. F-string line breaks can be extended, shortened, or removed all together! The declaration for different variables ("Total Votes:") can also be changed to declare outcomes in various ways.

---

In summary, the code provided can be formatted and reused for other election data sets for other elections around the country. Future analysts are not limited to the suggested tweaks shown above, more editing can be done to compile and reference data in other various ways. With such a maleable code with declarations and comments, this code can be edited for future elections with little hassle making it not only reliable but also highly efficient and useful.
