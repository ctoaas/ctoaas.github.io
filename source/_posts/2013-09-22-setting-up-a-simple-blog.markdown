---
layout: post
title: "Setting up a simple blog"
date: 2013-09-22 21:01
comments: true
categories: 
---
As part of a new business I'm setting up, I wanted to get a simple blog system online. In the past I've used Wordpress, and although I hate PHP have never found anything that made sense as an alternative.

For me the criteria for an alternative were :
- Written in a language platform I was interested in - this is pretty much any common, current web stack, except PHP.
- Feature rich with the ability to extend it, an abundence of extensions and an active community.
- Has a straightforward and cheap cloud deployment mechanism.

But thinking about it again recently I'm more interested in:
- Has a straightforward and cheap cloud deployment mechanism.
- Very little maintenance requirement - a static deployment to S3 would be perfect
- Allowing the post content to be edited locally in text files, in an open format
- Have a number of themes available, so that I only need to pick one and write some content and off I go
- This is less of a priority but I'm using node JS on a project I'm working on at the moment, which I'm new to, so any coding (extensions, templates, etc) being in Javascript would be ideal

This led me towards Blacksmith, https://github.com/flatiron/blacksmith, using an S3 static website for the hosting. I was pretty close to moving forward with this, but couldn't find much in the way of themes. I've now settled (I think) on Octopress, and probably github pages for the hosting. I have a basic understanding of Ruby, and haven't used it in anger - but I assume I'll be able to pick it up should I need to.

I'll now document the install process from my Mac.

I started by following these articles:
	http://miguelcamba.com/blog/2013/04/22/tutorial-create-a-blog-with-octopress-and-host-it-in-github-pages/

The first issue I received was when running rake deploy, which returned this error:
	"You have already activated rake 10.1.0, but your Gemfile requires rake 0.9.2.2. Using bundle exec may solve this."

Running "bundle exec rake install" fixed this.

The same went for the next few bundle commands, resolved using:
	bundle exec rake setup_github_pages
	bundle exec rake deploy

When running this deployment task I received the error:

	## Pushing generated _deploy website
	To -- removed for security --
	 ! [rejected]        master -> master (non-fast-forward)
	error: failed to push some refs to '-- removed for security --'
	hint: Updates were rejected because the tip of your current branch is behind
	hint: its remote counterpart. Merge the remote changes (e.g. 'git pull')
	hint: before pushing again.

One tip - when creating the repo in github, don't specify a git ignore or a licence and this issue seems to be avoided. I did find a solution to this on stack overflow : http://stackoverflow.com/questions/17609453/rake-gen-deploy-rejected-in-octopress

	Edit the Rakefile and look for this line:

	system "git push origin #{deploy_branch}"
	Alter the line by adding a plus (+) before the #{deploy_branch} tag:

	system "git push origin +#{deploy_branch}"

