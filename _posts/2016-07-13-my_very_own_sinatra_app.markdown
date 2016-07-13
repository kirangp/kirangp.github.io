---
layout: post
title:  "My very own Sinatra app"
date:   2016-07-13 09:07:14 +0000
---


So the time has come to write a blog about my very own Sinatra web app. For the past few fortnights I have had a chance to get my hands dirty with SQL, ActiveRecord, Rack and Sinatra. I really started liking Sinatra mid way through my Learn curriculum. It is like a trained dog. It follows your orders & executes the web application the way you want it to execute. If there are any problems in the execution it is very easy to pinpoint towards a particular point using pry.

### PC-Builder

Well I am an avid PC fan & decided to make a custom PC builder website using Sinatra. It is a very simple application which has the following functionalities.

1. A guest can check the current the PC builds already created by users.
2. A guest can register for an account using a username and password.
3. A guest can login to the website using a username and password.
3. A logged in user can create a new PC build with a build name and price.
4. Once a build is created, you can add a system configuration with a CPU, Motherboard, RAM, Videocard, Storage Powersupply & case. You can associate a system with a build name.
5. A logged in user can edit a system or a build.
6. A user can logout of the website.


### pry-rails gem

There were times when I wanted to pause my execution in an erb file but couldn't do it with the pry gem. But someone has already released a pry-rails gem which can be used inside an erb file. 

To use the gem include it in your Gemfile.
![](http://i.imgur.com/U5UyHXq.png)

And you can use binding.pry inside your erb like this

![](http://i.imgur.com/1MXboOa.png)

### Future
I have a few ideas which I can implement in future to make the website workable.

1. Users can add price for individual parts.
2. Users can add pictures of their builds.
3. Users can add the framerates for games & application start up time to help users decide about the builds.




