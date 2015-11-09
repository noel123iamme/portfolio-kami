---
layout: post
title: Bloccit
thumbnail-path: "img/bloccit.png"
short-description: Bloccit is a Reddit replica for social networking and news posted and managed by registered users.
---

{:.center}
![]({{ site.baseurl }}/img/bloccit.png)

{:.center}
<a class="btn btn-default" href="http://bloccit-noel123iamme.heroku.com" target="_blank">Demo Site <span class="glyphicon glyphicon-chevron-right"></span></a>


### Summary

Bloccit is a Reddit replica for social networking and news posted and managed by registered users.

### Explanation

As my first Rails app, this project looks to touch on several key features of a web application.  It contains a landing page (Home), several navigation tabs for Topics, Popular Posts, Public User information.  We needed to build in features for user access (login/logout), user roles (admin, moderator, member, and guest).  Email authentication and notification.  Ability to upload image files. 

As the developer, I needed to build from ground-up a production class web applicaiton.

### Problem

The primary user stories were:

<ol>
  <li>Create Home, About, Topics, User pages</li>
  <li>Style my website so as to be more user friendly</li>
  <li>Create a Topics page where underneath you can have user posts.</li>
  <li>Create Posts under various Topics.</li>
  <li>Create Comments on Posts.</li>
  <li>The ability to Vote (up/down) on a given post.</li>
  <li>The ability to Favorite (unfavorite) a given Post.</li>
  <li>Create the ability to sign-in Users where users can  
    <ul>
      <li>Can create Topics, Posts, and Comments.</li>
      <li>Can create private Posts</li>
    </ul>
  </li>
  <li>Create user authoriations where some users can be designated as:
    <ul>
      <li>Admin with full access to all Topics, Posts, and Comments</li>
      <li>Moderator with ability to manager content within a given Topic</li>
      <li>Member with ability to create public and private posts and comments</li>
      <li>and, Guest with ability to create public posts</li>
    </ul>
  </li>
  <li>Create ability for users to upload an avatar image of themselves.</li>
  <li>Create ability for users to upload images for their posts</li>
  <li>Ranking Topics by number of Posts and Comments</li>
  <li>Ability to send user an email when favoriting a post</li>
  <li>Ability to send an email to the user of a favorited post when another user posts a comment.</li>
  <li>User public profile page to show public Posts and Comments for a given user</li>
</ol>


### Solution

* GitHub to maintain the souce code
* Heroku to host production copy of the web app
* PostGres SQL for the production database
* SendGrid to handle email
* Bootstrap CSS for styling the site
* Amazon AWS S3 for storing image files for the site
* RSpec for test-driven development

* Some technologies used in the application development
  - Faker provides a way to generate sample data
  - Devise provides a full-featured authorization system for creating and authorizing users
  - Figaro provides a way to manage application private IDs and KEYs for prodution deployment
  - Pundit provides a way to manage user views and access to content through policy scopes
  - Redcarpet provides a way for users enter html-style posts and comments using "markdown" syntax.
  - CarrierWave provides a way to upload and store image files.
  - MiniMagic provides a way to manipulate images within the web application.
  - Will-Paginate provides a way to create paging of long lists of topics and posts

### Results

A working, production web application

### Conclusion

As my first Ruby project, this was a difficult and challenging task to say the least.  Learning Ruby syntax and the Rails framework was an expecially difficult task coming from a long time Microsoft VB.NET developer.  Thankfully, my mentor, the Bloc Stack Exchange, fellow students, Ruby developer community, and Google helped make finding answers possibles.