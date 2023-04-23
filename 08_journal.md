# Learning Journal Week 08

## WordPress Developing Custom Themes

**Weekly Objectives:**

- [x] Create a learning experiment
- [x] Reflect on learning experiment success/failures
- [x] Learn about using underscores starter theme

**Stand-Up Meeting:** <br>
[11/04/2023 - Meeting 03](https://youtu.be/pjwi8bn54BI) <br>
[18/04/2023 - Meeting 04](https://youtu.be/EYKuhkzewbw)

**Team Project:** <br>
[GitHub - Team04](https://github.com/cp3402-students/cp3402-2023-a2-team04)

### Learning Activity

Learning Experiment <br>

Context: <br>
One of the hardest aspects I have faced is learning how to work better in teams. If I reflect on my previous experiences
in group work, I am concerned that I often put myself in an odd position and appear to generally be the person trying to
direct the team back on topic if it has strayed or making decisions when it is time to move forward from an activity.
While this is appropriate for teams where I am delegated team leader; I feel that this approach is less appropriate in
teams without a delegated leader. I really need a way to ensure that the team members are aware of the need to move
forward, so that it is less of a requirement for me to interject at times. Hopefully, in learning to integrate something
into the team work process, it will enable me to work better in teams and develop better relationships with my team
members.

Experiment: <br>
Teamwork has been difficult to coordinate remotely as it is hard to determine if everyone is always present and
attentive during meetings. This has caused meetings to become unnecessarily long (approx. 3 hours) and not an effective
use of our project time. My experiment will be the use of a timer bot in Discord to help manage the meeting time length.
A timer will be set for 1.5 hours for the full meeting duration, another timer for 15 minutes maximum for the stand-up
and 15 minutes for the planning session.
<br>

Metric: <br>
The success of the experiment will be measured by the overall duration of the meeting. If I can get a 50% improvement
(1.5 hours) on our meeting time, then it will be marked a success.
<br>
Estimated Time: 1h 30m

#### Experiment Insights:

The timer was introduced to the team and set during the meeting time. I was less concerned with the stand-up meeting
time, as these had been of an appropriate length. The team acknowledged the use of the timer and this appeared to make
them announce to the rest of the team when the planning timer had ended, which helped make the team time aware and
accountable to the allotted time. The meeting ended up running for approximately 45 minutes. There was some stagnating
at the end of whether it was ready to be concluded.

#### Career/Employability/Learning Insights:

Making the team more time aware appeared to make a difference to the meeting length. It would be beneficial to replicate
this experiment in future team meetings to see if the effects are long-term. Although the meeting length did not reach
the 1.5-hour timer, I speculate that if discussion was fading, when the timer went off it would have been a good signal
that the meeting needed to end. Overall, the experiment was a success in accordance with the metric detailed above.

### Learning Activity

WordPress: Starter Theme Underscores <br>
[WordPress: Building Themes from Scratch Using Underscores](https://www.linkedin.com/learning/wordpress-building-themes-from-scratch-using-underscores-2/welcome?u=2223545) <br>
Estimated Time: 7h 5m

#### Content Insights:

The LinkedIn videos went through the process of creating a custom theme. It made use of gulp, node.js and npm as part of
its initial setup. It also discussed useful plugins such as: developer (with theme check) and show current template.
There were many other steps to set up the gulp, npm and node aspects; these seemed more advanced tools that helped with
mobile first development and compressing Sass. It suggested to design by starting on mobile and adding a media
breakpoint where the design appeared weird. Source maps are used to help find where to put the css code into the sass
folder, this is where gulpfile.js comes in to help. It needs to be toggled on in the browser settings enable CSS source
maps.

Suggested steps to change theme:

1. Change fonts: Google fonts add to enqueue of functions.php, provide backup font families
2. Heading sizes - check for all font responsiveness
3. Set up consistent media queries size constants: 600px, 900px - in variables-site folder _structure.scss
4. Check order of styles.scss for loading order and re-order if required
5. Go to content site/site.scss and insert new import statement for a new file global layout, create new _global sass
   file in the layout folder
6. In global scss add in layout css with media queries for responsiveness
7. Start from top to bottom with each module

#### Career/Employability/Learning Insights

It was a little concerning when I saw the set-up using gulp, node and npm as these were not elements that our group had
intended to use. We chose underscores because it did not have all these other dependencies, there were other starter
themes that did have these that we looked at. It made it important that I watched more of these videos to understand
what is the reason these were used.

There is so much to learn about building custom themes; therefore, it will be important to prioritise the key elements
to learn first and worry about more advanced features after becoming more familiar. A select number of items to modify
for the group project custom theme should be implemented to start. These features should easily accommodate the client's
provided content and needs. There are certainly aspects that need to be discussed with the group as to the approach
taken to creating our custom theme.

### Learning Activity

WordPress: Starter Theme WP Rig <br>
[WordPress: Building Progressive Themes with WP Rig](https://www.linkedin.com/learning/wordpress-building-progressive-themes-with-wp-rig-2/buidling-progressive-wordpress-themes?u=2223545) <br>
Estimated Time: 30min

#### Content Insights:

WP-Rig is a good starter theme to use if you are concerned about optimising performance. It has a wiki with
suggested plugins and other aspects to use during development.

#### Career/Employability/Learning Insights:

I had already done research into starter themes before watching this video. This video helped to confirm that I was
happy with the decision that our group made as it required further dependencies than our current setup. However, it
would be interesting to try a different starter theme in more depth in a new future project when I was feeling more
confident to continue experimenting with more complex workflows and setups.

### Learning Activity

DRY Development <br>
[WordPress Developer Tips: DRY Development](https://www.linkedin.com/learning/wordpress-developer-tips-dry-development/welcome?u=2223545) <br>
Estimated Time: 35m

#### Content Insights:

Package up commonly used functions into their own files. Modularise code wherever possible to improve code maintenance.
Header, Footer, Sidebar are all handled with a call to a function that gets the header etc. Use a loop to go through all
posts to display. These are all template parts used in the index.php file to reduce the amount of code. Conditional tags
test for true or false; all available conditional tags are listed on WordPress's website.

#### Career/Employability/Learning Insights:

It was great to smooth over the sort of patchy understanding I had on how themes and templates come together. I think
that this knowledge would have been beneficial much earlier in my learning process when trying to change an existing
WordPress theme for the first assignment. There was a big learning curve that would have been clarified quickly by this
video. 