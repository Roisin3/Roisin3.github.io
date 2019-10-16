---
layout: post
title:      "CLI Project"
date:       2019-10-16 02:59:37 +0000
permalink:  cli_project
---


Oh boy. This was nerve wracking. At the beginning of this project I was very initimidated. I had never scraped a website before, or built anything more advanced than a calculator!

I started by breaking this into parts. I need to scrape the website. I needed to organize the scraped data into something I could use. Finally I needed to build the interface to show the requested data to the user. 

**Scrape the Site**

This was an adventure. I had an idea of using my soccer team some how in the project off the bat. As I looked into the requirements a bit more I thought of using the standings from last season. I looked at the HTML and figured that it was scrapable and that I could use this.

The day I started the GCPL brought their website down to rebuild it. I spent the rest of the morning searching for a replacement. Eventually I found another 2019 season table and started working with that. It was different though, it had all the team stats, player stats, and schedule information in one large HTML table. This meant I didn't have clear tags to work with anymore. 

I took a look and only needed rows 1 - 18, 0 was headers and 19 started listing player data. I built a counter and scraper to gather the data of each team into an array and shovel those into a seperate array I could use to build my Team class. 

**Organize Data**

After creating the arrays from the scraped data. I had to organize it in a way that would make outputing it when requested easy and clear for me to work with, Each of the 18 teams has 8 stats, team name. games played, wins, losses, draws, points, goals for, and goals against. I knew all teams had these and they were all in this specific order. That made iterating through the array simple. It also gave me clear instance methods to initialze with, 

**Command Line**

Building the command line interface was my second big hurdle. After building the other parts I wasn't sure where to start with the user facing side, With that in mind I started thinking about how to ask the user to select a team. I ended up with printing a list of all the teams and having the user pick the correspoding number, After I had that built the rest came along relativly smoothly. I got the absolute barebones working, then I added things like "Please select a team" and "Welcome to GCPL table printer!" 

With those out of the way I began to think about edge cases like users entering invalid numbers and responses. I built the #choose_again method and a few if/else check to make sure everythign was valid. 


Finally, I was finished! Everything worked! In hindsight, I learned a lot about how to approach creating software. It was a good learning expierence to have this scale of project to start with, At some point, I would like to create a gem from this and use the gem tty-table to create a better table to hold the requested teams stats.

