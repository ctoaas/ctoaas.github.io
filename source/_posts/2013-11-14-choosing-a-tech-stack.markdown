---
layout: post
title: "Building a delivery team Part 1 - Choosing a tech stack"
date: 2013-11-14 07:48
comments: true
published: true
categories: 
---

One of the most satisfying parts of my roles has been creating technical delivery teams; these are the engine room of a tech business. You often hear about a "10x" increase in productivity between an average developer and a "rock star" developer, but for me that pales into comparison compared to the differences created by the interactions between members of a team and the environment they work in.

This is the first of a multi-part series of posts on building a delivery team and will also include hiring, team composition, tools and processes.

# Caveats

There are plenty of businesses where technology isn't important, where software is used, perhaps with a bit of customisation, or a business that has a website solely for marketing. Those businesses can probably ignore most of this; these articles are addressed at businesses who at their core require the creation and maintenance of software assets.

These articles are also focused on the early start-up phase of these types of organisations, where typically a single product is being built by a delivery team of less than 20. There are changes that need to be made on the way to this size, but as it grows beyond 20, and significantly more people on the business side this model will start to fall down and additional orchestration and communications channels will be needed.

# Our industry

There's a tendency within the industry to polarise; to pick a technology that one likes and propose it as the panacea solution to everything, with every other technology being rubbish. I believe a lot of this is due to a fear of the unknown, and wanting to increase the value of ones current skillsets, a classic case of "if all you have is a hammer, everything looks like a nail".

An often misunderstood debate is open source v proprietary; a lot of people believe that open source has become prevalent because it doesn't cost any money, when proprietary software from the likes of Microsoft requires you to purchase licences.

Whilst this may be true for businesses at the seed stage, for a technology business where the operation of technology is the business it's often deemed too risky to run this technology without professional support, and normally this professional support costs as much as a software licence.

The prevalence of open source is more down to the ability to participate in the community; to contribute to a products direction, fork it, patch it, help test it, etc; this is great if people are going to contribute, but most of the time that's simply not the case - most people are consumers of, rather than contributors to open source projects.

I often see businesses make a call on technology stacks because they're "open source and free", with little intention of contributing to the projects and not understanding the professional support that will be needed as they grow. This feels wrong to me.

# Choosing a stack

This article is going to be focused on the building of a modern web application; that is a series of backend services providing an API, which is consumed by a front end application and mobile apps.

When thinking about which technologies to use there are a number of facets to consider:

* Initial cost of tools / IDE : Whilst a lot of developers will use only a text editor, many still prefer facilities like code completion, intellisense, integrated debugging and refactoring that an IDE can provide. I've based this on the most popular tools I've seen and read about people using, that's not to say there aren't alternatives that are cheaper or more expensive for each case.

* Ongoing cost of tools	: This weighs heavily against the Microsoft crowd, who whilst they have great tools that are free for the first few years on Bizspark, they have per-seat developer licensing when you leave that program.

* Availability of developers : How many developers are available in the area I'm hiring in; this is a combination of the skills prevalence on Linkedin and my personal experience.

* Cost of junior developers / Cost of mid range developers : what are the market rates for developers in the area I'm hiring

* Availability of important functions / frameworks : I've seen startups create needing to create database drivers to connect their chosen stack to their database of choice; this contributes little to a startup providing their product / model, so should be avoided.

* Likelihood to be popular in 3 years : Is it going to be kept up to date with modern tools and processes. Are you still going to be able to find developers? Will people still want to work with it?

* Language / Framework learning time : Most professional developers have a good knowledge of OO & procedural code, like C# or Java, switching between these and other similar languages is relatively straightforward. Switching to a functional programming  paradigm in Scala is more difficult.

* Cool factor	: good developers want to work with cool modern tech.

* Language maintainability : the verbosity of the code you write, the amount of boiler plate code you need to implement and type safety affect the maintainability of the codebase that is produced.

* Suitability for concurrent systems : multi-threading, shared, mutable state and traditional process models are one of the major contributors to running stable highly concurrent applications. Immutability, 

* Existing large reference sites : Are there good examples of large organisations using it for core / critical functions, and contributing to the eco-system.

* Production / Hosting options : The hosting options for most of the major frameworks have started to converge on IaaS, PaaS or shared / self hosting. For newer technologies the deployment and PaaS offerings may not be so mature.

* Skills available from existing developer relationships : Do I know and trust people with the skills already that are available and can help us get things moving quickly without the recruiting risk.

* Architectural control : I want a consistent approach to application architecture, and have largely settled on MVC; whilst it's possible to attempt to enforce other patterns on top of a chosen framework (like MVP on top of WebForms) but this is often not done well.

* Maturity : How long has the tech been around?

* Ease of setting up automation (CI, deployment) : newer technologies may not have patterns for this yet	

* Interoperable with system X	: the application being appraised may need to integrate with a specific database or other legacy API. Unless you want to be writing low level drivers you 

NB. I've considered the developer related attributes outside London, as at the moment I'm not up to date on the London market. I'll update it later this year (I'm hiring at the moment, if interested drop me a line!)

# Results

I've modelled these options in a spreadsheet that can be downloaded [here](/assets/files/DevStackAppraisal.xlsx). The first version of this spreadsheet was a couple of years old, and a lot of the technologies I was considering then, and am considering now have matured and have similar scores, technologies that are becoming more popular now, like Go, or other tools you're considering, could show more of a variation.

# Choosing a stack for the client apps

The time of the pure JavaScript client apps has definitely come. With the speed and maturity of mobile browsers, and obsoletion of IE8 for most cases developers are free to create rich client interfaces in the browser, calling backend services for data and binding it on the front end.

Tools like Angular, Knockabout, Ember provide the patterns and plumbing to create modular, testable client-side applications. The biggest concerns with the single page style applications created with these frameworks are around deep-linking and SEO.

Tools like rendr take this a step further and run the same backbone application on the client and server, so that these issues are removed; if the server receives a request for a deep link within the application it processes it on the server and renders the page correctly.

For mobile it's still very much about native apps for each platform you want to support; tools like phonegap that allow you to develop cross-platform are great in principle, but often result in apps developed to the lowest common denominator, and the experience on all platforms suffered.

LinkedIn and Facebooks apps, amongst others, use a hybrid approach of native functionality and HTML5 delivered from the server, attempting to get the best of both; a native feeling experience while being able to update on the fly and re-use functionality between platforms - expect to see if these technologies are open sourced as they mature.