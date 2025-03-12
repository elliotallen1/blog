---
layout: post
author: Elliot Allen
---

This week was kind of just another week of waiting on this app. I started the week with emailing IT regarding permissions with Azure. It looks like we need to click the big scary button to allow Application permissions instead of Delegated permissions to get the app to send emails on behalf of the user. Since I was just waiting on IT to get back to me, I decided to focus on other issues in the project. 

The first issue I resolved was linking an email to the Request. Now, when a user submits a Request, their email is attatched to it. This will let the admin easily see who made the request in the app. I was not sure how to get the currently signed-in user, so I went to Google. Unfortunately, I was let astray... I tried going through an Identity route using a UserManager (?). I was not really sure what I was messing with and ended up making a huge mess in the code. It turns out, because of Azure AD, we can just get the user with 'User'. This made things infinetly easier, and now it all works!

After messing with that, I decided to go through some of the other minor issues in the app. First, I made the 'Need24Hours' field in the Request form default to 'No'. Then, I changed the Request tables. The Approve/Deny buttons were too tall, so I tried to change them to smaller icons. I liked the icons, but they were still too tall. I had to adjust the table styling to give more vertical space to the rows, and I also made the contents of the rows vertically aligned. Last, I made the 'Click here' link actually route to the Request form. 

This app is nearing the end (knock on wood). Once we come up with a plan for the emails, it should (should) be smooth sailing.