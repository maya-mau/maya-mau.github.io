---
layout: page
title: NewWithTags
description: A fashion-based social media platform for users to share outfit pictures and track fashion trends by location. 
img: assets/img/newwithtags/my_posts_page.png
importance: 3
category: work
related publications: false
---

In CS 304: Databases and Web Interfaces, I completed my first full-stack application in a team of four. We created NewWithTags, a fashion-based social media platform that would allow users to post outfit pictures and tag them by location and aesthetic. Once the site was populated with posts, users could sort posts by geographical and aesthetic tags to track trends by major city. 

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/newwithtags/main_page.png" title="Home page of NewWithTags web application" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="caption col-sm-4">
        The home page of the NewWithTags web application, showing a logo in the top left (NWT), a collapsed search bar underneath, and a row of three posts of various people in outfits. 
    </div>
</div>

We used MongoDB for the backend database and Javascript, HTML/CSS, and Bootstrap for the frontend application. The design (logo, color scheme, buttons, etc.) was first outlined in Figma before implementation. 

<div class="row">
    <div class="col-sm mt-2 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/newwithtags/copenhagen_post.png" title="A post of a person in Copenhagen standing next to a field in a red cardigan and floral skirt." class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-2 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/newwithtags/paris_post.png" title="A post of a person in Paris walking down a cobblestone street wearing black slides, white pants, and a dark top. They are carrying two bouquets of flowers." class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The NewWithTags application has a few main pages: the home page, login/sign up page, create page, and individual post pages. When first opening NewWithTags, users are shown the home page where all posts are displayed. Posts can be sorted by most liked/recent, or filtered by city/trend. Once clicked on, posts are given their own page where users can see a caption, comments, likes, and interact with the post if they are logged in. 


<div class="row">
    <div class="col-sm-6">
        <p>Users can either create a new account or log into an existing one. Passwords are encrypted using bcrypt and usernames must be unique. If the username or password is incorrect on login, an error message will appear using flashes. Examples of error messages a user can receive are shown on the left. Once a user is logged in, they can view their own posts and posts that they've liked.</p>
        <p>More robust error messaging would be helpful to inform users of the application state, and may be necessary if this application was launched.</p>
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/newwithtags/login_error.png" title="The login/sign up page with a message reading, 'Login failed. Check your username and password and try again.' at the top of the page." class="img-fluid rounded z-depth-1" %}
        {% include figure.liquid loading="eager" path="assets/img/newwithtags/search_error.png" title="A message reading, 'Sorry, this city does not exist.' underneath the expanded search bar where 'new york' is misspelled." class="img-fluid rounded z-depth-1" %}
    </div>
</div>

One of the challenges of this project was integrating sorting with filtering in the backend database. We used aggregation pipelines to fetch data from the database, which were complex but worked well when implemented. While we only learned MongoDB, a NoSQL database, it fit our social media application use-case. If this application was launched, we might need to shard the database across multiple servers to distribute load and improve performance, depending on the number of users and frequency of use. 

<div class="row">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/newwithtags/my_posts_page.png" title="My posted and liked posts page." class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="caption col-sm-4">
        The profile page of the NewWithTags web application for users that are logged in, showing a logo in the top left (NWT), profile details, and buttons to show the user's created and liked posts. 
    </div>
</div>

Because NewWithTags was a final project was for a full-stack web development course, every member of the team contributed to all levels of the stack. I was responsible for certain sorting capabilities and backend database structures, and created the script to reset and populate the database with sample posts, users, comments, and likes--something that enabled us to experiment with features while retaining a polished version of the application for presentation. 
