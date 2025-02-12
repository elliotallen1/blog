---
layout: post
author: Elliot Allen
---

This week was a little bit better than the rest. For once, I sat down, knew what I needed to work on, and worked on it. I spent last week updating the Request and Resource models as well as thinking more about our database schema. With the new models, I generated new pages to perform CRUD operations. The pages were generated and everything, but they were not super functional (especially the Create page for the requests). This week, my goal was to get that working. I wanted to actually create a new request and be able to view it on the Index page.

So I got to work and got it done. I looked back at previous projects to see how I did it back then and if I could apply the same concept to this project. After working on it for a while, it still was not working. For some reason the ModelState was always invalid, so the request never got created and I never left the page. I think it must have been an issue with how the resource was being saved to the request, but I could never figure out what it was. Finally, I added this line 'ModelState.Remove("Request.Resource");' to bypass the isValid check. I know this is probably not a good way of doing it, but it works so I am not going to touch it.

After getting that to work, I had to go throughout the website and adjust some things here and there. I made the Request table display all the correct information and merged it into the main repo.

Then, I decided to add a Status to the Request. It could be 'Pending', 'Approved', or 'Denied'. A request always starts at 'Pending', but an admin should be able to come in and Approve/Deny the request. I added buttons next to each request on the table to achieve this functionality. We do not have Admin roles set up yet, so anyone can click these buttons but the functionality is there.

Going forward, it looks like we need to prioritize a few things. We need User/Admin roles, a Student field for the request to see who requested it, an email notifier for when there is a new request, and sorting/filtering the request table.