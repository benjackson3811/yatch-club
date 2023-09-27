<a name="top"></a>

# Milestone project 5 Frontend

--- 

This project has its own backend API. The link to this repository is [Yatch-Club-API](). 

Live Website

View Live Wesbite here: ####

---

### Am i response image

--- 

### Table of Contents

- [Project purpose and description](#project-idea-and-description)
    - [Project Idea](#project-objective)
    - [Site owner goal](#site-owner-goal)
    - [Site user goal](#site-user-goal)
- [User Stories](#user-stories)
    - [Profile and account management](#profile-and-account-management)
    - [Event](#events)
    - [Rating](#rating)
    - [Comment](#comments)
    - [Navigation and authentication](#navigation-and-authentication)
- [Features](#features)
    - [Navbar](#navbar)
    - [Sign up](#sign-up)
    - [Sign in](#sign-in)
    - [Feed](#feed)
    - [Events Data](#events--homepage)
    - [Event Detail](#detailed-event)
    - [Create Event](#create-event-form)
    - [Profile](#profiles)
    - [Follow / Followed](#follow---followed)
    - [Comments](#comments)
    - [Categories](#categories)
    - [Footer](#footer)
    - [User features](#user-interaction--information-popups)
    - [Future features](#future-features)
- [Structure](#structure)
    - [Database](#database)
    - [Wireframe](#wireframes)
- [Typography and color scheme](#typography-and-color-scheme)
- [Technologies Used](#technologies-used)
    - [Languages](#languages)
    - [Frameworks](#frameworks)
    - [Database](#database-1)
    - [Tools](#tools)
- [Methodology](#methodology)
    - [Agile Project Management](#agile-project-management-with-github-projects)
    - [User Stories and github](#user-stories-as-github-issues)
    - [### Bug Tracking](#bug-tracking)
    - [### Iterative Development Approach](#iterative-development-approach)
- [Planning & Documentation](#planning--documentation)
    - [Backend](#backend)
    - [Frontend](#frontend)
    - [Reusable Components](#reusable-components)
    - [Testing](#testing)
    - [Documentaion](#documentation--readmemd)
- [Testing](#testing)
- [Programs and tools used](#programs-and-tools-used)
- [Deployment](#deployment)
- [Credits](#credits)

--- 

### Project purpose and description

Yacht Club is a website for a fictional yatch club based in the UK. 

[Wikipedia] (https://www.wikipedia.org/) defines the purpose of a "yacht club is to celebrate boaters and the sport of yacht racing, sailing, and cruising. What Is A Yacht Club? A yacht club is a social membership sports club for boaters."

This website allows users to view and share pictures of trips taken and future trips with the Yatch club. The website functionality is designed to allow this user to search shared photos of the trips, like them and add comments to share their experiances and feedback. 

The Yacht Club website has been created as 5th Portfolio project for the Code Institutes fullstack developer program. 

The website is designed as a browser-based interface to enable;
- users to create, read, comment and vote on shared content.
- content to be searched and catergorised.
- search results can be filtered on username, popularity, date created, title, content keywords and category. 

The project is built using React, JSX, (HTML, Javascript and CSS), specific frameworks and libraries (detailed in a below section) and connected to a separate backend API (also built for this course).
---

### Site owner's goal

My family are keen sailers and belong to sailing club that allows them to sail all around the UK and Northern Europe. At the minute the only place they can share their pictures is Facebook. I wanted to create a place where they could share their pictures, memories and feedback on old trips.

---
### Site User's goal

- To create a website for club members to share their trip pictures to club members. 
- To allow the club to show pictures of the previous adventures the members have been on. 

---
### User Stories

The below user stories have been defined for the project.
#### Navigation 
- [] Navigation: As a user I can view a navbar from every page so that I can navigate easily between pages.
- [] Navigation: Conditional rendering - As a logged out user I can see sign in and sign up options so that I can sign in/sign up.
- [] Routing: As a user I can navigate through pages quickly so that I can view content seamlessly without page refresh

#### Authentication
- [] Authentication - Sign up: As a user I can create a new account so that I can access all the features for signed up users.
- [] Authentication - Sign in: As a user I can sign in to the app so that I can access functionality for logged in users.
- [] Authentication - Logged in Status: As a user I can tell if I am logged in or not so that I can log in if I need to.
- [] Authentication - Refreshing access tokens: As a user I can maintain my logged-in status until I choose to log out so that my user experience is not compromised.
- [] Avatar: As a user I can view user's avatars so that I can easily identify users of the application.


#### Adding & Liking a Trip
- [] Create Trips: As a logged in user I can create Trips so that I can share my images of completed sailing trips!
- [] View a Trip: As a user I can view the details of a single trip picture so that I can learn more about it.
- [] Like a Trip: As a logged in user I can like a shared trip so that I can show my support for the trip that interest me.


#### The Posts Page
- [] View most recent Trips: As a user I can view all the most recent Trips, the most recently created shown first so that I am up to date with the newest content.
- [] As a user, I can search for specific trips with keywords, so that I can find the trips and user profiles I am most interested in.
- [] View liked trips: As a logged in user I can view the trips I liked so that I can find the trips I enjoy the most
- [] View trips of followed users: As a logged in user I can view content filtered by users I follow so that I can keep up to date with content.
- [] Infinite scroll: As a user I can keep scrolling through the images on the site, that are loaded for me automatically so that I don't have to click on "next page" etc


#### The Post Page
- [] Trip page: As a user I can view the trips page so that I can read the comments about the post
- [] Edit post: As a post owner I can edit my post title and description so that I can make corrections or update my post after it was created
- [] Create a comment: As a logged in user I can add comments to a post so that I can share my thoughts about the post
- [] Comment date: As a user I can see how long ago a comment was made so that I know how old a comment is
- [] View comments: As a user I can read comments on posts so that I can read what other users think about the posts
- [] Delete comments: As an owner of a comment I can delete my comment so that I can control removal of my comment from the application
- [] Edit a comment: As an owner of a comment I can edit my comment so that I can fix or update my existing comment

#### The Profile Page
- [] Profile page: As a user I can view other users profiles so that I can see their posts and learn more about them
- [] Most followed profiles: As a user I can see a list of the most followed profiles so that I can see which profiles are popular
- [] User profile - user stats: As a user I can view statistics about a specific user: bio, number of posts, follows and users followed so that I can learn more about them
- [] Follow/Unfollow a user: As a logged in user I can follow and unfollow other users so that I can see and remove posts by specific users in my posts feed
- [] View all posts by a specific user: As a user I can view all the posts by a specific user so that I can catch up on their latest posts, or decide I want to follow them
- [] Edit profile: As a logged in user I can edit my profile so that I can change my profile picture and bio
- [] Update username and password: As a logged in user I can update my username and password so that I can change my display name and keep my profile secure

---

### Wireframes

#### Homepage.    
![Screenshot](src/images/Wireframe_index.png)    

#### Event detail view.     
![Screenshot](src/images/Wireframe_detail_event.png)     

#### Calendar view.    
![Screenshot](src/images/Wireframe_calendar.png)     

#### Sign up.     
![Screenshot](src/images/Wireframe_signup.png)     

#### Sign in.     
![Screenshot](src/images/Wireframe_signin.png)     

#### Profile.     
![Screenshot](src/images/Wireframe_profile.png)  

#### Map.     
![Screenshot](src/images/Wireframe_map.png)  



## Typography and color scheme

#### Design Choices

#### Colour

![screenshot](src/assets/color-palette.png)    

Categories palette.   
![Screenshot](src/images/category_colors.png)      

#### Fonts and Typography

- Roboto font used on site, fall back font is sans-serif. Example of Roboto font from
[m1.material](https://m1.material.io/style/typography.html#)     
![screenshot](src/images/roboto_font.png)

[Back up](#table-of-content)

---

## Technologies Used

### Languages

- HTML / JSX (JavaScript XML)

- CSS

- Python

- Javascript

### Frameworks

- Django: A high-level Python web framework used for building the Recipe Collective website.

- React: A JavaScript library for building user interfaces. It is commonly used for creating dynamic and interactive components in web applications.

- Cloudinary: A cloud-based media management platform used for storing and serving images in the Recipe Collective project.

### Database

- ElephantSQL: ElephantSQL is a PostgreSQL database as a service. It is used as the database for the Recipe Collective project, providing a reliable and scalable storage solution for the application's data.

### Tools

- Git: A distributed version control system tracking project source code changes.

- GitHub: A web-based hosting service for version control repositories for storing and managing the project's source code.

- Gitpod: An online integrated development environment (IDE) used for developing and testing the Recipe Collective project.

- Heroku: A cloud platform that enables deployment and hosting of web applications. Heroku was used for deploying the Recipe Collective project to a live server.

- Balsamiq: A wireframing tool for creating mockups and prototypes of the Recipe Collective website.

- Lucidchart: Lucidchart is a web-based diagramming tool that offers a wide range of diagramming capabilities, including ER diagrams. It provides an intuitive interface and collaboration features, making it suitable for individual and team use.

- Google Fonts: A collection of free and open-source fonts used for typography on the Recipe Collective website.

- Font Awesome: A library of icons used for adding scalable vector icons to the Recipe Collective website.

[Back up](#table-of-content)
### Credits

- [Wikipedia] (https://www.wikipedia.org/) - used for the description of a yacht club.