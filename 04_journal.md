# Learning Journal Week 04

## Development and deployment workflows

**Weekly Objectives:**

- [x] Set up Microsoft Azure web hosting
- [x] Set up Joomla in live environment using Azure web hosting
- [x] Set up WordPress in live environment using Azure web hosting
- [ ] Set up Vagrant or Docker for development _(Achieved Local Only)_
- [x] Join a Team

### Learning Activity

Web Design Process <br>
[Mapping the Modern Web Design Process](https://www.linkedin.com/learning/mapping-the-modern-web-design-process/create-great-informational-user-experiences?autoplay=true&u=2223545) <br>
Estimated Time: 2h 15m

#### Content Insights:

The LinkedIn course on the modern web design process highlighted topics such as: roles/responsibilities, creating
guides, and the web design process overall. It was important to note the separation of roles where it recommends that UX
design, System Architect, Quality Assurance and Beta Testing roles are separated at minimum from the person involved in
the other roles e.g. Front-End, Back-End Developers. It was also interesting to hear about the guides: style, content,
code and process. These aspects will help with understanding future team dynamics in web design and basic methods to
improve collaboration. The aspects on the web design process were interesting where it was described as a
'dynamic process', which means the foundations of the process will stay the same, but adaptability is key.

#### Career/Employability/Learning Insights:

This course expanded my mind to the more in-depth realm of web design and how building sites can become more complex. At
this point my view was rather narrow, that websites only really need a single person or a small team. It has made web
design more daunting as a career option, particularly due to how much I have struggled with developing live web
environments. The process is very theoretical still, which is good as a foundation, but I will not be able to cement my
understanding until I have successfully followed the process myself.

### Learning Activity

Version Control <br>
[Versional Control for Everyone](https://www.linkedin.com/learning/version-control-for-everyone-2/version-control-it-s-not-just-for-programmers?autoplay=true&u=2223545) <br>
Estimated Time: 1h 43m

#### Content Insights:

The LinkedIn course gave an overview of version control and how to use it for different applications. The most
significant part was Section 5 on sharing a project, which may be required for future reference when looking at
assignment 2. Basic process is as follows:
Fork > Branch > Commit Changes > Push > Pull Request > Merge Pull Request > Fetch > Pull

#### Career/Employability/Learning Insights:

This course really only felt a little valuable towards the end, but it did suggest there was a course called GitHub for
Web Designers for further (hopefully more context specific) learning.

### Learning Activity

Moving WordPress from Local Environment to Live Environment using Migrate DB Plugin <br>
[Migrating WordPress with Migrating DB and DB Pro](https://www.linkedin.com/learning/migrating-wordpress-with-wp-migrate-db-and-db-pro/who-this-course-is-for-and-how-it-works?autoSkip=true&autoplay=true&resume=false&u=2223545) <br>
[WordPress Migration 2020](https://www.linkedin.com/learning/wordpress-migration/preparing-for-migration?autoSkip=true&autoplay=true&resume=false&u=2223545) <br>
Estimated Time: 2h 7m

#### Content Insights:

The migration courses from LinkedIn talked about using WP Migrate DB in order to create the .sql.gz file that would then
be imported into the live site database using PhpMyAdmin. It then used FTP to transfer across the files from the
wp-content folder for the plugins and themes. In order to follow this process the live site needed to have the database
setup with a fresh installation of WordPress to use the plugin.

#### Career/Employability/Learning Insights:

These videos felt like the step after the one I was up to in terms of setting up a live site as I hadn't gotten the
database set up correctly yet. It was good to watch as it gave me some new insight into perhaps some of the things I was
doing wrong and why I was struggling with the database at this point. It gave me a new direction of things to try.

### Learning Activity

Databases and Linking to Live Site <br>
[Azure Data Studio Essential Training](https://www.linkedin.com/learning/azure-data-studio-essential-training-15050110/what-is-azure-data-studio?autoSkip=true&autoplay=true&resume=false&u=2223545) <br>
[Azure Essential Training for Developers](https://www.linkedin.com/learning/azure-essential-training-for-developers/azure-for-developers?autoplay=true&u=2223545) <br>

Estimated Time: 2h 54m, Actual Time: 30m

#### Content Insights:

I looked at Azure training videos on LinkedIn in hopes that it might help me figure out how to make my Azure SQL
database usable for my website. All the current information I kept finding online for how to implement a website
involved an Azure SQL database, but the instructions were out-dated and the buttons they used to perform the setups were
no longer available. Unfortunately this content only provided overview information, not the specific detail that I was
looking for.

#### Career/Employability/Learning Insights:

There were so many out-dated learning materials for Microsoft Azure that it made me contemplate changing web hosts.
I generally am a click-around-and-figure-it-out kind of person, but it has not been clear where to do anything.
If I am unable to use Docker containers to set up my site on Microsoft Azure, I might be forced to change as I cannot
find relevant material to understand how to deploy my sites.

### Learning Activity

WordPress on Azure - Quick Start <br>
[Create a WordPress site - As App Service](https://learn.microsoft.com/en-us/azure/app-service/quickstart-wordpress#create-wordpress-site-using-azure-portal) <br>
[How to create WordPress on Azure App Service](https://www.youtube.com/watch?v=JQMKtcWg83I) <br>
[Six different ways deploying WordPress onto Azure](https://www.youtube.com/watch?v=trYCwcEYwDc) <br>
[Use MySQL Database on Azure to deploy Joomla! apps](https://docs.azure.cn/en-us/mysql-database-on-azure/mysql-database-joomla-setup) <br>
Estimated Time: 1h

#### Content Insights:

I investigated simpler means of deploying a WordPress site on Azure. There were two types of methods that I found, Azure
with WordPress as an app service or virtual machine. Azure offered the app service with a pre-built in database. As the
virtual machines often were associated with costs, I opt-ed to explore the app service further and concluded it was also
the simplest to set up.

#### Career/Employability/Learning Insights:

The first assignment did not require the full development workflow set up; therefore, I looked for a simpler means to
create a WordPress site on Azure. I decided that it was good to have an alternative approach to meet the deadline, as I
did not think I would be able to work out the development environments with containers in time. This also helped relieve
the pressure of not having anything that worked yet.

### Learning Activity

Joomla on Azure - Quick Start <br>
[How to Set up/Install Joomla Server on Ubuntu in Azure](https://www.youtube.com/watch?v=0CYZ-LL3gTM&t=237s) <br>
[Joomla Bitnami Documentation](https://docs.bitnami.com/virtual-machine/apps/joomla/get-started/access-application/) <br>
Estimated Time: 30m

#### Content Insights:

As I did with WordPress, I wanted a quick start solution to start working in Joomla. I looked at the Joomla by Bitnami
virtual machine and the documentation required to finalise the set-up.

#### Career/Employability/Learning Insights:

It seemed despite this being a 'one-click' solution, it involved a lot of knowledge about SSH, and virtual machines. It
took me a while to get my head around how to get my credentials and connect through ssh. My mind is absolutely swelling
with new information, and it has become overwhelming. Every single action requires a mountain of knowledge to implement
the simplest thing. I planned on taking a scripting subject next semester, though I was not convinced until now that it
is necessary.

### Learning Activity

Docker, Docker Desktop and Docker-Compose <br>
[Docker Compose](https://docs.docker.com/compose/gettingstarted/) <br>
[Docker](https://docs.docker.com/get-started/) <br>
[How to deploy Joomla with Docker](https://www.techrepublic.com/article/how-to-deploy-joomla-docker/) <br>
[Docker and ACI](https://docs.docker.com/cloud/aci-integration/) <br>
[Set Up WordPress and Docker](https://www.youtube.com/watch?v=pYhLEV-sRpY) <br>
[Docker on Azure](https://www.linkedin.com/learning/docker-on-azure/use-acr-locally?autoSkip=true&autoplay=true&resume=false&u=2223545) <br>
Estimated Time: 5h

#### Content Insights:

The first part of the learning journey was to understand Docker containers and Docker images. The second part of the
journey was creating them, running them and connecting them to a network. The third part was looking writing a docker
compose file. The last part was learning how to use this on Microsoft Azure, though this proved more difficult.

#### Career/Employability/Learning Insights:

It was clear that creating a Docker setup was not easy. It required a lengthy journey to understand each of the
components of containers, images, volumes, networks, and docker compose. This journey resulted in the creation of a
docker compose file and using Docker Desktop. This enabled the Joomla/WordPress, MySQL and phpMyAdmin containers to run
locally, but more information was required to deploy on Azure; therefore, I started a new more in depth learning
activity here.

### Learning Activity

Docker Local Environment, Staging Environment, Production Environment <br>
[Using Docker Containers with WordPress](https://wpengine.com.au/resources/containers-clusters-wordpress/) <br>
[Volumes](https://docs.docker.com/storage/volumes/) <br>
[Compose file specification](https://docs.docker.com/compose/compose-file/#volumes) <br>
[Docker compose down](https://docs.docker.com/engine/reference/commandline/compose_down/) <br>
[Learn How to stop, kill and clean up docker containers](https://blog.eduonix.com/software-development/learn-stop-kill-clean-docker-containers/) <br>
[How to use your own registry](https://www.docker.com/blog/how-to-use-your-own-registry/) <br>
[Docker Registry](https://docs.docker.com/registry/) <br>
[How to Get Started with Docker](https://www.youtube.com/watch?v=iqqDU2crIEQ&t=1002s) <br>
[Docker for Beginners: From Docker Desktop to Deployment](https://www.youtube.com/watch?v=i7ABlHngi1Q&list=TLPQMTgwMzIwMjP56ISB4sjQpw&index=2) <br>
[Deploying a container image to Azure App Service from Docker Hub](https://www.youtube.com/watch?v=_LNOg8kU4CE) <br>
Estimated Time: 5h

#### Content Insights:

I went through a lot of information on workflow, deployment and environments with relation to using Docker. I was unable
to find something that really detailed what I was trying to do, so I attempted to piece together the process. Once
images are pushed to Docker Hub or Azure Container Registry they can be used to create a web app service. However,; it is
unclear from this information how to use this to create a staging versus production environment. It is also unclear how
to turn this process into a 'continuous development' workflow.

#### Career/Employability/Learning Insights:

Between my failures to get Docker to work and Vagrant, I have become very disheartened by the process. I have yet to
give up, but simply looking at alternatives or new sources for information is not working. I think I require support
from my teammates to help figure out the missing pieces, as I am struggling to learn this independently.

### Learning Activity

Branch Protection <br>
[Protecting GitHub Branches](https://www.youtube.com/watch?v=hS7uybMi0z4) <br>
[GitHub Branch Rules](https://www.youtube.com/watch?v=CNCE1gts2Yw) <br>
Estimated Time: 20m

#### Content Insights:

The video highlighted creating separate branches and then adding protection rules in order to preserve the integrity of
the code. I watched a few videos on how to set up the team repository to use staging, development, main and experiment
branches. It suggested to use: require a pull request before merging with 1 person to review (more would make small
changes annoying), dismiss state pull request approvals when commits are pushed (otherwise new pushes to the same branch
may not be reviewed), require status checks to pass before merging (why add broken code?), require branches to be
up-to-date before merging, and include administrators (should be included in these rules).

#### Career/Employability/Learning Insights:

It was interesting to consider how I might manage a repository for a GitHub project in relation to web development with
other collaborators. The information I recorded above is relevant to this project, but the videos do provide further
detail for future references for managing rules with other GitHub projects. When setting up the repository, I also found
that some suggested options were not available without further learning (status checks).

### Learning Activity

Workflow: Local/Live; Development, Staging and Production <br>
[Managing releases in a repository](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository) <br>
[GitHub Actions: Approvals, Environments and Visualisation DEEP DIVE](https://www.youtube.com/watch?v=w_37LDOy4sI) <br>
Estimated Time: 20m

#### Content Insights:

After looking at protected branches, I noticed that the image and articles talk about releases; therefore, I looked at
an explanation to see how that might work with GitHub. It appeared easy to implement from the main branch, on the
right-side panel there is an option for releases. In this process I accidentally came across environments, which seems
to be a relatively newer feature of GitHub. It mentioned staging/development/production which made me look into how this
might help the team's workflow by creating automated steps. It was just an overview at this stage of learning.

#### Career/Employability/Learning Insights:

As workflow is unique to each team, it was important that I presented these findings to teammates to see how they felt
about adopting any of these approaches. The conclusion was that we all needed to learn more to gauge its
usefulness.

### Learning Activity

Vagrant and Vagrant Boxes <br>
[Getting Started](https://developer.hashicorp.com/vagrant/tutorials/getting-started) <br>
[Varying Vagrant Vagrants](https://varyingvagrantvagrants.org/docs/en-US/installation/) <br>
[Getting started with Vagrant & VVV for local development](https://webdevstudios.com/2015/01/14/getting-started-vagrant-vvv-local-development/) <br>

Estimated Time: 30m

#### Content Insights:

Vagrant is another alternative to using Docker. When I struggled to use Docker, I decided to change direction and look
at Vagrant. I looked at understanding what vagrant was and then different methods for creating a local environment. VVV
sounded like a good option as it created the staging/development/production environments - though noted it was '
overkill' for the purposes of this subject.

#### Career/Employability/Learning Insights:

I was able to install Vagrant and get it to vagrant up with vagrant box. I then attempted to install the VVV using the
installation instructions, but was only met with error messages half-way through the installation. Unsure how to proceed I decided to return back to using
Docker. 