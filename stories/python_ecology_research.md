---
layout: page
title: Macroeco : Using Python for Ecology Research
---

<h1>Macroeco : Using Python for Ecology Research</h1>

<p>Justin Kitzes and Mark Wilber of the <a href="https://bids.berkeley.edu/">Berkeley Institute of Data Science (BIDS)</a> are the authors of <a href="http://macroeco.org/">Macroeco</a>, a python package that “supports the analysis of empirical macroecological patterns and the comparison of these patterns to theoretical predictions.”</p>

<p>He and Mark put together a great intro video which embedded below —  in fact, I think Justin’s approach should serve as a template for anybody doing an open source Python package: a fully featured package, a useful helper UI, an academic paper and a YouTube video to tie it all together!</p>

<iframe width="640" height="360" src="https://www.youtube.com/embed/mQ4LVw_MQg8" frameborder="0" gesture="media" allow="encrypted-media" allowfullscreen></iframe>

<h2>A Word with Co-creator Justin Kitzes</h2>

<p>Justin was kind enough to answer some specific questions from Tech+Earth about his work on Macroeco and using python as a research tool. (Scroll to the bottom for a quick list of some of the resources Justin mentions.)</p>

<p><em>Q: What kind of setup do you have for working on Python libraries? What IDE or editor, helper tools, common practices?</em></p>

<p>I do my coding in Sublime Text, occasionally making use of Jupyter notebooks as scratch pads. When writing core functions in our package, for example, I would generally work on the function in a module file in my editor, save it, import (and reload) the module in a Jupyter notebook, and run the function with some small test data to make sure it works properly. Once things seemed to be working OK, I’d start writing our test functions, back in my editor, which we then ran with nose. Personally, I’m probably more proud of our test suite than any other element of our package – very few scientific packages are well-tested, and we invested a lot of time in getting very good coverage with difficult and detailed examples.</p>

<p>In terms of best practices, we largely followed the basic principles that are taught by Software Carpentry for good scientific programming, including structuring code, using version control, and project organization. I have a series of lessons on those ([http://datasci.kitzes.com](http://datasci.kitzes.com/)) that I use for my own teaching.</p>

<p><em>Q: What are some of the challenges to creating open source libraries for scientific research and a community of peers?</em></p>

<p>I think that the biggest issues don’t really have anything to do with the library itself, but instead relate to discoverability and documentation. Promoting your package and making it easily and independently usable by others are difficult tasks, and not ones that are normally part of our basic scientific training (or even our training in scientific programming). Moreover, scientists don’t tend to get rewarded for writing code, which further decreases the incentives to do a good job beyond just “getting the answer” for a manuscript.</p>

<p><em>Q. Why did you choose the BSD license?</em></p>

<p>I’m generally of the belief, as are many of my colleagues, that the BSD and MIT licenses are “more free” than the GPL, for example, as they place essentially no restrictions on the use of our code. We went with BSD over MIT because, hey, had to represent Berkeley!</p>

<p><em>Q. You created Macroeco Desktop, a simple interface that requires no programming, for users who don’t have much experience using Python. What percentage of your audience do you think uses the UI because they’re not comfortable with the command line? Do you intend to put more work into the UI in the future or focus on the library itself?</em></p>

<p>I would guess that the lower level package is more widely used than the UI at this point, as most people who are discovering our package are (understandably) already programmers, and so are capable of importing and using the functions at a relatively low level. This relates to the issue of discoverability – it’s not as easy to reach people who don’t know how to code and try to convince them to try a new piece of software. That said, my co-author and I use the UI all the time!</p>

<p>Going forward, I think that we could probably have a lot of impact by pulling out and generalizing the UI as a separate package, so that could be attached as a front end to packages written by others. One immediate challenge, though, is that we build the UI with wxPython, which is not yet fully ported to Python 3, so we might have to rewrite parts of the interface going forward.</p>

<p><em>Q. What other software technologies, frameworks or practices are important to your work?</em></p>

<p>I tend to work in both Python (my preference) and R (when necessary), and I make fairly extensive use of the usual Mac OS X stack – Sublime Text, Jupyter, Homebrew, pandoc, and LaTeX, to name a few.</p>

<p><em>Q. For the young ecologist, or scientist working in a field related to the environment, what’s the best way to become proficient in the software side of things? What educational resources do you recommend?</em></p>

<p>I would recommend more or less the same way that I learned, which has three parts. First, take some sort of workshop or bootcamp to get yourself exposed and up to speed on some very basics. Software Carpentry and Data Carpentry are great for this. Second, find yourself a mentor who’s already good at this stuff, and find some way of collaborating with him/her, even if it means volunteering your time. This is by far the best way to learn – it’s no accident that the apprenticeship model is so widespread and long lasting. Third, try to do something on your own, and use concrete projects as a means of expanding your skill set. So don’t set out to just learn some new method or technique, pick a project that you really want to do and learn new skills and approaches as they become relevant to completing that project. You’ll quickly learn to value quick Google searches and Stack Overflow when you run into trouble.</p>

<p><em>Q. What’s other new and interesting projects are out there right now that make you go “WHOAH!”</em></p>

<p>I don’t know about WHOAH!, but one thing that I do have my eye on are the increasing push towards suggesting, or requiring, that scientists follow good reproducible research practices, which is an area that I’m personally very interested in. I think that another “big deal” is going to be the rise of containerization technologies, like Docker, that help solve dependency and setup problems, which are hugely important and probably under-appreciated challenges to sharing and reusing code.</p>

<p>And there you have it. You can follow Justin’s latest work on his website: http://www.justinkitzes.com/. And if you are working on a tech project related in some way to a more sustainable future, [ping me](https://twitter.com/danielmcq) and let me know!</p>

<span style="color: #999999">[1] Kitzes, J. and Wilber, M. 2016. macroeco: reproducible ecological pattern analysis in Python. – Ecography 39: 361–367 (ver. 0).</span>

 

<h2>Resources:</h2>
<ul>
	<li><a href="https://web.archive.org/web/20161026192040/http://software-carpentry.org/">Software Carpentry – teaching basic skills for research computing</li>
	<li><a href="">Sublime Text</a></li>
	<li><a href="">Jupyter</a></li>
	<li><a href="">Homebrew</a></li>
	<li><a href="">pandoc</a></li>
	<li><a href="">LaTeX</a></li>
	<li><a href="">nose a python unit testing framework</a></li>
	<li><a href="">Docker a virtual container technology for software</a></li>
	<li><a href="">wxPython a blending of the wxWidgets C++ class library with the Python programming language.</a></li>
</ul>



