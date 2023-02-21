# RoomMatch
A web application made by me and 3 other students as a group project at the University of Pittsburgh. It's purpose is to help users find roommates by presenting them with a slideshow of other users, and an approve/disapprove button. It's matching mechanism allows users to only contact users they have mutually approved.
View it here at: https://cs1520-grouph.ue.r.appspot.com/
 Here is the homescreen, made using JavaScript for the animations and HTML/CCS. We also used flask templates and flask sessions to make each user's experience unique.
<img width="1426" alt="Screen Shot 2023-01-03 at 3 20 46 AM" src="https://user-images.githubusercontent.com/71620030/210325310-e06f27c8-43b2-41d8-a5fa-da63a37a3672.png">

Here we see an example of the process of finding a roommate. With this application, a user would see another user on their screen, and press the like or dislike button. They would then proceed to see the next user upon response. Each user would have a list of other users they liked and disliked on the back-end, saved on Google Cloud. The back-end would proceed to check if there are users mutually on each others list, and this would be displayed to each user privately on their profile. We were planning on working on a messaging system for these mutually matched users, but we ran out of time. We had trouble implementing this list due to the constraints in storage on Google Cloud. Each user entity held too much information after implementing the list. One work around would be to suppress some of this data, or store it into another database and this is something I would fix if I had more time to work on it.

<img width="1248" alt="Screen Shot 2023-01-03 at 3 28 37 AM" src="https://user-images.githubusercontent.com/71620030/210325300-ee241429-9eba-44c0-b4a4-8375578699eb.png">

Here we can see the Profile page. This is what I primarily worked on. My teammates and I worked together to implement Flask sessions so that users could log-in and log-out. I also designed the profile template and worked on the ability to edit the content of the page. One implementation that we had a really hard time solving was getting pictures to be able to be posted without being to big to be stored on Google Cloud's databases. We solved this by resizing the resolution and size of the pictures that were used as a profile picture.

<img width="1440" alt="Screen Shot 2023-02-21 at 1 36 14 PM" src="https://user-images.githubusercontent.com/71620030/220437644-94b38acb-1c86-43c5-bf1e-91fec58eaae2.png">


