# Kate's website 

I have build a single web page, using HTML and CSS.  Below are the steps and things I have learned while working on this project:

## Initial set up 

I had an initial meeting with _The client_ where we got to know each other a bit better. During the same session we layed out the plan and set up following objectives as:

* get to know each other 
* reasearch layout design 
* create survey with layout options and color pallets
* create survey to gather more content info
* create wireframe
* present and check wireframe with _The client_
* exchange info and photos needed for the page
* schedule regular meeting for pair programming 

While doing the reasearch we had regular meetings to discuss around what we are doing, our progress and next steps. 

## Info gathering

I used [this survey](https://docs.google.com/forms/d/e/1FAIpQLSc07OIUW2kmO5TVBpccaRN8i7zCpBwx8GgLBAIkaXsaB--37Q/viewform?usp=sf_link) for Kate to pick her favourite layout and collor pallete. I used [W3School](https://www.w3schools.com/colors/colors_palettes.asp) for the color pallete options. 

I used [this survey](https://docs.google.com/forms/d/e/1FAIpQLSfSIawvVidNMcOGtmCbKLgnioHM78wjvPK80QjR1m_gmoDd0g/viewform?usp=sf_link) to collect content information from _The client_.

I designed a **wireframe** to help me visualise where everything will go before starting coding.  Had another meeting with Kate to confirm the arrangment and start on the code. 

For inspiration around the layout and writing content I took a look at these [personal websites](https://www.themuse.com/advice/the-35-best-personal-websites-weve-ever-seen). 



## What I learned

### Fixed navbar and HTML structure

Most of my inspiration came from the material available on the **repos** offered and from **extensive googling**. 

I was not sure how to set the nav bar to stay fixed at the top while scrolling to the page. This is where I have learned the importance of the **HTML structure**.  Set a `div` for the `header` and another `div` for my `main`. This allowed me to set the position fixed for the `navbar` and do my separate setting for the `main` using **CSS**.  I used [this]()https://www.w3schools.com/howto/howto_css_fixed_menu.asp) and [this](https://www.w3schools.com/howto/howto_js_topnav.asp) for guidance. 

```CSS
.navbar {
  overflow: hidden;
  background-color: #96ceb4;
  position: fixed;
  top: 0;
  width: 100%;
}
.main{
  padding: 16px;
  margin-top: 30px;
}
```
The `position: fixed` is what keeps the `navbar` in place and by using `width:100%` ( **max width**) I made it be the size of the page. 

 When I was trying to link the buttons on my `navbar` with different sections of my page I have added a `section id=` to that part of the page. The `id` connects `navbar`. 
 
 After takling with Kate I found out I can add both `class` and `id` to my `div` , which makes it easier.  The I still think having the `section id=` helps with the structure of the HTML code, so I have used both. 

 ### Hero Image

 I wanted to have a smooth transition between the `header` and the `main`. I thought and image would be a good idea but I also wanted to add some writing on top of it. I chose *the sea* becasue Kate loves it and also the colors match the color scheme of the page. 

Old friend google helped me again and used [this](https://www.w3schools.com/cssref/tryit.asp?filename=trycss3_background_hero) as guidance for my `hero text` and `hero image`. 

### CSS float and clearfix hack

I used the CSS *float* to move the *my story* text around the image.  The `float right/left` property is what moved the text around the image. The `clearfix` hack is really good as it allows the text to wrap around the picture. 

I have also used `float` and `claerfix` to diplay images side by side. 

### Flexbox and Grid

This was really good to learn. I think its a briiant techniques that allows you arrange text and also images with flexible height. I think this will be a really usefull tool to use in the future. 

### Hoover and Inline block

Used the `hoover` for both my navbar and the `list elemnts` to outline them. 

Used:

```CSS
    .skill-set li{
        display:inline-block;
	    list-style:none;
    }
 ``` 
 to style my `list items` inside my `flex-container`. Gave a more artistic layout that the regular bullet points. 

 ### Responsive Galerry

 I chose this as a very creative and interactive solutiion to diplay images with added description. I particularly liked that you can open 

 ### Media Query

 I added this to my CSS code `flex-container` and also for my `responsive gallery`. This cool feature makes my website look good on on different sizes screens. Allows the columns and images to stack up when you resize the screen. 

 ## Issues and what can be improved

 ### CSS units

 I have created 3 `div class=block` where my <h4> text is kept along the page. I did this to give my page a bit more structure and for the layout. At the moment I have a different `div` for each block because the `margin` set-up is different. I have the margins set as the background goes over the next bit when I change it. 
  I think I need to reasearch on **CSS units**. 

# Website Challenge

## Overview

For your first project on the bootcamp, we want you to make a website all about your pair partner using HTML and CSS.

The person you are making your website for is your partner, aka The Client. It is your job as a programmer to understand what the client wants from a profile site, assess what information is available and useful, design what serves the audience of users (aka the other bootcampers) best from the experience, and then create something which best solves those needs. You won't be given any guidance of what to build - you'll need to empathise with your users to see what they would find useful (or even survey and talk to them), and plan your site accordingly.

## Outcome

- a single web page created with HTML and CSS
- a profile describing your client
- a short 1-page README.md file alongside it which describes how you went about the project (your thoughts, research, plans, and justification for decisions)

## Extra

This is not only a chance for you to practice the core skills of HTML and CSS, but also a chance to invest time in thinking about how to build a website for a client, and have a user-centric approach - a key learning objective of the course. You will need to actively communicate with the client to find out everything you need in order to design and build a website which represents them to the rest of the cohort.

Although you will each have an individual repository in which to make the website, there is nothing stopping you pair programming with your partner on the project. Organise your time so that you can spend an equal amount of time on each project. For example, if you spend three hours coding together on Sunday, you would spend 1.5 hours pair programming on one site, before moving over to the other site.

This project will span the first two weeks of the bootcamp, and you will be given time in live evening sessions to work on it as well.


























