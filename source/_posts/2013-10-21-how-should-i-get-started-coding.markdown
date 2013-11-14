---
layout: post
title: "How should I get started coding"
date: 2013-10-21 23:11
comments: true
published: true
categories: developers learning programmingπ job-advice
---
I'm asked so many times "how can I / my friend / my child get into programming?"

With the growing influence of technology in business, the amount of attention on the "tech startup" scene including the governments TechCity initiative, the widely proclaimed shortage of technical talent and numerous articles pushing software development as a top career choice, this is likely to be asked even more frequently. I've been iterating on an email response to people who ask and thought I'd share it.

There are plenty of resources on the web on every conceivable language and tool, but I haven't seen anything that maps out how a learner can progress from nothing to a professional developer standard, leaving people confused about where to start and how to go about it.

My suggested plan is listed below, it's not essential that they be followed in order, but each level gives the learner the building blocks they need to progress and offer a nice progression in my opinion.

* Learn the basic web page technologies
* Write lots of code
* Deploy a web page / site to a live environment
* Write lots of code
* Learn JavaScript and jQuery
* Write lots of code
* Learn a server side language and framework
* Write lots of code
* Get a grounding in multiple languages and paradigms
* Write lots of code
* Join meetups and open source projects
* Write lots of code
* Get some work experience
* Write lots of code
* Keep learning

The below is aimed at people new to software development, so a lot of detail has been ignored, and things simplified in an effort to get the learner moving as quickly as possible. Like an onion with multiple layers, as the learner progresses through the different stages, more details will be revealed to them.

# Learn the basic web page technologies
Web pages are the building blocks of the internet, and the current suite of web page technologies; HTML & CSS are a good starting point for somebody wishing to get into programming. Manipulating a few text files, refreshing a browser and seeing the effects of changes can be extremely satisfying and starts to give the learner an understanding of how software is created.

You should also start to understand the building blocks of the internet and how they relate to each other; Http, TCP/IP, DNS, SSL, XML, JSON, client side and server side scripting.

Resources:

* [codecademy](http://www.codecademy.com/tracks/projects) 
* Team tree house is also a good reference, although you have to pay for much of it:
	* [treehouse HTML](http://teamtreehouse.com/library/websites/html/introduction) 
	* [treehouse CSS](http://teamtreehouse.com/library/websites/css-foundations-2) 


# Deploy a web page / site to a live environment
With a basic understanding of how to create a web page, the learner is able to create a landing page for their next idea. For friends, family, etc to be directed to it, it needs to be hosted somewhere accessible on the internet. Take a look at the available options; My personal favourite at the moment is Github pages, which lets anyone host 'static' websites for free, on a custom domain (I use octopress to create the static site), Amazon Web Services (AWS) hosts static websites (via S3) and full web stacks (via EC2) very cheaply. There are plenty of other shared hosting solutions to check out that will help you get your site up on the internet.


# Learn JavaScript and jQuery
As soon as you have a static web application up and running you can start making it respond to your users actions; sticking with the "static" site idea, JavaScript allows you to make web pages interactive, but without requiring any additional server components beyond those covered above. Your website serves a JavaScript file in the same way as it would am html page, css file or image, and the JavaScript gets executed in the users browser.

JavaScript has an extremely good ecosystem of libraries to make dynamic pages easily, from jQuery to interact with and manipulate the elements on the web page to libraries that provide a "Backend as a service" for authentication, data storage, analytics, etc that mean you can quickly spin up extremely complex web apps with no server components at all. A good reference for these back end services can be found [here](http://en.wikipedia.org/wiki/Backend_as_a_service) and many of them offer free plans to get you started. MongoHQ is a particular favourite to allow your app to store any data it needs.

Resources:

* [codecademy javascript](http://www.codecademy.com/tracks/javascript) 
* [codecademy jquery](http://www.codecademy.com/tracks/jquery) 

# Join meetups, open source projects and engage in the community
The community of software developers has to be one of, if not the most engaged communities, both on the internet (hardly surprising given these are the people who create the internet) and in person. Whilst you will occasionally come across people that want to obstruct, belittle and generally be a pain in the backside on the whole the community is incredibly supportive to people with a desire to learn, and who have made a bit of effort to answer their own questions before asking for help. A well worded query on google will often give you the answers you need, and when they don't including evidence of what research you've done on your own "I read x, y and z but I still don't understand why it doesn't work the way I expected" in your questions will often lead to more favourable responses.

Discussing things with others, both in-person and online allows the learner to validate and build on their current understanding. The learners understanding of things they think they know will improve considerably when they explain them to others, and the conversations may also highlight issues with their understanding, or expand further into areas that weren't previously understood.

Some tips:

* Join meetups and open source projects, and seek out further opportunities to discuss and to peer review your code and ideas.
* In-person code events, like coding dojos or code battles, allow you to tackle code challenges in a group, extend your knowledge base through working with other people and help you learn how to work in a team.
* Github has fundamentally changed the way the software development community communicates; if you see a project you want to contribute to it's now simple to fork it, change what you want and then contribute it back to the maintainer for inclusion in their project. Github also helps you demonstrate a body of evidence that can help you in your conversations with potential employers.
* Share the code you write and engage in the community : places like stack overflow let you ask, and answer questions. Asking questions helps you further your understanding, answering questions, and the comments you receive, helps you validate and extend your understanding.
* Go to startup events, like Launch48 and Startup weekend, where you have the opportunity to apply your coding skills to a real life business problem. It doesn't matter how far into your programming career you are - these events are always crying out for more programmers and any help is appreciated.

Resources:

* [hackerrank](https://www.hackerrank.com/) 
* [codeeval](https://codeeval.com/) 


# Learn a server side language and framework
The "Backend as a service" providers can provide a lot of generic functionality that your app needs, but most software developers still favour writing their own backends; there are numerous reasons for this, but suffice to say you'll need to learn a technology that runs on servers.

There are so many options here it can be daunting, but for a beginner it can be boiled down to : Large corporations use the .Net and Java Enterprise stacks while startups use lighter-weight web frameworks based on Ruby, Python and JavaScript (JavaScript can run both on the client as discussed, or on the server using Node). Good developers learn multiple languages and frameworks and there's plenty of transferable skills between them, so don't get too hung up on making a decision; maybe do a few tutorials, speak to people in your area about what jobs are available, and jump in and start learning one. Right now my advice would be Ruby, or Node.js, but that regularly changes based on the market.

As you start extending your application to the server, you'll be able to run it locally, but if you used the static website options above you'll need to transfer to something that lets you run a server application so you can share it with people. heroku, nodejitsu, AWS and a number of other providers allow you to host your application for free; heroku is a favourite at present for most open source stacks, but research these and others to find the right solution for you if necessary. Another benefit of Heroku is that you'll start learning another important tool : Git, which at it's most basic level allows you to version your code and if using github, bitbucket or any other "hosted" system allows you to backup your code should the worst occur.

Resources:

* [nodebeginner](http://www.nodebeginner.org/) 
* [learn ruby in a month](http://www.onemonthrails.com/) 
* [codecademy ruby](http://www.codecademy.com/tracks/ruby)
* [codecademy integrate the twitter API](http://www.codecademy.com/tracks/twitter)


# Get some work experience
With a working knowledge of how to build web pages and a backend language, you should get experience working in some different organisations. Reach out to companies via contacts you meet, or via workinstarups.com, enternships and other internship placement schemes. A company taking on interns is looking for people with good programming skills, the motivation and drive to learn the businesses technologies and a good cultural fit in their group.

Include good examples of your work from your Github account in your covering letter when you apply, and call out some of the interesting things they would find in your code, speak positively about your experiences but don't be afraid to use examples of where you found difficulties to show how you overcome challenges.

Every companys working environment is different, and it's important to experience a few so that you can start to identify the things you enjoy and those you don't:

* Different projects use different languages, frameworks, tools, development processes
* On some projects you'll work on one person projects, others in varying sizes of groups of people.
* Sometimes you'll be developing "green field" applications from scratch, others you'll be fixing and improving an existing code base.
* On some projects you'll have very clear requirements at the outset, on others they'll be more open
* On some projects you'll be closely managed, on others you'll be free to manage yourself

It's important at this stage to start learning how to work in a commercial setting; you'll need to hit deadlines, will learn how to track the work you need to do and what you've done, how to work with other stakeholders in a project (the sponsor, customers, other developers, testers, operations, business analysts, etc), how to use Version Control Systems (like GIT) within a wider team.


# Get a grounding in multiple languages and paradigms
One thing universities do quite well, I would consider it to be the most important part of a CompSci degree and that's to expose people to different programming paradigms. In the UK it's often Fortran, Pascal and C or Java but unfortunately this is often a small part of their syllabus.

Currently the two styles of programming that are most widely used are Imperitive/Objected Oriented and Functional Programming, using either dynamic or statically typed languages. 

It's often possible to write both functional and imperative code in a given language, but some are better suited than others and learning one of each combination (statically typed & OO e.g. Java or C#, statically typed FP e.g. Scala, dynamically typed OO e.g. Ruby/Javascript, dynamically typed FP e.g. erlang) would give you a good base to work from.

Assuming you've got a solid understanding of JavaScript and Ruby a good next option would be Java, as it's a widely used strongly typed language. There's also certification available that can help validate your skills to potential employers.

References:

* [the best book for the Java certification scheme](http://www.amazon.co.uk/Head-First-Java-Kathy-Sierra/dp/0596009208/ref=sr_1_1?s=books&ie=UTF8&qid=1370003772&sr=1-1&keywords=head+first+java) 
* [book Java certification exam (worldwide)](http://education.oracle.com/pls/web_prod-plq-dad/db_pages.getpage?page_id=5001&get_params=p_exam_id:1Z0-803&p_org_id=&lang=) 
* [introduction to programming (with Java)](https://www.udacity.com/course/cs046) 
* [free programming books](https://github.com/vhf/free-programming-books/blob/master/free-programming-books.md) 


# Keep learning
The industry will never stop changing; there are always new languages, tools, techniques and 3rd party applications and services that can help you solve your problems easier, reducing the amount of custom code you need to write and maintain and allowing you to focus on the tasks that relate to your projects problems. You need to keep your finger on the pulse and be evaluating these new tools.

The best universities around the world are offering degree level classes online too, often for free. These are a great chance to get that 10-20% of knowledge that you miss if you didn't do a University CompSci degree.

There are loads of other interesting tracks on codecademy and treehouse from there, and loads of other resources on the web. Depending on what interests you you can look at different databases, different clients (Android, iOS, desktop apps for mac or windows, etc).

It's at this point you need to start learning about "patterns"; common ways of designing / organising your code. The "Gang of four" produced [the seminal reference on this](http://en.wikipedia.org/wiki/Design_Patterns) and there are plenty of resources around the web where they've been well reproduced.


# Write lots of code
You've probably realised that this recurs over and over again in my plan. I can't emphasise enough how important it is to actually write code; it doesn't matter if you're writing code completely for fun (solving coding challenges), contributing to startups or open source projects, or creating websites or apps for your parents / friends / neighbours / paying customers - the most important thing you can do as a programmer is hone your craft.

Some tips:

* There are plenty of code challenges online; these come in the form of generic puzzles with a known solution, or potentially challenges without a solutuon sometimes paying prizes; the important thing is they give you the opportunity to excerise the raw skills that you learn and apply them to real problems. Check out code katas, http://projecteuler.net/, https://code.google.com/codejam/, https://www.hackerrank.com/
* Join meetups and open source projects, and seek out further opportunities to discuss and to peer review your code and ideas.
* In-person code events, like coding dojos or code battles, allow you to takle code challenges in a group, extend your knowledge base through working with other people and help you learn how to work in a team.
* Github has fundamentally changed the way the software development community communicates; if you see a project you want to contribute to it's now simple to fork it, change what you want and then contribute it back to the maintainer for inclusion in their project. Github also helps you demonstrate a body of evidence that can help you in your conversations with potential employers.
* Share the code you write and engage in the community : places like stack overflow let you ask, and answer questions. Asking questions helps you further your understanding, answering questions, and the comments you receive, helps you validate and extend your understanding.
* Go to startup events, like Launch48 and Startup weekend, where you have the opportunity to apply your coding skills to a real life business problem. It doesn't matter how far into your programming career you are - these events are always crying out for more programmers and any help is appreciated.


# Wrap up
Following the path above a person with the motivation and drive, and working on the craft of software development full time should be able to get to the point where they could take work experience in 6-12 months and would be more employable than a lot of 3yr CompSci degree graduates. It's also important to consider the costs and the debt most graduates are burdened with.

Because of this I personally believe a Computer Science degree is not the best option for a large proportion of people that want to get into programming. Most software developer roles are not pushing the boundaries of the field. Most software developers are using an existing suite of tools, languages and techniques to solve business problems.

Solving a programming problem is typically a combination of:

* Experience - What similar problems have I solved before. What tools and techniques did I use? How can I improve on that approach?
* Research - Who else has solved a similar problem before. What tools have they created that I can re-purpose? How can I improve on that approach?
* Learning & implementation - How do I apply the selected tools and techniques to the problem?

Current computer science degrees in the UK help a lot on the last part, giving the learner a broader knowledge in that area, but I would argue that the plan detailed above would get a learner more of the specific parts important to most employers (the general purpose techniques). By following the plan above and writing lots of code, the learner will have much better Experience and Research skills, putting them well ahead.

I'm not against university degrees; there are many legitimate reasons to go to University if you want to become a programmer: CompSci degrees and graduates of them are needed as the boundaries of the field do need to be continually pushed, with the results of that filtering down to the mainstream to utilise. Non subject specific and social reasons for going to University; expanding your mental capacity, critical thinking / analysis, getting away from home for the first time, becoming independent, broadening your horizons, finding yourself, not knowing what you want to do with your life, laziness, etc. These are valid, but people shouldn't be afraid to be honest about which of them apply.

Doing a program as I've outlined here on your own, would require discipline and focus, and may be difficult for someone at the A-Level / university age. I've worked with a number of learning establishments on apprenticeship programmes and if the learner can find a suitable one in their area this is a great option. Some things to be aware of when appraising different programs:

* Many college IT apprenticeships focus on the networking and infrastructure side of things; these aren't really suitable for someone who wants to become a programmer.
* It's important to find a programme that loosely follows the above plan, and that uses modern languages in their teaching.
* I've found QA training in the UK to be pretty good - they have apprenticeships based on Java or .Net, and have a massive amount of other courses that you can include as part of the apprenticeship.


## Should I / when is the right time to teach my kids?
I've also been asked about this for younger children, and I have no experience of this, but the articles below should help.

* http://blog.enternships.com/post/53287729415/5-apps-to-trick-your-child-into-becoming-the-next
* http://lifehacker.com/how-and-why-to-teach-your-kids-to-code-510588878

