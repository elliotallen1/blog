---
layout: post
author: Elliot Allen
---

Boom! Alright I am back. 

Okay so the website is MOVING! This week was huge in terms of adding new features to the website. Now the users have a profile form that has a lot of information about the user. The user NEEDS to fill out this profile form before they are able to make any requests. Also, Ryan and I were finally able to present our progress to Christy Coker! The meeting went very well, and I will talk more about it later in this post. 

Alright, so adding the profile was a little bit challenging... The challenge was to get all of the pieces of the website connected using the logged in user's email (their Hendrix email). I had to use their email as a primary key for the Profile and a foreign key for the requests. This caused some more issues because SQL does not like non-integer keys. That issue was an easy fix - I just had to add some extra information to the db context. Anyway...

Yeah, so users have a profile now. This took longer than it should have because I did not do a lot of planning with the models. Before I knew to use the email as a foreign key, I tried to store the whole Profile in a Request. This is obviously silly and did not work, but I already scaffolded all of the pages. There were a lot of migrations run that night...  But, I figured out how the models should look, and now it all works perfectly! 

Next, the meeting with Christy went very well! She was very impressed with what we had to show her, and she was incredibly thankful. I also just enjoyed chatting with her. She did give us some suggestions. We need to change the name from SOS to SOAR (SOS no longer has funding). Sending an email notification when a request is approved/denied would be nice to do, but it may just not be possible. She also wants us to be able to request multiple resources at a time. 

I am glad to be making noticable progress on this website now. I always like presenting to people because I actually get to see how useful my work actually is for people. The work can be frustrating and difficult, but It is worth it to see how much easier it can make things for other people.