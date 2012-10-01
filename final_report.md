# Final Proposal

Our plan is to create a continuous integration server.

A variety of continuous integration server options already exist, such as Jenkins, CruiseControl, and Buildbot. These options, and many others, satisfy a variety of different user requirements; however, they all also suffer from problems. The largest problem is that most are massively complicated, built for the intricate needs of big, diverse teams that need an extremely customized set of needs. This means that they are massively configurable, but also means that it takes a serious chunk of time to set up any project. For small teams, testing is already a major hurdle, and setting up a continuous integration server takes so much time and expertise that it is difficult to justify.

We intend to build Rosie as a better option for small teams. Continuous integration is one of the best forms of testing feedback out there, and it should be easier to start using for any project. We are looking to shed much of the weight in current continuous integration options by abstracting out common pieces and leaving extraneous features and configurations behind. Rosie is the CI server of the future, built so that small teams can be up and running their own server in minutes with no expertise necessary.

Continuous integration servers are not a cutting edge technology: they've been built hundreds of times before. Therefore, we think this project is entirely feasible because we are simply trying to improve on an already existing service.

After talking with a few potential users, there were several things which immediately became clear. Most importantly, there is no way for us to build a CI server to satisfy every user. This has been the approach of previous projects and the result would be another intimidating, difficult behemoth for teams to grapple with. 

Feedback from one user who had spent time on small teams reinforced the need for something simple that could instantly get smaller teams up and running with this tool previously reserved for giant teams that had the man hours and expertise to spare. Therefore, we plan to target these small teams by focusing on ease of set up. We want our server to be useable by a project as soon as possible. If CI is easy to begin using, then we will hopefully see it being used on more and smaller projects.

We also discussed tools we could lean on in order to fit into common workflows and prevent ourselves from redoing the work that has already been done. Our users' experience with Github, along with tools like Gitbuilder and Heroku, helped us find acceptable dependencies for our project, and as a result we plan to integrate out-of-box with them.

Drawing from our requirement analysis, we've outlined some key requirements and features that the product must satisfy:
* ability to automatically run tests after every commit pushed to a central git repository
* single line creation of a CI server for any given product
* pre and post build custom bash scripting
* intuitive web UI for configuration
* easy deployment of CI to Heroku after configuration
* blame notification and information for build failures down to source code line where failure originated
* ability to create a new issue on Github for any build failure
* ability to automatically build any new pull request opened on Github and comment the result in the pull request thread

Ultimately, the complaints we heard from our users about their current CI tools were reassuring that this is a problem for a ton of teams and has plenty of room for better tools despite the heavyweight incumbents.

Right now, the solutions that do exist are bloated, hard to configure, and unnecessarily complicated; that being said, these solutions do provide a strong base for us to build on top of. We can see which features work well and which features don't; which customizations improve the experience and which detract from it; we will be learning from the mistakes and successes of the hundreds of developers before us.

Between the three of us, we have extensive experience building large scale web applications, and while none of us have ever built a CI server before, many of the lessons we have learned from other projects will apply to this one. Together, we are confident that we have the technological capability to complete this task.
