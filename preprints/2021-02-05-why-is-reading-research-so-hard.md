---
layout: blog
istop: true
title: "Notation and Formality: Why research publications are confusing"
background-image: ""
date:  2021-02-05
category: PhD
cite: 
thumb: graduation
latest: true
tags
- Research
- Literature
- Education
- Imposter Syndrome
---

<img src="https://i.ibb.co/bRkLHwP/slope.jpg"  alt="notation_spec_theta0" border="0" width = "100%">
<!-- Picture borrowed from CITE-->

## Who teaches the teachers? A perspective on formalized education

By the time we graduate high school, nearly all of us can read, write, and understand most math fundamentals. We could pick up virtually any textbook and, in the literal sense, read it cover-to-cover. What then is the purpose of spending thousands of dollars to have someone else walk you through more advanced concepts? Why not simply read the textbooks on your own?

Far from a trick question, professors - experts in their field - ideally give students a look beyond course content into something more. Insights stemming from how experts think about and solve problems are at times more valuable than the subject matter itself. Despite how codified knowledge has become, there are still tips and tricks that will inevitably be passed experientially and can't be found in books. 

Yet, who are professors going to learn from? Well, with their strong, sound bank of knowledge, they often self-direct their learning, digesting new concepts on their own. Most often, these "new concepts" are found in research publications that bring together existing knowledge and new ideas in valuable ways. The act of becoming excellent at self-guided learning - reading, understanding, and producing new research publications - has been formalized in the Doctorate of Philosophy, or PhD.

## Translating formal into conceptual   

Have you ever been in class (probably a math class), and in the middle of the lecture whispered to your friend: "ok so what exactly is he/she saying?" At first glance, your question appears prompted due to an inability to understand the content they are currently teaching. That is true, but the true question is more subtle than that. The fact you are in this math class at all implies that you at least superficially understand all the concepts on which your current lecture is built. It is unlikely that this new content is built on completely foreign concepts. More likely, it is understanding how this new concept connects to what you already know that you are stuggling with. 

In my experience, this is perhaps the most common mistake I feel I have seen teachers make. When I have struggled with new content, it is almost always due to an inability to connect the topic to my existing web of knowledge. Many studies on memory and cognition show that humans retain information much better when they can associate it relative to other knowledge. If you are curious about how this works, I highly recommend the book [Moonwalking with Einstein](https://www.amazon.com/Moonwalking-Einstein-Science-Remembering-Everything/dp/0143120530). This issue can arise due to even simple distinctions in notation or teaching style and, though individually insignificant, can aggregate big-time confusion.

## Understanding the notation monster with a toy example

As a toy example, consider the following function and optimization.


--------------------------------
Let $\mathbf{X}$ represent the set of observation vectors $\{\mathbf{x}^{(1)},  \mathbf{x}^{(2)}, ... ,  \mathbf{x}^{(m)}\}$ where  $\mathbf{x}^{(i)} \in \mathbb{R}^{n}$. For each input vector $\mathbf{x}^{(i)}$ there exists a label $y_i \in \mathbb{R}$ mapping the input to a continuous, real-valued target. Furthermore, consider the function $f_theta(.)$ to be an affine mapping from $\mathbb{R}^{n} \rightarrow \mathbb{R}$ of the form:

$$ f_{\theta}(\mathbf{x}^{(i)}) = \mathbf{w}^{T} \mathbf{x}^{(i)} + \mathbf{b} $$

The generating data distribution of $\mathbf{X}$ is assumed to be Gaussian, and therefore a mean squared error objective function was utilized to train the model. 

$$ L(\mathbf{X}, \mathbf{y}) =  \frac{1}{m} \sum_{i = 1}^{m}{(f_{\theta}(\mathbf{x}^{(i)}) - y_i)^2} $$

Though an analytical solution was possible, due to the large input space $n$ and number of data points $m$ stochastic gradient descent (SGD) was utilized to iteratively converge on the optimal parameters $\theta^* = \{\mathbf{w}^*, \mathbf{b}^*\}$.

---------------------------

Head hurt? Mine hurt writing this. Unless you are a math-savvy individual who works or plays in a technical field, then it is likely at least some of this did not make sense to you. When I started reading research written this way, I would jot down a (long) list of things I did not understand to return to later. Not long ago, my list would have looked like this:
- What does "affine" mean?
- I remember that fancy looking "R" from math class, but what did it represent and what does the "d" exponent mean?
- What does the arrow between the fancy "R"s mean?
- Why are some letters bolded and some not?
- What does the $\theta$ subscript mean?

The length of your list will differ based on your expertise, but even if the passage above makes complete sense to you, you'd likely agree that this is extremely _formal_. What are you trying to show with all of this technicality? Is this at all similar to anything that I have seen before?

## Simplicity in disguise

As you likely guessed, the arcane description above has some connection to your vast bank of previous knowledge. Even if you scorn math, I bet you have seen the following before:

$$ y = mx + b $$

Indeed, most likely remember slope-intercept form from school, even if they have not used it in decades. Intuitively, you can see that $m$ scales $x$ larger or smaller and $b$ shifts it up and down. The purpose of all this shifting is to ultimatelu match up points on an x-y plane such that a line passes as close to them as possible. As you got older, perhaps you started to see $y$ get replaced with $f(x)$, a slightly more functional form.

Though dressed up in pomp and mathematical formalism, **Both of these sections are logical extensions of slope-intercept form for linear regression**. The objective of both of these equations is the same - place a line so that it is as close to data points as possible. Essentially, the difference between the two is as follows:
- Slope-intercept form assumes that the input data has only one "feature", or dimension (only one "x" in $f(x)$). By contrast, the original description is for multiple linear regression, where multiple inputs are used (muliple "x"s, muliple "m"s)
- In elementary school, $f(x)$ is usually optimized by using "rise-over-run" techniques for $m$ and then plugging in different $x$ and $y$ values for b. This was largely a visual endeavor of counting. Since it is harder to visually consider data with more than three features ("x"s), multiple linear regression finds its optimal "m"s and "b"s with stochastic gradient descent, a more sophisticated approach.

Still not convinced? Consider the following explanation. All that discussion of dimensions and mappings is a formal way of saying 

> We have a dataset of m rows and n columns. For each row, we have a single number that we want to be able to predict given the input values in each column of that row.

The idea of using $f_{\theta}(.)$ to map the input is just another way of thinking about the problem. Somehow, we want to convert our input into a desirable output of a different dimension. This is no different than wanting to get a specific value for $y$ by plugging $x$ into the function $f(x) = mx + b$. Lastly, the talk of the loss function and data generating distribution is a formal way of motivating a chosen optimization, again to find the best "m"s and "b"s for our function. At the end of the day, all we care about is getting a specific "y" from our "x"s using "m"s and "b"s, just like back in grade school.

## Why so stuffy? The role of formality in research

At this point, you are likely asking "If these simple and advanced topics are so similar, why be so obtuse in your description?" For one, topics do not always extend so smoothly from our grade school experiences. The world is a complex place; it makes sense that at times our manner of describing it would be complex as well. However, in many cases there is another explanation - the writers wish to be **exact**. Ideally, they want to write in a way that regardless of the culture, language, and domain of the reader, someone with "X"-level expertise in mathematics can understand their ideas. 

However, the problem here is that as technology has progressed, the assumed "X"-level of expertise needed to understand these papers has become incredibly high. Research papers are not read like newspapers. They are pored over, disected, parsed through line-by-line. Even after several months of practice, I still find myself wishing that research papers would cut through their notation jungles and discuss their ideas conceptually, as if I were chatting to the authors over a beer. Ideally, advanced ideas could be explained in a way that connects them to more rudimentary concepts. Indeed, some excellent research papers do exactly this, but unfortunately such gems are rare.

Fortunately, I am clearly not the only researcher who wishes to make technical publications more accessible. To my delight, websites and blogs like The Batch, Distill, and Towards Data Science all attempt to engage a less expert audience. Like many, I used to question my ability to understand research and technical publications generally. Sometimes, I still do. Remembering why these publications are written so formally, as well as recognizing resources built to connect this work to you existing knowledge will make you a much happier, effective reader and self-guided learner.

## Coming Up: The importance of giving technical presentations

Writing up technical ideas clearly is difficult but centrally important. As with any language, mathetmatical and scientific notation endeavor to define precise meaning to symbols, codifying the intent of the researchers. Harder still, however, is presenting your complex, interdisciplinary, months-long research to a non-expert audience in under 15 minutes. In the next post, I take a look at the importance of effective presenting and communication in research.









