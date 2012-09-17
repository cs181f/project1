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


* only manageable through hubot (no web UI)



