YOUTUBE TRENDING ETL PROJECT 


Project Proposal:

https://docs.google.com/document/d/1g48VaWJGWbX0CZv_kYsnJjqptjK97n0sR4FLuXY7l9I/edit

Research and Gathering
We located two sources, one from Kaggle and the other from a website:

Website with Video Game Trending Sales: 

https://www.vgchartz.com

Kaggle Data located in USvideos.csv

Cleaning and coallating
The Youtube Data (YT Data) was in the above csv. That needed to have its date format adjusted, desired columns identified, undesired columns dropped, and put into a usable table. The data was then sent into a different dataframe with just the YT tags and the video ID. This would become a link to the new Video Game data.

While the YT data came nicely in a csv, the Video Game Trends took much more effort. With Brendan leading the charge, the team managed to scrape just over a year's worth of trending sales off of the website with Selenium and webdriver. This data was then broken down and subdivided by game name and the date it was trending.The game name would become the key that linked the VG and YT data together. 

This cleanup took a considerable amount of time. 

PostgreSQL
Once the tables were created, we created a Database using pgAdmin and inserted the dataframes into their respective tables using connection strings and Amazon Webservers to keep the database live.

We had to update the ER Digram along the way as plans changed, leaving us with this:

https://app.quickdatabasediagrams.com/#/d/2t2wGR

Finally, we broke everything down and made it into Github Pages which you can find below:

https://matkuhlm.github.io/CWRU_ETL_Project1/

Authors:

Brendan Rhoads (Team Lead)

Matt Kuhlmann (Web Designer)

Cristina Sheridan (Database Owner)
