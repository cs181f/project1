Competitive Research
====================

Given the scope of the problem, it is unsurprising that the Continuous Integration (CI) server space is overcrowded. These are some of the current solutions with their strengths and weaknesses.


# Hudson

Hudson is one of the oldest CI solutions around. It is built on Java, supported by the Eclipse Foundation and has been a production solution for large companies for a long time.

Strengths:

* extremely comprehensive and extendable

Hudson has hundreds, if not thousands of plugins, that allow you to add practically any feature to your CI setup

* integrates with git and GitHub well
* easy to use custom build script to build any type of code
* battle tested over a long time
* Free (released under MIT license, open source)
* well documented
* web UI
* can manage multiple builds and multiple build machines

Weaknesses:

* hard set up and configuration
* web UI is very convoluted

Being so old, and so customizable, it is very easy for a beginner to get lost when trying to install and set up and Hudson server.

* split between Hudson and Jenkins

A major group of Hudson contributors left the team to branch Hudson into a "more" open source version called Jenkins, discussed below. This left the team fractured and development occuring at a slower pace.

# Jenkins

As mentioned above, Jenkins is actually a seperate branch of Hudson that is being maintained by a different group of people. Accordingly, it has almost all the same pros and cons as Hudson. The one difference is that it is being worked on more actively than Hudson, so there are both improvements and bugs being worked into the software.

# Team City

Team City is a proprietary CI system created by JetBrains.

Strengths:

* can manage multiple builds and multiple build machines
* IDE integration
* pre-commit build testing

Weaknesses:

* no GitHub support
* free tier is very limited (and costs a lot otherwise)
* not open source
* limited language support (Java, .NET, Ruby)

# Bamboo

Bamboo is a proprietary CI system created by Atlassian.

Strengths:

* compatible with major build engines and vcs (?dunvi)
* clean and intuitive user intaface
* add ons for extending capabilities
* heavily integrated branching management (?dunvi)

Weaknesses:

* proprietary and expensive
* issues with CVS

# CI Joe

CI Joe is an open source, extremely simple, CI server created by GitHub.

Strengths:

* dead simple set up
* easy git and GitHub integration
* build any language
* campfire triggers
* easy to access pre and post build triggers

Weaknesses:

* no longer maintained
* hard to customize functionality
* extremely limited feature set

# Integrity

Integrity is an open source CI server.

Strengths:

* GitHub support
* supports and project which can return build error and success codes
* easy configuration
* easy deployment to Heroku
* open source

Weaknesses:

* only supports Git
* many dependencies
* no longer maintained
* doesn't work on 

# BuildBot

BuildBot is a open source CI server written in Python.

Strengths:

* open source
* very few dependencies
* very extensible and customizable
* wide variety of language and platform support
* used by many very well known open source projects

Weaknesses:

* extremely hard to get started
* more like a framework to build your own CI server than an actual solution

# Janky

Janky is an open source CI server developed and used by GitHub.

Strengths:

* built and actively maintained by GitHub
* great integration with GitHub
* simple command system
* easy setup and installation (if you already have Jenkins set up)

Weaknesses:

* requires installation and usage of Jenkins server (see weaknesses and strengths for Jenkins above)
* only manageable through hubot (no web UI)

# CruiseControl

CruiseControl is an open source CI server.

Strengths:

* open source
* well documented
* lots of 3rd party extensions

Weaknesses:

* difficult to install and configured
* not actively maintained
* only support Java, .NET and Ruby

# Summary and Conclusions

Combined, the variety of CI solutions currently on the market have all the features you could ever want in a CI server. Apart however, consumers are forced to pick and choose which problems they will endure to gain certain advantages. We hope to pick and choose the following strengths when designing Rosie:

* single line installation and deployment

For many of the available solutions, installation involves installing the multitude of dependencies for the software before you can ever begin installing it. These installations are often hard to replicate, can take a long time, and dissuade any sensible user from using the product. With single line installation, users will be able to get something up and running in minutes and then go from there. Furthermore, we want to hook up with Heroku, so in minutes you can have a CI server running live on the web.

* intuitive web UI for configuration and build monitoring

Many of the available solutions force you to configure important settings manually in the code—a serious hassle. With an easy to use web UI, we hope to make settings easily accessible and configurable. Furthermore, we want you to know the status of your builds in a single glance—no more digging through layers of UI to get to the important information.

* easy integration with Git and GitHub

Many products do this right, so we'll follow their lead and do it as well. Git and GitHub have pretty much become the standard for version control and easy integration with these services is a must.

* open ended pre and post build triggers

While we want Rosie to be easy to setup, we also want users to have all the control when it comes to the service. With easy to access and set up pre and post build triggers, we'll make it easy to do anything with the code and information Rosie interacts with.

