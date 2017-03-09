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
I'm learning how to use the Meteor framework as a part of my Software Engineering course. At the time of writing this essay, we've only been about two weeks into Meteor, but we've already encountered a slew of problems, ranging from small but annoying error messages, to hour-long build times. Today, I'll tell you about my struggles with Meteor and how I managed to solve (or deal with) them.

# Problems setting up
Anyone who develops in Windows knows *the struggle* of doing so. Integration problems, compatibility issues, you name it. After a while, it gets to the point where you *expect* something to go wrong, and have Google open, ready to start your journey for a solution.

Our instructor, Dr. Johnson, warned us (the Windows users) that installation may either go perfectly fine, or it may go terribly wrong. So when it actually came time to install Meteor, I set aside a two-hour block of time in preparation of things going terribly south. However, 10 minutes later, the installation finished, and I breathed a sigh of relief. Too bad that didn't last long.

## The problem
The first real issue came when I was halfway through a Meteor tutorial. At this point, I had my Meteor server running and everything was working fine. I was able to make changes to the html file and it showed the changes correctly. It was when I had to create a JavaScript file and rebuild my application, where I was greeted with the following error:

<div class="ui centered grid compact segment">
  <img class="ui large image" src="/images/windows-jscript-error.png">
</div>

Great. I knew it was only a matter of time, but it still would've been nice to be able to have gone through an entire installation and demo without having some kind of vague error.

## The search for a solution
I followed the traditional routes: Error message->Google->Forums->Back to Google, etc. It didn't lead anywhere. So I did what anyone would do and went back to the very beginning to see if the problem persisted. It did not. Now I know that somewhere between the very beginning and then, I had broken Meteor. I went step by step and a few minutes later, found that the error was coming from my JavaScript file. I commented everything out (because that's what you do when things break) and it worked. It was a pretty simple fix and so that's what I went with.

Not an hour goes by and one of my classmates suggested another fix. He said the problem was associating the JavaScript file with Windows Script Host and that it would be solved by changing to association to IntelliJ. And so that's what I did:

<div class="ui centered grid compact segment">
  <img class="ui large image" src="/images/javascript-associate-intellij.png">
</div>

Lo and behold, it works! Curious, I probed further and changed the file association to something different. Surprisingly it works with not only IntelliJ, but Chrome as well. So here's my theory: when you build Meteor, somewhere along the lines, it will try and run the JavaScript file with whatever program that's set to handle it. For some reason, Windows Script Host was throwing an error and didn't allow the build to finish. Setting this to IntelliJ or Chrome will fix this issue because it doesn't throw an error when Meteor tries to open the file with IntelliJ or Chrome.

# Problem building
So now that I've gotten somewhat used to building and running Meteor applications, I thought my struggles would be over and that Meteor would be all good now. Unfortunately, that wasn't the case when it came time to do 'Digits'.

Just a brief overview, 'Digits' is the name of a Meteor application that we were to recreate. It involved us starting with a template and making modifications to match the example given. We were given ~45 minutes to work on this in class.

## The problem
As usual, I started working on the application by following the instructions step by step. I created a git repo on GitHub, cloned it over locally, copied the template files, and ran `meteor npm install` in the app directory. Those worked fine.

What didn't work was the next step, which was to run meteor with a config file. Meteor said it needed to download some files so I said OK. However, instead of taking a few minutes to download, the ETA it gave me was 3000 seconds. That's almost an hour! I weighed my options: I could just let it do its thing and hopefully it will go away the next time I try to run it, or I could stop it from downloading and try to Google a solution. I figured the latter would most likely take longer than the hour-long download, so I just let it do its thing.

## The solution
It turned out that the hour-long download wasn't the end of it. After it was done downloading, it wanted to do more things (at this point I just let Meteor do its thing) so I just let it go. Whatever it was doing, it made my computer really hot and really loud. My CPU temperature was in the **high 80s** and my fans were blaring! I was ready for my computer to catch on fire.

<div class="ui centered grid compact segment">
  <img class="ui large image" src="/images/laptop-fire.jpg">
</div>

Just joking. Although, I *was* pretty nervous, but continued to hope that Meteor would fix itself.

After about ten minutes of Meteor torturing my laptop, the temperatures started dropping and the fans started slowing down. Whatever happened, it's over now. Meteor finished running and I can view the website as expected. I even tried a reset and another run, and...it worked. It seemed that whatever it did, it was a one-time thing and *hopefully* I'll never have to deal with that again.

We'll see. I have to do Digits part 2 tonight.