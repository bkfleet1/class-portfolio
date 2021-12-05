# CHALLENGE 2 PORTFOLIO WEBPAGE

# Acceptance Criteria
The following items requirements were provided as the scope of work and acceptance criteria.

### Item 1
> - WHEN I load their portfolio
> - THEN I am presented with the developer's name, a recent photo or avatar, and links to sections about them, their work, and how to contact them

### Item 2
> - WHEN I click one of the links in the navigation
> - THEN the UI scrolls to the corresponding section

### Item 3
> - WHEN I click on the link to the section about their work
> - THEN the UI scrolls to a section with titled images of the developer's applications

### Item 4
> - WHEN I am presented with the developer's first application
> - THEN that application's image should be larger in size than the others

### Item 5
> - WHEN I click on the images of the applications
> - THEN I am taken to that deployed application

### Item 6
> - WHEN I resize the page or view the site on various screens and devices
THEN I am presented with a responsive layout that adapts to my viewport


# Site Code
The following narrative details the developer's notes for the portfolio website challenge to conform with the acceptance criteria. Moreover, the hyperlinks below provide further supporting materials for site development.
> - Deployed code: https://bkfleet1.github.io/class-portfolio/
> - GitHub repository: https://github.com/bkfleet1/class-portfolio 

Other links
> - Project writeup: https://bkfleet1.github.io/class-portfolio/assets/documents/portfolio.pdf 



# Repository
The developer performed the following steps to initiate the project.

1.	Logged into developers GitHub portal
2.	Created a new repository named "class-portfolio" and a readme.md file
3.	Enabled the repository’s web page features, which are found under the repository’s settings > pages
4.	Opened Git Bash terminal entered the following commands:
> - cd to desktop/projects
> - git clone git@github.com:bkelley1/class-portfolio.git
> - git checkout -b develop (create develop branch)
> - touch index.html (create index.html file)
> - touch .gitignore (create .gitignore file)
> - mkdir assets (make directory assets)
> - cd assets (change directory to assets)
> - mkdir images (make directory images)
> - mkdir documents (make directory documents)
> - mkdir css (make directory css)
> - cd css (change directory to css)
> - touch style.css
> - cd ../../ (change directory to local repository root)
> - git add - A
> - git commit -m "initial portfolio commit"
> - git push origin develop
> - git checkout main
> - git merge develop
> - git add - A
> - git commit -m "initial portfolio commit"
> - git push origin main
> - git checkout develop

At this point the development environment on the developer’s local machine and GitHub repository were established and ready for development. Below is a screen capture of the class-portfolio repository.
 [portfolio repository](./assets/images/repository.png) 

# Site Structure
The portfolio site essentially consists of the following structure.

> - head
> - body
> - header
> - section class=”hero”
> - section class="about-section"
>> - div id="aboutme" class="about-box"
>>> - div class="about"
> - section class="projects-section"
>> - div id="projects" class="projects-box"
>>> - div class="projects-group"
>>>> <!- applies to project 1 only ->
>>>> - div class="first-project"
>>>>> - div class="project-links"
>>>> <!- applies to project 1 only ->
>>>> - div class=”projects” 
>>>>> - div class=”project-links”
>>>> <!- applies to all future projects ->
>>>> - div class=”projects” 
> - footer id=”contact”
>> - div class="contact-box"
>>> - div class="contact"
>>>> - iframe (google maps)
>>>> - address

The following graphic further illustrates the site structure.
  [portfolio site architecture](./assets/images/portfolio-design.png) 

# Developer's Notes
The acceptance criteria previously noted is addressed in the following manner.

### Item 1
> - WHEN I load their portfolio
> - THEN I am presented with the developer's name, a recent photo or avatar, and links to sections about them, their work, and how to contact them

The site header contains an avatar with the developer’s name. Additionally, the header contains a nav section with an unorganized list that contains hyperlinks to the following sections. IDs were used to link the list elements below to their relevant section.

>> - about me - contains a photo and background information about the developer. 
>> - projects - contains sample work products completed by the developer as well as place holders for other projects
>> - contact - contains the developer’s contact information
 [header nav code](./assets/images/header.png) 

### Item 2
> - WHEN I click one of the links in the navigation
> - THEN the UI scrolls to the corresponding section

As illustrated below. the developer added the following IDs to link the navigation menu in the header to their relevant sections. 

about me
'''  <section class="about-section">
     <div id="aboutme" class="about-box"> '''

projects
'''  <section class="projects-section">
    <div id="projects" class="projects-box"> '''


contact
''' <footer id="contact"> '''

### Item 3
> - WHEN I click on the link to the section about their work
> - THEN the UI scrolls to a section with titled images of the developer's applications

The following screen capture illustrates the projects section with images, titles, and a brief description of each project.
 [project section](./assets/images/project1image.png) 

### Item 4
> - WHEN I am presented with the developer's first application
> - THEN that application's image should be larger in size than the others

The following screen capture illustrates the larger image size of the first project cited.
  [project 1 larger image](./assets/images/project1image.png) 

### Item 5
> - WHEN I click on the images of the applications
> - THEN I am taken to that deployed application

The deployed code is accessible at https://bkfleet1.github.io/class-portfolio/

### Item 6
> - WHEN I resize the page or view the site on various screens and devices
> - THEN I am presented with a responsive layout that adapts to my viewport 

The developer used media queries contained in the CSS to resize site elements at 980px and 768px resolution. The following screen capture illustrates sizing at 856px.
 [site mobile responsiveness](./assets/images/responsiveness.png)










