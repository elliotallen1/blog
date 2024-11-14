---
layout: post
author: Elliot Allen
---

Boom! It is Week 3 for me at Disco Tray, and I am finally able to make some progress! The error storm has passed, and now I can actually see the website! So let's go through how we got here...

Okay so in the first week, we had no clue what was going on. The project was already in a weird state from the previous developers. My issues were with my localhos and my certificates, but at the time I thought it was just because the project was hectic. This was fine; we just needed to get it fixed. Right?

In week two, the project was fixed, but my issues were still the same. Since the problems were not with the project, they had to be coming from my machine. I tried countless things with my certificate. Deleted it. Tried to get a new one. Didn't work. Then one stack overflow post told me to do some stuff with my Keychain Access. So in the process of doing that, I accidentally deleted my entire keychain and it was very difficult to get back. 

In week three I was all out of hope. I had no clue what to do. Everything I was trying did not work, and I also had no direction for where to go next. I tried changing my browser over to Chrome. Didn't work. I tried to delete and reinstall all related software. Didn't work. Just when I was all out of hope, I opened [this link](https://learn.microsoft.com/en-us/answers/questions/1425240/microsoft-entra-keeps-throwing-idw10109-all-client) that Dr. Goadrich sent me. Down in the P.S. section, Alexander said that changing the ClientCertificates to ClientSecret in appsettings.json. I got the secret, and it actually worked!

Now that my nightmare is over, I can actually get started on the website. I am not very happy with the current styling of the website, so I think this will be m next venture. I will be making Moqups and sharing them with my team to see what they like. Then we can get the ball moving!