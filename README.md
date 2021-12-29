

# DUKEY'S BREWS

![Meda Screens](assets/images/meda-screens.png)


[Dukeys Brews Live Site](https://0osaraho0.github.io/Dukeys/)

# About

This website is aimed at home brewing enthusiasts.  The owner of the website wishes to share his home brew recepies and home brewing ideas and have a space for other home brewing enthusiasts to be able to make contact and subscribe to his news letter.


# User Experience (UX)

before starting the website I sat down with the owner and discussed what he wanted to see from his website.

Site owners goals
- It needed to be easy to navigate
- It needed a contact or chatroom style section so that he could meet other beer enthusiasts.
- He wanted a section to show some of his recepies.
- He would like a blogging section so that in the future he could add to it when he next brews.

we rated these goals on a scale of 1 to 5 in importance and feesability

| Goal | Importance | Feesability |
|---| ---|----|
|Easy to navigate|5|5|
|Chatroom|2|2|
|Contact page|5|5|
|Recepies|5|5|
|Blogging|3|1|
|Gallery|1|5|

After looking at the feesability of the goals we decided to go ahead with making the website but to leave out the blogging page and the chat room section of the contact page for the initial update.  My skills as a developer are not quite at that stage yet and the owner does need to do that right away anyway.  The owner also does not have many pictures at this time so decided to leave the gallery for a later update as well.

With this in mind we decided to go for a front page with a link to his recepies and a contact page.

# Wireframes

Please see the initial wire frames for this site.

![Wireframe Front Page](assets/images/wireframe-home-page.png)
![Wireframe Recipe Image Page](assets/images/wireframe-recipe-front.png)
![Wireframe Recipe Image Hover](assets/images/wireframe-recipe-back.png)
![Wireframe PContact age](assets/images/wireframe-contact.png)


After going over the wireframes with the website owner we decided to go with beer glasses rather than bottles and a dark background with light writing.

### Colour Scheme

The owner wanted a masculine feel to the page, and I felt the site needed a clean look to it. I have decided to go for a simple colour scheme of  #202020 and #fff8dc to facilitate this.  
![#202020](assets/images/202020.png)
![#fff8dc](assets/images/fff8dc.png)

I also went for Amber as the image background colour in case the image doesnt load.  This is to create contrast with the h2 on the contact page and because it is beer coloured.
![Amber Background](assets/images/contact-amber-background.png)

### Typography

I have used the fonts bebas Neue for my h1 and h2s on my recipe cards as it is bold, eye catching and clean looking.
I have used Georama for the rest of the font because it also has a clean look and is easy to read.
I used Helvetica and Georgia for my back up fonts because they look similar.

### Imagery

The images used on the home and contact pages are inviting for thirsty beer enthusiasts that get excited over a refreshing pint of beer.  I used beer glasses on the recipe page rather than the bottles in the wireframes because they look more homely and inviting than the bottles.

The recipes have a white boarder arround them to give them a nice finish that matches the edge of the pictures. both picutes and recepies have a 10px radius to give nice rounded corners.

# Features

## Existing Features

- The header is visible on every page and has a consistant design throughout.
- The menu bar is is available at the top of every page, this gives the user ease of navigation when moving to different pages on the site.
- The tagline "Lets Brew.. Some Beer" informs the user the site is about brewing beer and takes you straight to the recipe page when clicked.  This promotes ease of use for site navigation.
- The hero image is of a pint of beer also gives the user information that the site is about beer brewing and looks inviting to beer drinkers
- The footer has social media links so that the user can link to the owners social media sites where then can find more up to date information from the owner and comment and connect with other beer enthusiasts through social media.  These are visible as you scroll up and down the page so they are easy to find.
- The recipe page has a hover function so the user can place the curser over the image of the beer and the recipe pops up over the top. This is fun inviting imagry and also makes the recipe for each beer easy to find. Each picture also has the name of the beer underneeth is so they are easy to find.
- The contact page allows enquires to be sent straight to the site owner. 
- radio buttons on the form allow the user to say yes or no to the newsletter.  I have used radio buttons rather than a tick box so that it is obvious they do not want the newsletter rather than possibly neglecting to tick the box.  This promotes better UX because it is then clear what he needs of the user are.

### Features left to impliment

- A gallery page of photos.  Once the owner has a sufficent number of photos he likes a new page can be added and the navigation bar updated.
- a comments section.  The owner would at some point like a comments section where beer enthusiasts and himself could talk with each other straight onto the site.  This coud be added to the contact page underneath the form and the navigation bar could be updated as well to show this.

# references

I used w3 schools to help with fixing my footer. https://www.w3schools.com/howto/howto_css_fixed_footer.asp



# Existing Bugs

on media query 836px the nav bar doesn't float left in time and goes to the top of the screen for a very short period.  I have not fixed this query yet.  it is only on a very small number of screen sizes.  more work needs to be done to get it to go under the title at the correct screen width.


# Fixed bug.  

I found an error with my recipe cards on small divices. Width of the recipe hover box was not getting smaller as I had indicated.
I inspected the code below and found a typo error gpx instead of px.
~~~
.card-reverse {
        width: 266gpx;
        height: 218.76px;
    }
~~~

The footer on the recipe page overlaps with the names of the beers at the bottom.  I have made a small fix just by making the footer text smaller.

The hover cards on the recipe page overlap the footer this causes bad UX expecially on mobile devices because you can't click the social media links without the hover cards getting in the way.

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
Fist I needed to take of the 80vh on my container.  This distorted the display on my larger screens but interestinly not my smaller screens

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

# Testing

I have tested all links to ensure that they take you to the correct place on the site.
I have tested all social media links and they all open to the correct web page in a new web page.

I used https://wave.webaim.org/ to test the accessibility of my website.  
![Wave Test](assets/images/wave-test-1.jpg)

It showed 2 errors on my recipe page, both of which were empty headings.  After checking my code I had not closed the closing tags.  This was an easy fix

It also showed errors because my headings were not flowing properly.  I had used h1s on my recepies when i should have used h2s.  this again was an easy fix

![Wave Test](assets/images/wave-test-contact.png)

The wave test on my contact page showed a contrast error with my h2.  This was because the image background color was #202020.  To correct this error I changed the background colour for the picture to Amber.  I picked Amber because it is beer coloured.

![Wave Test](assets/images/wave-test-home.png)

My home page showed zero errors.

Next I tested the site with The W3C CSS Validation Service.

It found the following errors

![w3c Test](assets/images/w3c-validation.png)

I have been through my code and corrected all of the errors stated.  Only the last error caused me to complete an extr small fix on the size of the recipe hover card to go with it. I now have zero errors as shown below.

![w3c Test](assets/images/correct-w3c.png)

### Lighthouse Tests

Homepage lighthouse test

![trafficlight Test](assets/images/lighthouse-home.png)

Recipe Page test

![trafficlight Test](assets/images/lighthouse-recipe.png)

This recipe page was quite a bit of work to pass this test.  I had to resize all of my beer glass pictures and swap two that were poor quality for higher resolution pictures.


Contact Page Test

![lighthouse test](assets/images/lighthouse-contact.png)


