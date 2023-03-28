# Learning Journal Week 05

## WordPress: Developing Child Themes

**Weekly Objectives:**

- [x] WordPress site for Assignment 1
- [x] Joomla site for Assignment 1
- [x] Continue Development/Staging/Live learning journey

### Learning Activity

WordPress Child Themes <br>
[WordPress: Building Child Themes](https://www.linkedin.com/learning/wordpress-building-child-themes-3/level-up-to-wordpress-developer?autoplay=true&u=2223545) <br>
Estimated Time: 2h 4m

#### Content Insights:

The LinkedIn video discussed child themes. It highlighted that choosing a parent theme was important as it could save a
lot of time down the track. Look for layout, style, fonts, colours and animations when choosing a parent theme. When
creating a new child theme: create a new folder in themes (inside wp-content), then inside the folder create a style.css
file and update the metadata for the theme. Add a file called functions.php with the code from the child theme
documentation functions from wordpress.org.

It made suggestions at each step to test by using something small and obvious. Use the laziness principle to build upon
what code already exists that uses best practice and design in the browser (inspect). Add functions with help from
developer.wordpress.org and modify pluggable functions by searching for them in the parent theme folder, copying and
pasting into the child theme functions.php. Filter function allows one to change a section of content e.g. adding
Recipe: to the front of a title. Remove/add function change entire sections on a theme e.g. removing a widget section.

Show Current template plugin helps to show what template is being used on the site. Modify themes and php functions
first, if required then look at modifying templates. In order to add new fonts (like from Google fonts) it needs to be
added into the functions.php. Add a Screenshot for the child theme by naming it screenshot.png and add into child theme
folder. Upload theme using FTP program or zip and upload through WordPress admin by going to themes add new and upload.
If content changes have been made go to appearance and live preview, make changes then activate and publish. If changes
need to happen all at the same time export content, then import onto the live site. Plugins are also available for more
seamless workflow.

#### Career/Employability/Learning Insights:

There is a lot to learn when it comes to WordPress and dealing with WordPress themes. As a potential area of speciality
for a career path, it shows how much WordPress has dominated the CMS market. One aspect that was highlighted a lot in
the videos was that each small change can be very time-consuming and this should be considered when doing our own
projects. I wrote more detailed notes about the video above to hopefully reduce the number of times required to return
to these videos for reference.

### Learning Activity

Responsive Web Design <br>
[Learning Responsive Web Design in the Browser](https://www.linkedin.com/learning/learning-responsive-web-design-in-the-browser/welcome?autoplay=true&resume=false&u=2223545) <br>
Estimated Time: 1h 51m

#### Content Insights:

Create a design language by using style tiles that help to develop a style guide. Draft layouts using pen and paper as
it helps with quick experimentation. Draw out which containers are required from your layout drawings. Identify modules
within the design, this helps to identify repeated parts.

Design in the browser by using a browser and inspect, then make changes by changing the code css (style.css). Start
mobile first design and add media break points as you scale up focusing on individual modules. In order to easily
make responsive typography, set a font pixel size, then use media queries when reaching min-width to resize the
font-size to a new em value. Flexbox is a good technique for achieving multi-column layouts using CSS. Use the colour
picker within the browser to experiment, a dropper can be used to pick out colours from your images.

#### Career/Employability/Learning Insights:

From a learning perspective, I have found HTML and CSS with changing the code the easiest to understand. What I am
finding complicated is the different methods depending on whether a CMS is involved in the process. Everything in this
video showed a format I am more familiar with, but I need to broaden my familiarity to just the last part of working in
WordPress.

### Learning Activity

WordPress Building a Website <br>
[8 hours compelte course WordPress Tutorial (2023)](https://www.youtube.com/watch?v=09gj5gM4V98) <br>
Estimated Time: 4h

#### Content Insights:

The WordPress video on YouTube was a comprehensive breakdown of using WordPress without using a plugin page builder like
Elementor. This was an important video to find as every single tutorial used these plugins and not the core
functionality of WordPress like we were required to use for the assignment. The video went into detail on the entire
dashboard and then went through how to actually make a site. It provided valuable insights into how WordPress can be
used more effectively and the capabilities of some features I hadn't realised yet.

#### Career/Employability/Learning Insights:

In completing this course, I did not want to dedicate the full 8-hours. I watched it on double speed in order to half
the amount of time taken and skipped elements I was familiar with to reduce the time on any repeated content. The
objective in watching this video was just to see how someone else really used WordPress to create a website and pick up
on all the extra features that I could not figure out what they did yet in my own muck around sessions in WordPress.

### Learning Activity

Docker Compose and Azure <br>
[Tutorial: Deploy a multi-container group using Docker Compose](https://learn.microsoft.com/en-us/azure/container-instances/tutorial-docker-compose) <br>
Estimated Time: 10m

#### Content Insights:

This website documents how to use a docker compose file and tweak it to work with Azure's container registry.

#### Career/Employability/Learning Insights:

I was skeptical about using Microsoft's own documentation at this point. Half of the information I found was outdated on
Azure's documentation. I retained this website to use a reference as I attempt to use this information to create the
staging and production side using Docker and Azure. If unsuccessful, I will discontinue using Microsoft as a point of
reference and stick to third-party information that is more up-to-date.