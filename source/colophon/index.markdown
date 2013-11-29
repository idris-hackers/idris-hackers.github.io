---
layout: page
title: "colophon"
date: 2013-11-29 10:44
comments: false
sharing: false
footer: true
---

This site is clearly powered by the [Octopress](http://octopress.org/).
Handy links for working with Octopress are as follows:

The main [documentation](http://octopress.org/docs/) also has more information.

+ [Setup](http://octopress.org/docs/setup/)
+ [Deploying with Github](http://octopress.org/docs/deploying/github)
+ [Blogging Basics](http://octopress.org/docs/blogging/)

Handy default steps for blogging:

1. Ensure you have the correct environment for working with Octopress
1. Clone the sites octopress instance:
1. Checkout the source branch
1. Generate content
1. Generate new site
1. Deploy new sites
1. Commit new content
1. push source back.

```
$ git clone git@github.com:idris-hackers/idris-hackers.github.io.git website
$ cd website
$ git checkout source
$ bundle install
$ rake new_post["My First Post"]
$ $EDITOR source/_posts/2013-11-21-my-first-post.markdown
$ rake generate
$ rake deploy
$ git add .
$ git commit -m "A handy message"
$ git push origin source
```

For Ubuntu to set up your Octopress environment:

```
$ sudo apt-get install ruby1.9.3
$ sudo gem install bundle
```
