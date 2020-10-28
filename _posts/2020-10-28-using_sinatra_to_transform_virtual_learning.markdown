---
layout: post
title:      "Using  Sinatra to Transform Virtual Learning"
date:       2020-10-28 10:32:32 +0000
permalink:  using_sinatra_to_transform_virtual_learning
---


Let me preface this by saying, I have A LOT of friends in  the educational field. Ever since the start of COVID-19, they've mentioned how stressful it is to transition to virtual learning. Fast forward 7 months, and most of them are still teaching online; but the others are in person (while anticipating  another shutdown). While some schools have been preparing to potentially close again, other schools have not considered that possibility, leaving many teachers unsure of how to plan the rest of the year. 

Not only has it been stressful for teachers, but  many kids are losing the social and cognitive development due to being virtual, and not seeing their peers anymore. This has inspired my Sinatra Project, LeSin Plan. 

There are a few different goals for LeSin Plan:

1. Allow teachers to share lessons that  worked for them via virtual learning and in person
2. Help teachers  easier transition to virtual learning
3. Give students the  social  interaction they crave when they're not  physically going to school everyday (via the lessons picked/posted by teacher)

## Tying it All Together

I knew I needed a User class for the teachers, and a lesson class, and I knew a lesson would belong to a teacher, what I didn't know was  how  teacher's create lesson plans. Is it PDF, a word form, an image? Seriously, if  you're in the educational field let me know because I'm curious. Since I  was unsure, and all I had was Google, I decided  to allow teachers to upload lesson plans via an image. Under each lesson plan you can see what grade it's geared toward, the subject, and a little description. 

For teachers, in addition to their name, email, etc. I decided to also put in which state they teach for. Since each state has it's own curriculum, and standards, for kids to move up to the next grade. Eventually, for a better user experience, I plan on creating a route to filter by Pre-K, Elementary, Middle or High School, or by state.  

Another feature I'm happy about, is that I also provided the capability to allow anyon on a school staff, not just teachers, to utilize this. I'm sure it's hard  for the school psychologists and school social workers to keep up with their students as well. 

## The Struggle is Real
This project took me about a week-ish to complete. Two weekends spent coding and many late nights (even though I wake up at 5:30 for work), but I got it done. The biggest struggles for me during this time were the Patch and Delete  methods because I didnt *fully* do them correctly in any of the prior labs and felt so much uncertainty with them. I knew how the routes worked, I struggled with the HTML aspect  in t he  code. 

Luckily, another self-paced  student  recommended Ayana's video and it was like something suddenly clicked. I remember doing my own Patch and delete routes and I was thinking, "That was the only thing it was? The hidden input type with the `_method`  of `patch` or `delete`?" I felt so silly for not understanding sooner but I had such an issue with Sinatra. I think because there were so many little sections before the actual Sinatra section, it felt like a lot at once; but I understand now how they all tie in with the final project, and I'm happy I have a better understanding.

## Reaching the Finish Line.


Once completing the project, I began adding some CSS and making it look how I wanted it too, but I didnt want to rush it. I plan to continue styling this website, and giving it the look/feel I envision for it. I  hope one day this website gives teachers the capability to read other lesson plans, create lesson plans for teachers nationally, and help millions of students in the process. I'm sure teachers have these *secret* websites with resources, and  I'll ask my teacher friends one day, but for now, I'm just pretty damn proud of what I  created, and that's enough for me. 




