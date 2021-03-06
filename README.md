

# DUKEY'S BREWS

![Meda Screens](assets/images/meda-screens.png)


[Dukeys Brews Live Site](https://0osaraho0.github.io/Dukeys/)

# Table of Contents

- [About](#about)
- [User Experience (UX)](#user-experience--ux-)
- [Wireframes](#wireframes)
  * [Colour Schemes](#colour-schemes)
  * [Typography](#typography)
  * [Imagery](#imagery)
- [Features](#features)
  * [Existing Features](#existing-features)
  * [Features left to implement](#features-left-to-implement)
- [Existing Bugs](#existing-bugs)
- [Fixed bugs.](#fixed-bugs)
- [Testing](#testing)
  * [Wave Test](#wave-test)
  * [Jigsaw test](#jigsaw-test)
  * [Lighthouse Tests](#lighthouse-tests)
  * [Nu Html Checker](#nu-html-checker)
- [References and Acknowledgments](#references-and-acknowledgments)
- [Technologies Used](#technologies-used)
- [Deployment](#deployment)
- [Personal Devlopment](#personal-devlopment)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>


# About

This website is aimed at home brewing enthusiasts.  The owner of the website wishes to share his home brew recipes and home brewing ideas and have a space for other home brewing enthusiasts to be able to make contact and subscribe to his news letter.


# User Experience (UX)

before starting the website I sat down with the owner and discussed what he wanted to see from his website.

Site owners goals
- It needed to be easy to navigate
- It needed a contact or chatroom style section so that he could meet other beer enthusiasts.
- He wanted a section to show some of his recipes.
- He would like a blogging section so that in the future he could add to it when he next brews.

we rated these goals on a scale of 1 to 5 in importance and feasibility

| Goal | Importance | Feasibility |
|---| ---|----|
|Easy to navigate|5|5|
|Chatroom|2|2|
|Contact page|5|5|
|Recepies|5|5|
|Blogging|3|1|
|Gallery|1|5|

After looking at the feasibility of the goals we decided to go ahead with making the website but to leave out the blogging page and the chat room section of the contact page for the initial update.  My skills as a developer are not quite at that stage yet and the owner does need to do that right away anyway.  The owner also does not have many pictures at this time so decided to leave the gallery for a later update as well.

With this in mind we decided to go for a front page with a link to his recipes and a contact page.

# Wireframes

Please see the initial wire frames for this site.

![Wireframe Front Page](assets/images/wireframe-home-page.png)
![Wireframe Recipe Image Page](assets/images/wireframe-recipe-front.png)
![Wireframe Recipe Image Hover](assets/images/wireframe-recipe-back.png)
![Wireframe Contact Page](assets/images/wireframe-contact.png)


After going over the wireframes with the website owner we decided to go with beer glasses rather than bottles and a dark background with light writing.

---

## Colour Schemes

The owner wanted a masculine feel to the page, and I felt the site needed a clean look to it. I have decided to go for a simple colour scheme of #202020 and #fff8dc to facilitate this.  
![#202020](assets/images/202020.png)
![#fff8dc](assets/images/fff8dc.png)

I also went for Amber as the image background colour in case the image doesn't load.  This is to create contrast with the h2 on the contact page and because it is beer coloured.

![Amber Background](assets/images/contact-amber-background.png)

---

## Typography

I have used the fonts Bebas Neue for my h1 and h2s on my recipe cards as it is bold, eye catching and clean looking.
I have used Georama for the rest of the font because it also has a clean look and is easy to read.
I used Helvetica and Georgia for my back up fonts because they look similar.

---

## Imagery

The images used on the home and contact pages are inviting for thirsty beer enthusiasts that get excited over a refreshing pint of beer. 

![Home page hero image](assets/images/small-hero-image.png) ![contact background image](assets/images/small-contact-img.png)

---

I used beer glasses on the recipe page rather than the bottles in the wireframes because they look more homely and inviting than the bottles.  It also has the name of the beer in bold underneath.

![Example Glass](assets/images/small-sample-glass.png)

---

The recipes have a white boarder around them to give them a nice finish that matches the edge of the pictures. Both pictures and recipes have a 10px radius to give nice rounded corners.

![Recipe Card](assets/images/recipe-card.png)

---

# Features

## Existing Features

- The header is visible on every page and has a consistent design throughout.
- The menu bar is available at the top of every page, this gives the user ease of navigation when moving to different pages on the site.

![Header](assets/images/header-snip.png)

---

- The tagline "Lets Brew.. Some Beer" informs the user the site is about brewing beer and links straight to the recipe page when clicked.  This promotes ease of use for site navigation.
- The hero image is of a pint of beer and also gives the user information that the site is about beer brewing and looks inviting to beer drinkers

![Tagline](assets/images/tagline.png)

---

- The footer has social media links so that the user can link to the owner's social media sites where they can find more up to date information from the owner and comment and connect with other beer enthusiasts through social media.  These are visible as you scroll up and down the page so they are easy to find.  I played with favicons for the icons to the social media links but in the end preferred the look of them written out so decided not to use them.

![Footer](assets/images/footer.png)

---

- The recipe page has a hover function so the user can place the curser over the image of the beer and the recipe pops up over the top. This is fun inviting imagery and also makes the recipe for each beer easy to find. Each picture also has the name of the beer underneath it so they are easy to find.

---

- The contact page allows enquires to be sent straight to the site owner. 
- radio buttons on the form allow the user to say yes or no to the newsletter.  I have used radio buttons rather than a tick box so that it is obvious if they do not want the newsletter rather than possibly neglecting to tick the box.  This promotes better UX because it is then clear what he needs of the user are.
- The submit button has a hover function to make it clearer when it is being pressed.

![Contact Form](assets/images/form.png)

- The heading on the contact page makes it clear what the form is for and that you can subscribe to the newsletter.  These extras promote ease of use for the consumer.

![Contact Head](assets/images/contact-head.png)

---

## Features left to implement

- A gallery page of photos.  Once the owner has a sufficient number of photos he likes, a new page can be added and the navigation bar updated.
- a comments section.  The owner would at some point like a comments section where beer enthusiasts and himself could talk with each other straight onto the site.  This could be added to the contact page underneath the form and the navigation bar could be updated as well to show this.

---
# Existing bugs

There is very little space between the bottom of recipe hovers and glass images on the recipes page, on some screen widths, I have played with moving the glass pictures up the page slightly but this then affects the styling at the top of the page.  The footer could do with some padding but I have not added it as this stage because it makes this styling worse.  More work needs to be done to this to make everything fit properly on the page.  You can still see everything that is needed at the moment so I don't consider it to be an urgent fix, but definitely something that I would want to look at if I had more time.

# Fixed bugs

On media query 836px the nav bar doesn't float left in time and goes to the top of the screen for a very short period.  I have not fixed this query yet.  it is only on a very small number of screen sizes.  more work needs to be done to get it to go under the title at the correct screen width.

to fix this I changed the margin top on my .menu in the 836 media query from -2% to 4%

.menu {
        float: left;
        margin-left: 2%;
        margin-top: -2%;

---

I found an error with my recipe cards on small devices. Width of the recipe hover box was not getting smaller as I had indicated.
I inspected the code below and found a typo error gpx instead of px.
~~~
.card-reverse {
        width: 266gpx;
        height: 218.76px;
    }
~~~
---

The footer on the recipe page overlaps with the names of the beers at the bottom.  I have made the footer text smaller.

The hover cards on the recipe page overlap the footer this causes bad UX especially on mobile devices because you can't click the social media links without the hover cards getting in the way.

To fix this bug I needed to look at the code for the cards and hover cards.
~~~
.container {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    height: 80vh;
    width: 100%;
}

.card {
    text-align: center;
    width: 33.3%;
    height: 45%;
    z-index: auto;
}

.card>h2 {
    font-family: "Bebas Neue", Helvetica, serif;

}

.card img {
    height: 80%;
    width: 45%;
    border: 2px white;
    border-radius: 10px;
}

.card-reverse {
    display: flex;
    position: relative;
    text-align: center;
    top: -100%;
    left: 10%;
    width: 422.5px;
    height: 259.76px;
    opacity: 0;
    z-index: 2;
}

.card-reverse>ul {
    z-index: 2;
    font-size: 12px;
    list-style-type: none;
    background-color: #202020;
    border: solid cornsilk;
    border-radius: 10px;
}

.card:hover .card-reverse {
    opacity: 1;
}
~~~
Fist I needed to take of the 80vh on my container.  This distorted the display on my larger screens but interestingly not my smaller screens

I looked at my smaller media queries and noticed that I had added individual vh hights to my .card as shown below. 

~~~
 /*recipe page 400px*/

    .card {
        width: 100%;
        height: 25vh;
    }
~~~

I added individual vh line hights to the .card divs in the larger screen sizes rather than % ones i had before.

~~~
.container {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    width: 100%;
}

.card {
    text-align: center;
    width: 33.3%;
    height: 40vh;
    z-index: auto;
~~~

Once I had completed this I was able to give my footer a z index of 1000 so it sat above everything else on the page.

~~~
footer {
    position: fixed;
    left: 0;
    bottom: 0;
    width: 100%;
    background-color: #202020;
    color: cornsilk;
    z-index: 1000;
}
~~~
---

The hover cards are overlapping the navigation bar at the top of the page on devices between 562px and 400px.

I have updated the .card height from 33vh to 27vh in that media query.

~~~
.card {
        width: 100%;
        height: 33vh;
    }

    .card {
        width: 100%;
        height: 27vh;
    }   
~~~
This ended up causing the recipe cards to overlap slightly at the bottom on small screen sizes so I have reverted the above card height back to 33vh and have adjusted the top  on the .reverse-card to -88% in the 400px media query and -96% in the 562px media query.  This looks ok now.

---

# Testing

I have tested all links to ensure that they take you to the correct place on the site.
I have tested all social media links and they all open to the correct web page in a new web page.

---

## Wave Test

I used [https://wave.webaim.org/] to test the accessibility of my website.  
![Wave Test](assets/images/wave-test-1.jpg)

It showed 2 errors on my recipe page, both of which were empty headings.  After checking my code I had not closed the closing tags.  This was an easy fix

It also showed errors because my headings were not flowing properly.  I had used h1s on my recipes when I should have used h2s.  this again was an easy fix.

![Wave Test](assets/images/wave-test-contact.png)

The wave test on my contact page showed a contrast error with my h2.  This was because the image background colour was #202020.  To correct this error I changed the background colour for the picture to Amber.  I picked Amber because it is beer coloured.

![Wave Test](assets/images/wave-test-home.png)

My home page showed zero errors.

---

## Jigsaw test

Next I tested the site with The W3C CSS jigsaw Validation Service [https://jigsaw.w3.org/css-validator/].

It found the following errors

![Jigsaw test 1](assets/images/w3c-validation.png)

I have been through my code and corrected all of the errors stated.  Only the last error caused me to complete an extra small fix on the size of the recipe hover card to go with it. I now have zero errors as shown below.

![Jigsaw test2](assets/images/correct-w3c.png)

![jigsaw Test3](assets/images/jigsaw-recipes.png)

![jigsaw test 4](assets/images/jigsaw-contact.png)

---

## Lighthouse Tests

Next I tested with [https://web.dev/measure/]

Homepage lighthouse test

![trafficlight Test](assets/images/lighthouse-home.png)

Recipe Page test

![trafficlight Test](assets/images/lighthouse-recipe.png)

This recipe page was quite a bit of work to pass this test.  I had to resize all of my beer glass pictures and swap two that were poor quality for higher resolution pictures.  I also had to ensure my font size did not go below 12px on mobile screen sizes.

Contact Page Test

![lighthouse test](assets/images/lighthouse-contact.png)

---

##  Nu Html Checker

Next I checked with the Nu Html Check [https://validator.w3.org/]

Home Page

![nu test 1](assets/images/nu-html-home.png)

Recipes Page

![nu test 2](assets/images/nu-html-recipe.png)

Contact Page

![nu test 3](assets/images/nu-html-contact.png)

---

# References and Acknowledgments

- I used [w3 schools](https://www.w3schools.com/howto/howto_css_fixed_footer.asp) to help with fixing my footer.
- I used the love running project with the form.
- My friend Simon Duke was the idea behind the website and provided some of the beer recipes.
- Other recipes came from [https://beerandbrewing.com/beer-recipes/] 
- [W3 schools](https://www.w3schools.com/howto/howto_css_product_card.asp ) helped with my cards.
- Me Mentors Daisy Mc Girr and Okwudiri Okoro were generally very very helpful.
- The Tutor support team were also helpful when I got stuck.
- DaveyJH for allowing me to follow his readme and use it as a template.

# Technologies Used

- Balsamiq wireframes were used to create my wireframes
- [Color Hunt] (https://colorhunt.co/) was used to help find my colour scheme
- Chrome Dev Tools was used to modify website once the main structure was in.
- [https://wave.webaim.org/] was used to check the accessibility of my site
- [https://jigsaw.w3.org/css-validator/] was used to check the css on my site.
- [https://web.dev/measure/] was used to check the UX and performance of my site
- [https://validator.w3.org/] was used to check the html on my website.
-https://ecotrust-canada.github.io/markdown-toc/ to make my contents links.

# Deployment

- My website was deployed to GitHub Pages 
- First go to the GitHub repository and select settings
![GitHub Settings](assets/images/github-settings.png).
- Then scroll down to the GitHub pages section and click the link.
![GitHub Pages](assets/images/github-pages.png)
- Then click on the dropdown box below source and pick Branch Main and, indicated in the red circle and click save.
- You will then be deployed, your web address will show in the green banner, in the blue circle.
![GitHub Pages 2](assets/images/github-pages2.png).
- It can take a couple of minutes for your website to deploy.



# Personal Devlopment

- I have learnt so much doing this project.  The first thing I learnt was to calm down and try to work things out before asking for help.  I found a couple of times I sent a request to tutor support only to figure it out myself whilst I was waiting.  Although my problem solving skills are definitely coming along I am working on them all of the time and they are diffinitely an ongoing skill.

- Git commits were another steep learning curve.  The ones at the begining were not explanatory enough and although I tried to get better at them as the project went on I did find it difficult.  

- The hardest bit for me is only doing one thing and a time rather than lots of little fixes all over the site and then having a messy commit message or even forgetting what I have done completely.  This is still a work in progress that I will continue to hone on future projects.  I do understand how bad commit messages make it difficult for other developers looking at your work to understand what you have done, and I am committed to making this skill better. 
- At the very begining of this project I started off with a different look to the website.  I started before my first meeting with my mentor and he advised me to go in a different direction after that first meeting.  I did not include this information in the readme because I felt like it was better to start from scratch again at this point. I have learnt to make sure I have good wireframes that I show to my mentor or workplace moving forward so that I don't waste time giong down a wrong path.
