---
layout: essay
type: essay
title: Final Project Ideas
date: 2017-02-23
labels:
  - Software Engineering
  - Meteor
---

# Overview
Parking at the University of Hawai'i is limited. Furthermore, just getting to university is a task in itself because of the heavy congestion drivers face.

## The problem
Parking is limited and can be expensive. Not everyone can get a regular parking pass, as they are prioritized by class standing. However, there is a carpool pass, which functions similarly to a regular pass, except during peak hours, the driver has to be accompanied by other riders.

## The solution
The solution is to match drivers with carpool passes with riders who are along the way. This will benefit both the driver as he/she now essentailly has a regular parking pass, and it benefits the riders because they no longer need to commute themselves. Furthermore, this benefits the entire community as it reduces the number of cars on the road, leading to less congestion and thus, faster commutes.

# Page ideas
The app will consist of several pages:

* A login page where UH students and staff login with their credentials
* A menu where you can either post (as a driver looking for riders) or search (as a rider searching for a driver)

# Use-cases
Here are some use cases:

* Drivers will input their latest departure time and a max radial distance that they're willing to pick up someone from, riders will input the time they need to get to school by, app will match drivers with users
* On-demand scheduling for riders who missed their scheduled assignment, can look for upcoming scheduled assignments with seats left and with destinations near the user's address
* Interface for easy commands such as "I'm on my way", "I won't make it, go without me", or an actual chat window for more detailed messages

# Beyond the basics
* Users can post their schedule, location, and app will generate possible matchings between drivers and riders
    * Maybe 'search along the route' option where destination is not limited to just the driver's location radius
* Integrate Google Map's traffic data to get real-time estimates on commute time
* Calendar for the drivers and riders that can sync with their Google calendar to tell them who their driver is, when they're leaving, etc.
* Payment system where the riders can contribute to the driver's gas/parking pass fees