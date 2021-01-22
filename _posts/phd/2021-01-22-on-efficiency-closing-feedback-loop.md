---
layout: blog
istop: true
title: "On Efficiency: What a PhD taught be about learning and working smart"
background-image: "https://i.ibb.co/gdqzjcH/efficiency-banner.png"
date:  2021-01-22
category: PhD
cite: https://blogs.oracle.com/datascience/how-data-science-can-improve-business-efficiency
thumb: graduation
latest: true
tags:
- PhD
- Productivity
---


<img src="https://i.ibb.co/gdqzjcH/efficiency-banner.png" alt="efficiency" border="0" width = "100%">
<!-- Picture borrowed from CITE-->

## Task and human efficiency are not the same

Efficiency in people is a difficult trait to quantify. We know it when we see it and just as easily can point out when we don't. When efficiency is task-centric, such a balancing a budget or developing software, it is relatively straightforward to track progress and measure success. Consider the quality (and perhaps quantity) of the final product, the time it took to complete, and the resources that were needed to complete it. Integrate these three traits together into something like the following (not a real metric), as you have a proxy for true efficiency!

$$ \text{Efficiency}_\text{task} = \frac{
\text{Quality}_{\text{result}}*\text{Quantity}_{\text{result}}
}
{
\text{Time}*\text{Resources}
}$$

In science, business, economics, and many other fields, there are formalized notions of efficiency for everything from budgeting to energy. Why then, is it so difficult to pin down a theorem for human efficiency? Despite what some believe, human efficiency is not a solved science; if it were, the thousands of self-help productivity books would all say the exact same thing (or at least converge to it in time). Private and public organizations could (and likely, would) standardize their approach to human resources - an enormous "if-else" lookup table on how to eek out every drop of (healthy, productivity-driven) performance from their people. Without further consideration, this doesn't sound so terrible. We all want to perform well, and naturally would seek out environments that optimize us: a human gradient descent.

Yet, this is likely never coming. Why? Because efficiency is dynamic and highly task-specific. For a given task, productivity metrics can usually be defined. However, how do you optimize **across** these tasks, the thousands things people do in a given day or week? Moreover, there are many vital activities we do that have little or no concept of effiency because they don't have a clear notion of success. How does one, for example, have an efficient relationship or outing with your friends? Efficiently settle down and raise a family? 

Indeed, efficiency is largely considered an objective concept best applied to tasks with a common notion of success. The remainder of this article will operate under such an assumption. Yet, it is important to remember that with only 24 hours in a day, everything you do is intertwined by this scarcity. To have relationships, you need time to spend on them. Problems at work have a nasty habit of (at least mentally) following you home in the evening. Thus, becoming more efficient professionally may give you more time to dedicate to things that are not as goal oriented but are arguably more important.

## Efficiency is not the same as effort

Working hard will always be a vital trait in success, personal and professional. However, efficiency and hard work seem to be conflated at times. Certaintly, the two are strongly (and negatively) correlated. The more efficient you are, the less hard work is needed to complete something. This draws up cliches like the "circle - square" image in the header of this article. Yet, a failure to internalize the message remains enormously common. 

For example, when I started as a graduate student, I was offered access to a high-performance computing server to augment my research. To log in, I needed to run several commands - ssh to the server, spin up my virtual environment, launch my development tools, tunnel some of these services back to my local computer, and so on. Running these commands only took 1-2 minutes, but had to be repeated every time my computer went to sleep or I closed out of the terminal.

At first, I simply focused on memorizing these commands so that I would not need to look them up. However, after some frustration with my local internet connectivity (an interruption would close my server session), I decided to look into **aliasing**. Now, with a single command I can spin up my computing environment. Moreover, I installed [Amphetamine](https://apps.apple.com/us/app/amphetamine/id937984704?mt=12), an app that prevents your computer from sleeping even if you close your laptop. Instead of spending 3-4 minutes a day exdecuting commands to log in to these servers, I could immediately launch a session and ensure it remained connected for as long as needed.

## What is worth optimizing: Automate the mundane and repetitive

Now, it is worth asking: "Is that really worth the effort?" Only a few minutes of time saved seems like a small gain considering that it took roughly an hour for me to research and automate these tasks. This is true, and an important question to coninually ask yourself. For many, the discussion begins and ends right here. Some things are really not worth optimizing. 

However, approaching your life with an _optimization mindset_ can have surprising advantages. Instead of thinking about how much an optimization might help you today, consider its benefit aggregated over time. After checking my labs server logs (and some estimation), I found I ran my launch commands ~115 times this fall alone. Even with a low estimate of one minute to launch each session, I saved 2 hours of time. Even small tweaks add up!

## Intra- and Inter-task Efficiency

More generally, holistic efficiency can be thought of in two distinct steps: intra- and inter-task efficiency. Think about how you spend your time each day. What activities commonly arise? Do you often work in spreadsheets? Powerpoint? Software? Make a list of these tasks, then consider them in greater detail. What types of commands do you commonly use? Is there any repetition across your work that could be solved with a macro? Hop from one task to the next, and with each consider the bits that are repetitive. You might be surprised at just how much you can automate. After putting in some initial time, you may find your intra-task efficiency improving with your "super user" tricks.

The second piece of this, inter-task efficiency, is a little tougher to describe and likely has more variation between people. It is essentially how well you can allocate time and energy between tasks of differing type, importance, and effort. In this case, the placement of what you need to do in a given day is likely crucial for how productive you may ultimately be.

As another personal example, I noticed over the fall that a few tasks tended to be **productivity black holes**- namely, research. If I started on research early in the day, the odds I would not finish the homework assignments I had planned to do was much higher. Something about research would suck me in, diverting my attention away from everything else and causing me to lose perspective. To combat this, I started knocking out my homework early in the day, reserving the late afternoon for research where, if nothing else, an urge for dinner would pull me away. 

Sometimes, these productivity traps were not related to other work as much as the characteristics of completing it. I am easily distracted by computers. Sites like [Hacker News](https://news.ycombinator.com/), [Distill](https://distill.pub/), and general Googling can quickly sideline my day.  After noticing this in myself, I did by best to complete all hand-written work first before moving to the computer. Though a small distinction, I found that focusing on and completing even an easy task increased my chances of staying focused on subsequent activities, essentially reaching a state of [flow](https://positivepsychology.com/mihaly-csikszentmihalyi-father-of-flow/). Conversely, if I got distracted in the morning, that trend was more likely to persist through the whole day. Sometimes very subtle differences in your routine can have a cascading effect on your overall efficiency, especially if you perpetuate them.

## Exploration v. Exploitation: You are what (tools) you use

In most of what we do, we encounter the exploration - exploitation trade-off. This is best embodied by the indecision you feel when you go to a restaurant. Do you get something new, or stick with what you know you like? If you explore, you might find something you like even better, but also may be disappointed. Alternatively, by playing it safe you know what to expect but have no idea how much better things could be. This can be extended to relationships, machine learning (especially reinforcement learning), and belies the difficulty in making efficient decisions.

You would never use a hammer to put in a screw, yet few search for optimal tools in technology. This is significant for multiple reasons. For one, virtually everyone uses technology in their work. Even tiny improvements in how you use technology will yield dramatic results over time. Second, there is a productivity tool for nearly _everything_. Spill water on your keyboard and lose function of a few keys (this happened to me)? There is a tool to shift your keys around! Want to run Windows OS on a Mac? Yep, there is a way to do that. Want to convert a word document to a pdf to an image to a gif and embed it in a PowerPoint? You see the idea.

Clearly, exploring your domain for productivity tools is valuable. On one consulting project, I remember another developer showing their code updating and reconciliation process. Code was manually copied down from a remote server, edited locally, saved as "XYZ_\[DATE\]_edit", then copied back to the remote server, ultimately renamed to just "XYZ" after the code reviews. If bugs were found, this process had to repeat, and occasionally files were lost.

You don't have to work in technology to see why this is a problem. It does not matter how brilliant you are; such a long feedback loop to make progress on a project prohibits efficiency, and unnecessarily so. Source control, pull requests, and virtual desktop development immediately accelerated the productivity of this team. Most situations are not as dramatic as this one, but again, even small improvements like automating your server connection add up over time.

## Coming Up: Why research is so hard to understand

Keeping a mindset centered around efficiency is valuable, particularly when learning a new skill, which by definition takes time, repetition, and effort. For me, this challenge came in the form of reading and understanding research in my field. The next post will look into this further, specifically discussing why research papers are so difficult to understand and how a change of perspective can help you understand cutting edge technology.








