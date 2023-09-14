layout:true

<p class="footer">
<span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Data and the Web</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://www.datapolitan.com" property="cc:attributionName" rel="cc:attributionURL">Richard Dunks</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative-Commons-License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/80x15.png" /></a>
</p>
---

class: center, middle
![img-center-small](images/pratt_logo.png)
# Data and the Web
## ARCH-851E: Critical Geography and Techniques of Representation
### Richard Dunks

---

class:center,middle
![img](images/big-data-meme-star-trek.jpg)
### Follow along: http://bit.ly/PrattCriticalGeo

---

# Introductions
+ Name
+ Very brief summary of your project
+ What operating system you're using (including the version)
+ One thing you think of when you hear the phrase "open data"

---

# Let's get some downloads started
+ [Python 2.7 via Anaconda](https://www.continuum.io/downloads)
+ [OpenRefine 2.6](https://github.com/OpenRefine/OpenRefine/releases/tag/2.6-beta.1)
+ [JSONView for Chrome](https://chrome.google.com/webstore/detail/jsonview/chklaanhfefbnpoihckbnefhakgolnmc?hl=en)
+ [Sublime Text](http://www.sublimetext.com/2) or [Notepad++](https://notepad-plus-plus.org/download/)

---

# Goals for this Morning
--

+ Introduce key topics in open data
--

+ Demonstrate some key techniques acquiring data from the web
--

+ Demonstrate how to use an Application Program Interface (API)
--

+ Introduce OpenRefine for acquring and cleaning data
--

+ Introduce Python for acquiring and cleaning data

---

class:center,middle
# My Ultimate Purpose:
# &nbsp;<br>&nbsp;

---

class:center,middle
# My Ultimate Purpose:
# Empower you to access data on the web <br> &nbsp;
---

class:center,middle
# My Ultimate Purpose:
# Empower you to access data on the web <br>(wherever it may be)

---

class: center, middle

# Let's Get Started

---

> Facts do not "speak for themselves." They speak for or against competing theories. Facts divorced from theory or visions are mere isolated curiosities.

## -Thomas Sowell *A Conflict of Visions*

---

> We live in a world where there is more and more information, and less and less meaning.

## ―Jean Baudrillard *Simulacra and Simulation*

---

class:center,middle
# Quick History of Open Data

---

# Why do we publish laws?
[![img-right-small](images/massachusetts_laws.jpg)](https://openlibrary.org/books/OL6574549M/The_colonial_laws_of_Massachusetts)

[![img-left](images/peking-gazette.png)](http://bs.dayabook.com/the-peking-gazette-for-1873)

<a title="Asb at the German language Wikipedia [GFDL (http://www.gnu.org/copyleft/fdl.html) or CC-BY-SA-3.0 (http://creativecommons.org/licenses/by-sa/3.0/)], via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File%3AGortys_law_inscription.jpg" target="_blank"><img alt="img-left-bottom" src="images/greek_law.jpg"/></a>

---

class:center,middle
# What good are laws if we don't know how they're implemented?
# &nbsp;

---

class:center,middle
# What good are laws if we don't know how they're implemented?
# Which is what data tells us

---

class:center,middle
![img](images/iquantny_fireHydrant.png)
Source: [Meet the Fire Hydrant that Unfairly Nets NYC $25,000 a Year](http://iquantny.tumblr.com/post/83696310037/meet-the-fire-hydrant-that-unfairly-nets-nyc)

---
class:center,middle
![img-full](images/iquantny_fireHydrant2.png)
Source: [Success: How NYC Open Data and Reddit Saved New Yorkers Over $55,000 a Year](http://iquantny.tumblr.com/post/87573867759/success-how-nyc-open-data-and-reddit-saved-new)

---
class:center,middle

# Modern History of Open Data
![img-full](images/od_timeline.png)

Source: http://fcw.com/articles/2014/06/09/exec-tech-brief-history-of-open-data.aspx?admgarea=TC_ExecTech

---

# Contributors to the Open Data Movement
--

+ Open science
--

+ Open-source software

---
class:center
# The Problem with Open Data

---
class:center
# The Problem with Open Data
![img-center](https://everythingsimpsons.files.wordpress.com/2010/12/boyscoutz4.jpg)

---
class:center
# The Problem with Open Data
![img-center](https://everythingsimpsons.files.wordpress.com/2010/12/boyscoutz4.jpg)
## Data is everywhere around us<br>But it's not easy to access and use

---

class: center, middle

# What is Open Data?

---

class: middle, center
> Open data is data that can be freely used, shared and built-on by anyone, anywhere, for any purpose

## [Open Knowledge Foundation](http://blog.okfn.org/2013/10/03/defining-open-data/)

---

# Key Features of Open Data
--

+ Availability and access
--

+ Reuse and redistribution
--

+ Universal participation

---

# Benefits of Open Data
--

+ Transparency
--

+ Releasing social and commercial value
--

+ Participation and engagement

---
class:center,middle
# Concerns with Open Data

---

# Reliability
--

+ Veracity of source
--

+ Currency of data

---

# Privacy
--

+ Personally identifiable information (PII)
--

+ Mosaic Effect

---

# Confidentiality
--

+ Proprietary information
--

+ Trade secrets
--

+ Government procurement information

---

# Security
--

+ Identify sensitive infrastructure
--

+ Describe methods and procedures

---

class:center,middle
# Open Data Sources
## &nbsp;

---

class:center,middle
# Open Data Sources
## In order of usability

---

# Open Data Portals
--

+ Organize available data
--

+ Provide tools for visualizing, combining, and downloading data

---

# Open Data Portals
![img-full](images/nycopen_data.png)
### https://data.cityofnewyork.us/data

---

# Application Program Interface (API)
--

+ A tool for making a website's data digestible for a computer
--

+ A translation layer between computer systems to allow the exchange of information
--

+ Makes data easier to work with

---

# Application Program Interface (API)
![img-full](images/api.png)
### Source: https://zapier.com/learn/apis/
---

# Application Program Interface (API)
![img](images/api_response.png)

---

# Web Scraping
![img-full](images/web-scraper.png)

[Introduction to web scraping by Thomas Levine](http://thomaslevine.com/dada/web-sites-to-data-tables/)
---

# Web Scraping
![img-full](images/databox.jpg)

[Web Scraping with OpenRefine video from Eric Brelsford](http://www.youtube.com/watch?v=KQlCTo0Q71Q)

---

class:middle,center

# If it's online, you can get the data
## &nbsp;

---

class:middle,center

# If it's online, you can get the data
## Trust me

---

class:middle,center
![img-full](http://cdn.arstechnica.net/03-01-2010/data_liberation_sticker.jpg)

Source: http://arstechnica.com/tech-policy/2010/03/why-google-makes-it-easy-to-leave-google/

---

class:center,middle
# So, let's get some data

---

class:center,middle
![img-full](images/winking-dog-meme.png)

---

class:center,middle
# Let's Scrape Some Data
## http://bit.ly/ScrapeExample

---

# Manual Scraping Example
![img-full](images/man_scraping.png)

---

# Manual Scraping Example
![img-full](images/man_scraping2.png)

---

# Manual Scraping Example
![img-full](images/man_scraping3.png)

---

# Manual Scraping Example
![img-full](images/man_scraping4.png)

---

# Manual Scraping Example
![img-full](images/man_scraping5.png)

---

# Manual Scraping Example
![img-full](images/man_scraping6.png)

---

class:middle,center
# Copy the response
# Paste into text editor
## &nbsp;

---
class:middle,center
![img-full](images/json_raw.png)

---
class:middle,center
# Let's Talk Data Formats

---

class:center
# Data Formats - JSON 
###(**J**ava**S**cript **O**bject **N**otation)
![img-center](images/json.png)
---

class:center
# Data Formats - CSV

---

class:center
# Data Formats - CSV
![img-full](images/csv.png)

---

class:middle,center
# How Did I Get JSON into a CSV?

---

class:middle,center
# Introduction to OpenRefine
![img-center-medium](images/or_book.png)

https://www.packtpub.com/big-data-and-business-intelligence/using-openrefine 

---

# OpenRefine
--

+ In-browser application
--

+ Used to clean data
--

+ Converts data from various file types
--

+ Exports data into various formats

---

# OpenRefine - Pros
--

+ Works with lots of data types
--

+ Great for converting Excel files to CSV (the carriage return problem)
--

+ Facets are powerful (facet on anything)
--

+ Can export to various formats
--

+ Meant specifically to clean data

---

# OpenRefine - Cons
--

+ In browser memory is limited
--

+ Only display 50 rows at a time
--

+ Meant for cleaning data (not displaying it)

---

# Copying Data into OpenRefine
![img-full](images/or1.png)

---

# Copying Data into OpenRefine
![img-full](images/or2.png)

---

# Loading JSON Data into OpenRefine
![img-full](images/or3.png)

---

# Loading JSON Data into OpenRefine
![img-full](images/or4.png)
### Mouse-over the desired JSON level

---

# Creating a Project
![img-full](images/or5.png)

---

# If you get an error about Reconcile service, try this:
### https://groups.google.com/forum/#!topic/openrefine/IkMN-GLm_nw
####(Requires Google login)

---

# Renaming a Column
![img-full](images/or6.png)

---

# Renaming a Column
![img](images/or7.png)

---

# Renaming a Column
![img-full](images/or8.png)

---

# Export Data as CSV
![img-full](images/or9.png)

---

class:center,middle
# I'm assuming you know how to get it into a map from here
<iframe width="70%" height="320" frameborder="0" src="https://richard-datapolitan.cartodb.com/viz/b3b19856-81d4-11e5-91b4-0e3ff518bd15/embed_map" allowfullscreen webkitallowfullscreen mozallowfullscreen oallowfullscreen msallowfullscreen></iframe>

---

class:center,middle
# Want more? 
## See Eric Brelsford's [YouTube video](http://www.youtube.com/watch?v=KQlCTo0Q71Q )

---

class:center,middle
# Let's try that again
### http://nyti.ms/1DOACSp 

---

class: center, middle
![img-full](images/nyt1.png)

---

class: center, middle
![img-full](images/nyt2.png)

---

# CSV Response
![img-full](images/nyt2_csv.png)

---

class: center, middle
![img-full](images/nyt3.png)

---

# Data Formats - TopoJSON
![img-center-small](images/topojson.png)
### https://github.com/mbostock/topojson

---

class:center,middle
# We can automate this
## More on that later

---

class:center,middle

![img-full](images/the-open-data-movement.jpg)
<p>Source: <a target='_blank' href='http://www.paulvanslembrouck.com?utm_source=visually_embed'>ptvan</a></p>

---

class:center,middle
# How do we access all these APIs?

---

# API Steps
--

+ Make a request
--

+ Get a response
--

## &nbsp;
![img-full](images/api1.png)

---

# Using an API
--

1. Register for API keys
--

2. Use the keys for a request
--

3. Parse the response
--

4. Make beautiful visualizations

---

# Example API Response
--

![img-full](images/api2.png)
--

![img](images/api3.png)
--

## This is JSON (**J**ava**S**cript **O**bject **N**otation)

---

# Sample API Request
![img-full](images/4s_api1.png)

---

# Sample API Request
![img-full](images/4s_api2.png)
--

### Endpoint
+ `https://api.foursquare.com/v2/venues/search?`

---

# Sample API Request
![img-full](images/4s_api3.png)
--

### Query Parameters
+ `ll=40.7037253789768,-74.0079939173954`
+ `radius=100`
+ `limit=50`

---

# Sample API Request
![img-full](images/4s_api4.png)
--

### Authentication
+ `client_id=TQTH2POSXDUDYOHKHXM0VKDRCBSSYAFUWMVSWBCI10URJBTR`
+ `client_secret=F3TEHU5APOLSMLSJZYZYUV1SOL5V0V2HUS150YXGTXFPINGS`
+ `v=20140609`

---

# Sample API Response
![img](images/4s_api_resp.png)

---

# Questions?
![img](images/Batman-and-Robin-Running_meme.png)
### https://developer.foursquare.com/docs/venues/search 

---

# Opening API Response directly in OpenRefine
![img-full](images/or_api1.png)

---

# Opening API Response directly in OpenRefine
![img-full](images/or_api2.png)

---

# Opening API Response directly in OpenRefine
![img-full](images/or_api3.png)

---

# Opening API Response directly in OpenRefine
![img-full](images/or_api4.png)

---

# Removing Empty Rows
## Switch to rows
![img-full](images/or_api5.png)

---

# Removing Empty Rows
## Text Facet on Column
![img-full](images/or_api6.png)

---

# Removing Empty Rows
## Select "blank"
![img-full](images/or_api7.png)

---

# Removing Empty Rows
## Remove All Matching Rows
![img-full](images/or_api8.png)

---

# Removing Empty Rows
## Reset Facet
![img-full](images/or_api9.png)

---

# Your turn
## https://foursquare.com/developers/apps  
+ Register for an account (if you don’t have one already)
+ Create an application
+ Provide a URL (`http://www.pratt.edu` works just fine)
+ Get your client ID and client secret


---

class:center,middle
# 10 Min Break
![img](http://imgs.xkcd.com/comics/11th_grade.png)

http://xkcd.com/519/

---

class:center,middle
# Luckily I'm not showing you Perl

---

class:center,middle
![img-full](https://web.archive.org/web/20160321111959/http://howes-it-going.com/perl_ex4.jpg)

https://web.archive.org/web/20191213233500/http://howes-it-going.com/perl_mdb.html

---
exclude:true
class:center,middle
# A Quick Introduction to Python
![img](http://learn.coleggwent.ac.uk/pluginfile.php/350752/mod_book/chapter/5983/royal%20python.jpg)

http://learn.coleggwent.ac.uk/mod/book/view.php?id=198016&chapterid=5983

---

# But first...What is a program?

---

# But first...What is a program?
+ A list of instructions to a computer

---

# But first...What is a program?
+ A list of instructions to a computer
+ Computers can do repetitive tasks quickly and efficiently

---

# But first...What is a program?
+ A list of instructions to a computer
+ Computers can do repetitive tasks quickly and efficiently (unlike humans)

---

# But first...What is a program?
+ A list of instructions to a computer
+ Computers can do repetitive tasks quickly and efficiently
+ Instructions are created by humans

---

# But first...What is a program?
+ A list of instructions to a computer
+ Computers can do repetitive tasks quickly and efficiently
+ Instructions are created by humans
+ Instructions must also be in a form a computer understands

---

# So, what do computers understand?

---

# So, what do computers understand?

<a href="https://twitter.com/CitiBikeDocks/status/632679418264219649">![img](images/cb_status1.png)</a>

---

# So, what do computers understand?

<a href="https://twitter.com/CitiBikeDocks/status/632679418264219649">![img](images/cb_status1.png)</a>

### "success" (In case your binary is a little rusty)

---

# Programming Languages

---

# Programming Languages
+ Help us write instructions in human-readable code

---

# Programming Languages
+ Help us write instructions in human-readable code
+ Human-readable code is then translated into machine-readable code

---

class:center,middle
# This is called "compiling"
![img](https://imgs.xkcd.com/comics/compiling.png)

https://xkcd.com/303/

---

# Why Python?

---

# Why Python?
+ Programming languages vary in structure, syntax, and operation

---

# Why Python?
+ Programming languages vary in structure, syntax, and operation
+ Each have their particular strengths and weaknesses

---

# Why Python?
+ Programming languages vary in structure, syntax, and operation
+ Each have their particular strengths and weaknesses
+ Python sits at the sweet spot between ease of use, functionality, and versatility

---

# Why Python?
+ Programming languages vary in structure, syntax, and operation
+ Each have their particular strengths and weaknesses
+ Python sits at the sweet spot between ease of use, functionality, and versatility

![img-center-small](images/venn.png)

---

class:center,middle
# But don't take my word for it

### http://lorenabarba.com/blog/why-i-push-for-python/

---
class:center,middle
# Now...
![img-center-ml](http://i.giphy.com/oadZJB3hwMFjy.gif)

---

# Open the Anaconda Launcher and Select iPython Notebook
![img](images/launcher.png)

---
class:middle,center
# Open [API_example.ipynb](https://raw.githubusercontent.com/datapolitan/talks_lectures/gh-pages/20151103_PrattCriticalGeography/API_Example.ipynb)
# Save file

---

class:center,middle
![img-full](images/4sq_csv.png)

---

# Advantage of Python

---

# Advantage of Python
+ Iterate through multiple center points

---

# Advantage of Python
+ Iterate through multiple center points
+ Vary the radius and limit

---

# Advantage of Python
+ Iterate through multiple center points
+ Vary the radius and limit
+ Filter for only unique results

---

class:center,middle
# Wrap-Up

---

# What We Covered

---

# What We Covered
+ History of Open Data

---

# What We Covered
+ History of Open Data
+ Definition of Open Data

---

# What We Covered
+ History of Open Data
+ Definition of Open Data
+ How to Get Data from a Webpage

---

# What We Covered
+ History of Open Data
+ Definition of Open Data
+ How to Get Data from a Webpage
+ How to use OpenRefine

---

# What We Covered
+ History of Open Data
+ Definition of Open Data
+ How to Get Data from a Webpage
+ How to use OpenRefine
+ How to use an API

---

# What We Covered
+ History of Open Data
+ Definition of Open Data
+ How to Get Data from a Webpage
+ How to use OpenRefine
+ How to use an API
+ Introduction to Python

---

# Thank you
+ [richard@datapolitan.com](mailto:richard@datapolitan.com)
+ [@datapolitan](https://twitter.com/datapolitan)/[@rdunks1](https://twitter.com/rdunks1)