# Tutorial

This document explains some basics that you'll need to edit webpages and
also gives some links for further reading. Let's start!

DISCLAIMER: The information below might be out of date. Feel free to fix this :)

# Where to start

There are two ways to work with website content.
One way is to edit all the pages directly through github web interface. This is
very simple and doesn't require any additional software.
The second way is to use git client and clone repository to your local computer
and use your favorite text editor to edit pages.

We'll cover both ways.

## Edit content through github

To get some understanding how files in this repository correspond to content
of web pages, we'll start with editing file [index.md](index.md). Text from this
file is shown on the main page of website. For convenience, most of the pages
with content use [Markdown](http://packetlife.net/media/library/16/Markdown.pdf)
syntax for formatting text. Try to edit this file (there is edit button
right next to "Raw", "Blame" and "History" buttons). You may fill some information
about yourself or just add some funny phase like "WOOHOO! I love my website!".
Then use "Commit changes" button and below and go to check [apotapenko.com](http://apotapenko.com).
Your changes should be there almost immediately.
That's basically all it takes to change content on the site. Easy, right?

## Edit content through local git repository

Moving to the second option:
* clone repository
* open index.md in your editor
* write something meaningful(or not)
* save file
* ``git add index.md``
* ``git commit -m "index.md updated"``
* ``git push``

Now you should see the effect of your changes.

## More practice

As soon as you realize all your power, you may want to edit some other
pages and sections of the site:

* cv/index.md
* teaching/index.md
* research/_posts/*
* blog/_posts/*

Editing research and blog posts is a bit tricky, but you should be ok
as soon as you follow given templates and name the files in the same manner
as examples(yes, names matter, they specify page title and date).

# Further reading

If you read this part then you want to figure out how all the web magic works and how can you edit new pages and sections to website. Welcome!

The plan is simple: Just go through the materials that I've selected and you'll get all the basic understanding.
If you have any questions don't hesitate asking me via kashin.andrej [at] gmail.com

* Read [this post](http://jmcglone.com/guides/github-pages/) in order to understand how Github Pages work
* Useful material on pages design syntax: [Markdown](http://packetlife.net/media/library/16/Markdown.pdf)
* Install [Jekyll](http://jekyllrb.com/docs/installation/) to enable local preview before publishing. This can be a problem under Windows, so you can skip this step.

# Technical info

There are some folders and files in repository that we haven't touched yet
* images/ - Obviously, contains images that are used on pages
* css/ - Contains styles for webpages
* _layouts/ - Contains default webpages templates that are used in different site sections
* CNAME - Address to webpage. Required by DNS server that tries to understand
	what to show on your [apotapenko.com](apotapenko.com) page.
* site.md - License, tech details and thanks to previous authors
* _config.yml - Configuration for Github Pages parser called Jekyll.
