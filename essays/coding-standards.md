---
layout: essay
type: essay
title: Coding Standards
date: 2017-02-09
labels:
  - Coding Standards
  - Software Engineering
---

## The necessity of standards 
Standards exist for a reason. They provide consistency and allow for different things to work together. Take this iconic connector known as USB (short for Universal Serial Bus). It's one of the most widely used connectors today. Behind this connector, is a USB standard that all USB-compliant devices must uphold.

<img class="ui medium image" src="../images/usb-port.jpg">

USB is used for a lot of different things. We use it to charge our phones, to connect things to our laptops, and probably for a billion other things. That being said, can you imagine how disastrous it would be if *some* devices decided to use a different standard behind the same connector? Yeah, it would be complete chaos. That's why standards exist, and that's why all devices with USB ports must be compliant with the USB standard.

## My thoughts on coding standards
Let me just start off by saying, standards are a **must**. I'm pretty big on coding style and I've probably invested more hours researching about good coding style than I'd care to admit. Let's just say, I've spent *a lot* of time going through StackOverflow posts and reading people's responses to questions like: [Brackets or no brackets with if-else statements?](http://stackoverflow.com/questions/2125066/is-it-bad-practice-to-use-an-if-statement-without-brackets)

```c
// Without brackets
if (condition)
  stuff;
else 
  other stuff;

// With brackets
if (condition) {
  stuff;
} else {
  other stuff;
}
```

In case you were wondering, I think the example with brackets is better. That was a good question don't you think? I had to think long and hard about that one because I used to write my if-else statements without brackets, but then I realized the error of my ways. In case you're wondering why you'd want to explicitly use brackets, even though you don't need to, it's because sometimes you'll add in another line of code after your initial "stuff" without checking to see if it's actually a part of the if-else statement.

Here's another great question to think about: [Should I use spaces after if-else statements?](http://stackoverflow.com/questions/4368055/coding-style-advice-rationales-for-placing-spaces-in-control-statements-with-c)

```c
// No space
if(condition){
  stuff;
}else{
  other stuff;
}

// With spaces
if (condition) {
  stuff;
} else {
  other stuff;
}
```

I think the second one with spaces is better. I hope you see the importance in questions like the above two.