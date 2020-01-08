# Gainesville Pickleball Website

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

This repo is the source for the web site of Gainesville Pickelball, a 501c3 dedicated to the promotion of the sport of Pickleball in North Central Florida.


## How is this web site managed?

The web site is rendered via [Jekyll](jekyllrb.com), a static website generator. It is based on the [Feeling Responsive](https://phlow.github.io/feeling-responsive/) Jekyll theme. It's hosted by Github using their GitHub Pages feature. This combination makes for an extremely low recurring cost for the web site. It costs no more than the domain name it's presented at.

Analytics are provided via Google Analytics. The Google Analytics tracking id is managed by Philip Chase. 

Managing a Jekyll web site requires skills common amongst software developers. If you have that skill set or have a volunteer who does, such a web site is cheap and secure. If you are non-technical, you can learn this too. 


## Sharing

All of the content for this web site is available under the Creative Commons Attribution 4.0 International Public License. That means you are free to use any of the content as long as you acknowledge where you got it. 


## Site Development

If you would like to manage this web site, you will need to some software tools on your computer and some technical skills to manage them. This is your 10 cent tour.


### Prerequisites

Install these tools on your computer. 

* Any git client - [Github Desktop](https://desktop.github.com/) is good and it provides easy integration with GitHub's service where this repository lives.  

* Jekyll - The [Jekyll Quickstart](https://jekyllrb.com/docs/) guide provides installation instructions for Jekyll and its prereqs.


### Recommended training

You'll be well-served to read the [Getting started](https://jekyllrb.com/docs/) section of the Jekyll docs. You won't have to create the web site, as one is provided in the GitHub repo, but the concepts described in the tutorial will help you understand what Jekyll will do with the changes you make to the files in the repo and how those will become part of the web site.


### Setup

Once the software is installed, clone the git repo at [https://github.com/gnvpb/gnvpb](https://github.com/gnvpb/gnvpb). `cd` into the cloned repo, and run `serve.sh` or this command:

```
bundle exec jekyll serve --config _config.yml,_config_dev.yml
```

That script will run Jekyll in dev mode and serve the content it creates at [localhost:4000](http://localhost:4000)

Access the web site to verify it works before you make any changes.

### Adding Content

The most common things you might need to do are to revise the details on a venue, add an event or write a new post.

#### Update a venue

The venues are described in the [_venues](./_venues) folder. Each venue has its own file that provides all of the facts about that venue. Each venue has a lot of front matter. The front matter is the name-value pairs that occur between the '---' lines. It's used in a template that generates the web page for the site and also in web pages that need to list the sites. Look at [_venues/300.md](_venues/300.md) and compare that page to the web pages at [http://gainesvillepickleball.club/venues/300/](http://gainesvillepickleball.club/venues/300/) and [http://gainesvillepickleball.club/venues/](http://gainesvillepickleball.club/venues/). 


#### Add a tournament

Tournaments are described in the [_tournaments](./_tournaments) folder. As with the venues, each tournament has its own file  that completely describes the tournament. To make a new event, copy an existing tournament file, and adjust the front matter and body to describe the new event. 

Tournaments are listed on the main page with the next tournament at the top of the list. 


#### Add a post

Post are news articles. They are contained in the [_posts](./_posts) folder. Posts' file names are always prefixed with the date of release for the posts.  The date format is `YYYY-MM-DD`.  This date allows the posts to be sorted for display. Posts are presented on the main page with the newest post listed first. 

