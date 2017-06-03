# Toonami Ratings MySQL Table

I'm Elias, creator of the now-defunct ToonamiCountdown.com and former writer at ToonamiFaithful.com.

Back in 2015, I had plans to create a new website called "ToonamiRatings.com", where anyone would be able to view [as] Toonami ratings data from its launch (2012) to the current day. I started inputting some data into an SQL table, and even put together some rough drafts for how the data would be presented on the website. But as other things in life began to consume my time, I abandoned the project. However, I've still been paying annually for the "toonamiratings.com" domain name, hoping that some use would eventually come of it.

A couple weeks ago I had the idea to go back to this project, fill out the rest of the SQL data up to the present day, and put it up on GitHub in case anyone else wants to continue from where I left off. I'm opening the opportunity to anyone who wants to fulfill my vision of a one-stop, easy-to-use, full-featured Toonami ratings website, complete with all sorts of graphs to visualize the vast amount of data that's been collected over the past five years. If this sounds like a project you'd be willing to take over, please contact me on my Twitter (@EJthedrummer) or Reddit (/u/MeshuggahIsLife) and I can transfer you the "toonamiratings.com" domain. In addition, I'm making the data available for anyone to use for any purpose, as long as I am credited by name.


## Data

The columns of the SQL table are as follows:

- Show (tinytext, NOT NULL) = the name of the show
- Date (tinytext, NOT NULL) = the date of the airing
- Time (tinytext, NOT NULL) = the timeslot of the airing
- Household (float(3,2), DEFAULT NULL) = total household ratings (in millions)
- Total (smallint(7), NOT NULL) = total viewers (in thousands)
- AHousehold (float(3,2) DEFAULT NULL) = household ratings (18-49 demographic)
- ATotal (smallint(7), DEFAULT NULL) = total viewers (18-49 demographic)

The "Household", "AHousehold", and "ATotal" values are NULL by default because their availability varies from time to time, and you'll notice that not all of them are filled for each date. I've filled out the table to the best of my ability using various online sources, but if you see anything that is missing, and can provide me with a source to fill it in, I'll gladly do so.

Shows that last longer than a half hour are listed multiple times (e.g. 1-hour special will have two entries, movies will have five or six entries). This is so that the day averages are more accurate. 

I will probably keep updating this table for a little while (maybe a month or so?), but I expect that whoever picks up the project will assume the role of updating it every week.

Huge thanks to AmbientVirus, Toonami Faithful, /u/irongarden3, /u/redragon11, /u/Error400BadRequest, and /u/I3rok3n_Sword2 for their  tables and spreadsheets which were a tremendous help in compiling this data, and of course an even bigger thanks to Douglas Pucci (@SonOfTheBronx) for providing us with all this data in the first place. 

If anyone has any questions at all, or would like to use this data, don't hesitate contact me on my Reddit (/u/MeshuggahIsLife) or Twitter (@EJthedrummer)! :) 
