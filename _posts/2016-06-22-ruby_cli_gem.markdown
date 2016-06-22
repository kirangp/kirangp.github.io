---
layout: post
title:  "Ruby CLI Gem"
date:   2016-06-22 12:30:45 +0000
---


So here I am, the first test of my Ruby programming career. I have created a Ruby CLI Gem which scrapes the Metacritic website in the PC section and lists the 'Top 10 PC Games of all time' in my gem. Users can select any of the ten games by typing from 1-10 and the gem lists various details about the game.

My gem has two classes `TopGames::CLI` and `TopGames::Scraper`. As the name implies, `TopGames::CLI` class has the code that runs through the CLI section. It mainly focuses on getting user input and displaying output which is called from the `TopGames::Scraper` class. I am listing the start method below which starts by listing the games & calls the `TopGames::Scraper` class for details regarding the game which is given as an input by the user.

![](http://i.imgur.com/bt2SnZj.jpg)

The `TopGames::Scraper` class scrapes the Metacritic website using using Nokogiri. I faced an issue where the website wouldn't open in Nokogiri. After some searching on our beloved stackoverflow, I came across the solution. I had to use a user agent when opening the page. The code is listed below.

```
page = Nokogiri::HTML(open('http://www.metacritic.com/browse/games/score/metascore/all/pc/filtered?sort=desc', 'User-Agent' => 'Mozilla/5.0 (Windows NT 6.0; rv:12.0) Gecko/20100101 Firefox/12.0 FirePHP/0.7.1'))
```

I have listed most of the methods from my Scraper class below.

![](http://i.imgur.com/XXsaHJd.png)

I had lots of fun working on the CLI Gem.








