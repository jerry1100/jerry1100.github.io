---
layout: essay
type: essay
title: Necessity of Standards
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

```javascript
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

In case you were wondering, I think the example with brackets is better. I had to think long and hard about that question because I used to write my if-else statements without brackets. However, I read in the comments that writing if-else statements without brackets could lead to bugs in the code, I made the change. In case you're wondering why you'd want to explicitly use brackets even though you don't need to, it's because sometimes you'll add in another line of code after your initial "stuff" without checking to see if it's actually a part of the if-else statement.

Here's another interesting question (IMO) to think about: [Should I use spaces after if-else statements?](http://stackoverflow.com/questions/4368055/coding-style-advice-rationales-for-placing-spaces-in-control-statements-with-c)

```javascript
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

I think the second one with spaces is better. I know that some of you will feel that questions like these are a waste of time and that I should be focused more on the quality of my code rather than how it looks, but I'd argue that good-looking code *is* a necessary condition of quality code. Try writing code "your way" and request for it to be added to a project like the Linux kernel, Linus would not be happy with you. That's not to say that you're a bad programmer, but in large software projects, there is a *huge* emphasis on coding standards. That being said, you have to make sure your code is compliant with *the standards*, even if it means not following *your standards*. This is to ensure that the codebase is uniform and maintainable. That's why companies like Google also put out [their own coding style guide](https://google.github.io/styleguide/cppguide.html).

## Thoughts on ESLint
Now that I've talked a little about my thoughts on coding standards, let me talk about my experiences with ESLint. First off, I'm on Windows 10 and installing it was a pain. Thankfully however, I managed to string together a configuration that worked after about an hour. Conveniently, a day later, my professor sent us a guide detailing exactly what we needed to do to get it working.

Anyway, I think ESLint is fantastic. It's amazing to be able to see instant feedback on your code and whether or not it's up to the standard. The only thing I don't like about the standard is that they use 2-space indentation rather than 4, but that's not a big deal. When I have some free time, I'll definitely have to look into getting something like ESLint for other languages like C and C++.
