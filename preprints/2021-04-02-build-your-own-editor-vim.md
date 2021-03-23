---
layout: blog
istop: true
title: "Ode to Vim: Why building your own IDE is worth the effort"
background-image: 
date:  2021-04-02
category: Development
cite: https://stackify.com/top-integrated-developer-environments-ides/
thumb: code
latest: true
tags:
- Productivity
- Development
- IDE
- Vim
---

<!-- Picture borrowed from CITE-->
<img src="https://i.ibb.co/5hPP9rj/IDE.jpg" alt="IDE" border="0" width = "100%">

## What do you love about your favorite IDE?

For software developers, an IDE can make or break productivity. The more familiar you are with an IDE's specific structure, shortcuts, and nuances, the better you will be at building software in general. Some choose IDEs specific to a language, such as PyCharm or IntelliJ. Others prefer simpler text editing tools like Sublime, Atom, or Notepad++. Whatever you personally choose, I am willing to bet that if you have worked with it for awhile that you would live and die by that editor. In some ways it becomes and extension of ourselves at work, school, any time we are writing code or editing text.

Yet, certainly there is _something_ that your current IDE does not offer that might be helpful. At the same time, unless you are a super-user who scours documentation tip to tail, it is likely that you are not aware of all the shortcuts, tips and tricks an IDE has to offer. This is indeed part of the fun of development - there is always something new to learn. Why then, you might ask, should you switch at all?  

##  Why I decided to switch to Vim

For years, I worked primarily with Sublime Text editing. Though Sublime's initial learning curve is small, it provides an immense amount of flexibility and complexity in the form of `Install Packages` and custom build systems. In fact, that is what initially drew me to Sublime. With a push of a button, `CONTROL-B` to be precise, you can build your current file with any build system you have set up. If you wanted to work in Java, just drop down to the Java build system. The same goes for Python, C++, Markdown, and anything else. Sublime's structure is built around minimalism and simplicity, with more than a few powerful tricks packed in (`CONTROL-D` for multiple cursors is one of my favorites).

Yet, as I started graduate school I noticed that I would repeat many of the same commands to complete just one assignment. As an example, if I needed to build a predictive model, the overhead I suffered to debug it grew as I progressed in the project. If I was nearing completion, I might need to run several build up steps to even test what I was currently working on. This migh take only a minute, but I noticed that in many cases I would need to re-run this step several times to debug my code completely.

With time, I wised up and started storing intermediate steps in Jupyter notebooks, porting out features only when I was fairly certain they would accomplish what I intended. Yet, this led to lots of clicking back and forth between Jupyter and Sublime, straining my hands and slowing me down. In some cases, I was now jumping between three and four different IDEs - Jupyter, Sublime, Overleaf for LaTeX documents, and the command line to push my changes to a Github repository. All of these different environments made me very good at `CONTROL-TAB` for switching windows, but regardless I felt that I was spending way too much time hopping and sharing items between IDEs. Eventually, I began to search around to see if there was anything that would allow me to accomplish all of these tasks from the same window.

## Don't mourn the death of your mouse

At first, a tool that integrated several of my IDEs together seemed unlikely, especially considering I had never heard of one after working in technology for a handful of years. Perusing the internet led to many different approaches to this problem. Some people attempted to created custom scripts that made the handoff between these environments easier. Others took advantage of plugins (of varying quality, in my experience) to try and jam functionality into their development environment of choice. Most intriguing of all, however, was the sheer number of posts that recommended using Vim, a text editing tool with origins nearly as old as computing itself. Though there are many things that make Vim unique from other systems, perhaps it's most defining trait is its use of compositional keymappings built to replace the need for a mouse. Compositional keymappings is a mouthful - a simple way of thinking about this is applying an action, or `verb`, to an object or `motion`, to use Vim-speak. For example, the verb for delete in Vim is `d` and the motion to move down a line is `j`. So, if you wanted to delete your current line and the one below it, you would just type `d2j`.

I had heard of Vim before, but always thought it was for old-school programmers who got their start with systems that did not have a mouse. Plus, I just couldn't understand how someone could be more productive without the use of a mouse. However, then I noticed there were several graduate students who were also using Vim for their development. In particular, one labmate explained quite simply the idea of Vim - **Never leave the home row**. 

Though it seems like a flash, the time it takes you to move your hand to the mouse and back to thkeys adds up for most people who work on a computer all day. Giving the keyboard the expressivity to accomplish everything and mouse can (and more!) makes you faster as well as more precise and efficient.

## Climbing Vim's learning curve 

Unfortunately, this efficiency does not necessarily come cheap. Among editors, the learning curve to work in Vim is one of the steepest, primarily because it removes the need for a mouse entirely. Moreover, 


## What you get for giving up your mouse 

## How to build your IDE from the ground up 

## Additional tricks
