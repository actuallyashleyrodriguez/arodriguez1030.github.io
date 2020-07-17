---
layout: post
title:      "Does the "I" in CLI Stand for Imposter Syndrome?"
date:       2020-06-25 21:27:50 -0400
permalink:  does_the_i_in_cli_stand_for_imposter_syndrome
---


My very first project is here! I have to say I was extremely excited to get to this point, but at the same time there was a lot of doubt. There was the feeling of "Can I do this alone?" "Without Flatiron's tests will I be able to know what to do?" and "What if I completely fail? What would I do?". Obviously that's not the right mindset to have when you're getting into anything, but the imposter syndrome was hitting me hard! Luckily, I knew exactly what I wanted to do and how I wanted it to come out! With COVID and thousands of people out of work, I wanted to find the top cities hiring for software engineering positions for June of 2020, and I had this elaborate idea of what information I wanted to output once you selected a city. !

Jokes on me! Of course my carefully thought out vision came to a screetching hault when every single website that had the information I was looking for was not scrapable! I spent more hours finding the right website to scrape, than I actually did scraping the website (funny enough that part came *easier* to me). Two days, and I lost track of how many websites later, I finally found ***the one***. You know those scenes in movies, when the clouds part and there's the moment when everything turns around. Well, that was that moment for me. I was so excited, I could FINALLY finish my flow-chart and planning, but most important I could FINALLY start my code. Can I get a woot woot? (**woot woot!**)!![](https://thecarousel.com/wp-content/uploads/2020/01/woman-stands-on-mountain-over-field-under-cloudy-sky-at-847483-1152x768.jpg)(Visual representation of me finding the website for my code.)


## The Code Part (DUNN DUNN DUNNNN)
I was super excited to start my project, but I wasn't sure ***where*** to start. Luckily, Flatiron has tutorials for days on the CLI (Eden Events is a great one to reference if you're in need of assistance). Personally, the rest of the project was fairly simple and easy, since I already had an idea of how I wanted the flow to go (shout out to the flow-chart that was part of the planning requirements!). My plan was now to output the top 10 cities hiring software engineers, then you would either select the average salary for engineers in the city or you would make a selection to see the top 3 companies hiring. 

After I created my bundle, and got a few necessary items out of the way, I began by scraping the website. Even though I found the perfect website I was able to scrape, a lot of the paragraphs were labeled the same. In order to scrape the right information I needed to input specific markers to identify what I was looking for. For instance the method for both salary and top companies hiring were `website.css ("p a")` so I had to iterate through and specify if the text included "$" it would be a salary, and if the link included "cmp" it was a company. I tied in the scraped information in with a `TopTechCities::City` class, where each city had a name (obviously), a salary and companies hiring. 

Now comes the part that gave me gray hair. My bin folder called on `TopTechCities::CLI.new.run_app` to run my project, that was the easiest part. In the `TopTechCities::CLI` class however, a majority of my time was getting the code to output the items exactly the way I wanted, which just meant googling different methods to get me where I wanted to go. I created a method to output my cities and give them an index, but most of the code was listed into one method `#get_city`.It was initially only supposed to be a method to get the city the user selected, so then then they could see the menu items within the city, but once the city was selected, I got lazy and didn't want to have to re-input that code so I kept everything in that method. 

Looking back, that might've been my downfall. since I had multiple user inputs within the same method, I wasn't able to exit the app from the initial cities menu. In order to exit you had to select a city first and then exit from the menu within the city. When I tell you I spent days on it before giving up, I spent DAYS! This is how I felt when I was on day 2 of trying to make exit work on both menus:

![](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQSBkMD-cWGyh3BHDREbMmilKk-9qTF5Ugnow&usqp=CAU)


I submitted it without figuring out the issue, and it honestly still bugs me. I randomly go back and try something else that (surprise) doesn't work. In the end, that was my only major concern, so I shouldn't be too hard on myself. Although I was terrified going into this, and was doubting my abilities, I realized I know a lot more than I thought I did. The doubt I had in the beginning of the project, made the completion of it so much sweeter! I'm very proud of myself for making something from scratch, and it makes me even more excited to get to the next projects! 



