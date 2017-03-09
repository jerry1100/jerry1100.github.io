---
layout: essay
type: essay
title: Meteor Struggles
date: 2017-03-09
labels:
  - Software Engineering
  - Meteor
---

# Preamble
I'm learning how to use the Meteor framework as a part of my Software Engineering course. At the time of writing this essay, we've only been about a week into Meteor, but we've already encountered a slew of problems, ranging from small but annoying error messages, to hour-long build times. Today, I'll tell you about my struggles with Meteor and how I managed to solve them.

# Setting it up
Anyone who develops in Windows knows *the struggle* of doing so. Integration problems, compatibility issues, you name it. After a while, it gets to the point where you *expect* something to go wrong, and have Google open, ready to start your journey for a solution.

Our instructor, Dr. Johnson, warned us (the Windows users) that installation may either go perfectly fine, or it may go terribly wrong. So when it actually came time to install Meteor, I set aside a two-hour block of time in preparation of things going terribly south. However, 10 minutes later, the installation finished, and I breathed a sigh of relief. Too bad that didn't last long.

The first real issue came when I was halfway through a Meteor tutorial. At this point, I had my Meteor server running and everything was working fine. I was able to make changes to the html file and it showed the changes correctly. It was when I had to create a JavaScript file and rebuild my application, when I was faced with a Windows Script Host error:

<img class="ui medium image" src="/images/windows-jscript-error.png">