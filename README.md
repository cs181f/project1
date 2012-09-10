Rosie
======

## The continuous integration server of the future.

For those who don't know, a continuous integration server has a simple goal: automatically build and test your software as you develop and deploy; always ready to alert you if something goes wrong. It's an extremely important function—but a product space that is very underdeveloped.

At the moment, setting up a continuous integration server is one of the most time consuming, and painful, parts of creating a strong software configuration management environment. Nevertheless, if you ask any software engineering guru, they will tell you that the constant testing feedback a CI server provides is worth the pain. 

A variety of options exist, most notably Jenkins, but each choice comes with a variety of weaknesses. Some solutions are closed source; others are no longer maintained; some only support a few languages; others have extremely limited ability to complete custom builds. Each has it's own problems, but it seems that everyone of them suffers from the same fatal flaw: an impossibly hard installation and configuration process.

With so many flawed solutions on the market, developers are constantly searching for a better alternative: that's where Rosie comes in. The three of us have all struggled with continuous integration servers; we've experienced the problems personally, and we're ready to build a better option.

Judging by the current crop of products, one might think that building a CI server would be a daunting task—perhaps one that would be over our heads—but we think otherwise. Our plan is to cut out the cruft: we'll design and build a simple, easy-to-use, and clean CI server that does what you need...and no more. A friendly web UI for running and examining builds, a speedy backend build queue and queue manager to handle all of the nitty gritty details, and a single command installation interface. Between the three of us, we have all the relevant experience in server management and web development to successfully create such a product.

As we mentioned above, this project is personal: we've had enough of the crappy CI server solutions and we're excited to build an awesome alternative.