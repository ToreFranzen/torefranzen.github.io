---
layout: post
title: "Intro to Hacking the BrewPi"
date: 2016-09-04 00:29:17 -0400
comments: true
categories: 
---
Intro
-------------
For those that don't know, [BrewPi](http://www.brewpi.com/) is the answer to modern man's problem of controlling Beer fermentation temperature. Originally, it was a Raspberry Pi coupled with an Arduino (and more currently a Photon Spark). The Arduino (or Spark) acts as the work horse of the operation by measuring temperature and controlling heat and/or cooling for the fermentation chamber. The Raspberry Pi would act as a web server, displaying information and sending commands to the Arduino (or Spark). The creators of the project have also kindly posted their code in git hub [https://github.com/BrewPi](https://github.com/BrewPi).

WTF Are you trying to do? The thing works already!
-------------
What I would like to do is remove the Arduino and still have a functioning setup. Initially, this looks like it might take some time and thought. I want to do this as a learning experiment. There is no intention on sabotaging the efforts of the BrewPi team. They rightfully deserve credit and I have the utmost respect for them and the product they have created.

With all that out of the way, I have come up with a few ideas of how I can make a stand alone BrewPi out of the Raspberry Pi (3):

 - Understand the Arduino/Spark code and rewrite into python code (or something else, i.e. bash) to run in an infinite loop on the pi
 - Create wrapper code around the existing firmware and simulate on the pi
 - Something else?
 - Forget the whole thing and go buy an Arduino

So Whats Next?
-------------
Not much besides delving into the [BrewPi git hub repo](https://github.com/BrewPi) and trying to figure out how the darn thing works. So far, I have learned about the [PID algorithm](https://en.wikipedia.org/wiki/PID_controller) and am currently figuring out how its implemented in the BrewPi. (Note: I have a Computer Science background and not one in electronics or control theory). Hopefully there will be more status updates to come.