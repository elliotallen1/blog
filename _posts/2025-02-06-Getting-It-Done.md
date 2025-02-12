---
layout: post
author: Elliot Allen
---

We have been working on the SOS Resources project for a while, and it still requires some work. Since this was the first week of the new semester our team decided that we really needed to get this project done. Our goal is to get it done by mid-February.

I was looking over the project during our meeting, and a realised that the requests were never actually being stored in the database. All of the information for the requests were just being stored in an email. I figured that this was not the desired behavior for this project, so I raised the question of how do we change our database to store requests. This led me to creating a new schema.

I changed the models for the Resource class, and added a Request class. A Resource is now represented as a Name, Type, Description, and Quantity. The Type was previously a string, but I changed it to be an enum. This way is cleaner plus it will make it easier to do implement logic for when the Type of the Resource is a Textbook.

I think this is a good foundation for the rest of the project. Now we just need to get our database working like it should. There is still a lot to do on this project, but if we all put in effort then it should wrap up nicely.