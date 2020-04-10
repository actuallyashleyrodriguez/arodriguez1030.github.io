---
layout: post
title:      "Coding During Covid?"
date:       2020-04-10 16:02:26 +0000
permalink:  coding_during_covid
---


So amidst all the craziness of COVID19, I've decided to use this time to continue learning to code. Honestly, the more I work on it, the more confident I feel in my decision, so that's a plus! This week I'm going to explain how to complete one of the labs I've finished this week. I want to get into the habit of explaining my code and the reason behind the code layout. The lab I'll be discussing is the "If Statements Lab" because I was super close in getting the code perfectly, but I literally missed one thing that ruined the entire test from passing (isn't that so frustrating when that happen?!). So essentially the goal of this lab is to define a method, `#speak_to_grandma` and using `if`, `elsif`, and/or `else` statements to pass the test. Since Grandma is hard  of hearing, we're looking to see if the speaker is talking normal, or shouting. If the user is talking normally, we want grandma to respond `HUH?! SPEAK UP, SONNY!`, if they're shouting Grandma responds `NO, NOT SINCE 1938!` (because of course grandma didnt actually  hear you) and lastly if you say `I  LOVE  YOU GRANDMA! ` exactly,  then Grandma says `I LOVE YOU TOO PUMPKIN!`. 

# **The Breakdown**
*** Let's create our method, we're doing to define `#speak_to_grandma`. Since we're comparing what is being said to Grandma, the method is going to have a string as an argument. It's  going to look  like this:**

```
def speak_to_grandma(string)

end
```

*** That's  the shell of our method now let's get to the meat and potatoes of the code. We know from the objection of the code the purpose is to use if/else statements. We want to see if the speaker is shouting or talking normally, however if they are shouting we want to see if they're shouting `I LOVE YOU GRANDMA!`  exactly. I'm going to compare that string first,  and I'll explain why in the next section. So we will be using `==` to compare the string for an exact match. **

```
def speak_to_grandma(string)
if string == "I LOVE YOU GRANDMA!"
"I LOVE YOU TOO PUMPKIN!"
end
end
```

So what I'm saying up there is if my string says`"I LOVE YOU GRANDMA!"` exactly, then grandma will respond with `"I LOVE YOU TOO PUMPKIN!"`.  Don't forget in addition to the method needing an `end`, everytime you add an `if` statement it needs an `end` also. 


*** Bam! One down, two more to go! We got this! Next we're going to see if the person is shouting, and if they are, grandma will respond with `NO, NOT SINCE 1938!`. We're going to use `.upcase` for this, which is basically makes all the letters capital; but instead of making it capital we're going to use the comparison operator again to see if the string is all capital letters (`string == string.upcase`). Still with me? Great! **

```
def speak_to_grandma(string)
if string == "I LOVE YOU GRANDMA!"
"I LOVE YOU TOO PUMPKIN!"
elsif string == string.upcase
"NO, NOT SINCE 1938!"
end
end
```

 Have you figured out why we compared `"I LOVE YOU GRANDMA!"` before we compared the string to `string.upcase`? It's because if we were to do `string.upcase` first `"I LOVE YOU GRANDMA!"` would respond with `"NO, NOT SINCE 1938!"` since the speaker is shouting, that will pass as `true` and never make it to the next line. Makes sense? 

*** Last one! LET'S GO!! Alright so, we've already said if speaker says `"I LOVE YOU GRANDMA!"` respond with this, and if they're shouting respond with this. If they're not shouting, Grandma can't hear you so we're going to use an `else` statement to say anything else Grandma is going to respond with `"HUH?! SPEAK UP, SONNY!"`.  So our final product will look like this:**

```
def speak_to_grandma(string)
if string == "I LOVE YOU GRANDMA!"
"I LOVE YOU TOO PUMPKIN!"
elsif string == string.upcase
"NO, NOT SINCE 1938!"
else
"HUH?! SPEAK UP, SONNY!"
end
end
```

And that's it! My mistake was that I didn't compare my string to `string.upcase` so everything that passed through the elsif statement passed as true because I was making them all capital! A small mistake, but it makes sense when you think about and what you're telling Ruby to do. 

Welp, that's all for this week, folks. Sorry for being extremely long winded (I am a natural talker so I tend to ramble). I hope I was able to help though! See you next time! 
