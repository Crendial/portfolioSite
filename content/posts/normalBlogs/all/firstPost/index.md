---
title: My first post
date: 2026-11-19
subject: Normal post
topic: All
weight: 10
tags:
  - Hugo
  - Learning
summary: Something about setting up this very site!
---
# Why make this site?
I'm currently in my month long internship in Italy. Got the idea of a portfolio site suggested to me, which came with the benefits of trying/using Hugo. This internship has already taught me a plethora of tools from scratch (Django, Tailwind, lazyvim) so why not put another on the pile? Sure it won't be the deepest learning experience ever, templates make that nearly unnecessary, but getting the basic ideas down and adding the toolkit to my Nix configs could go a long way in the future.

# The process

## Finding a suitable template
I'm sure there are plenty of templates out there on Github but going out there is like dumpster diving. Yeah you CAN find something valuable but trash is always trash. So I decided to settle with just looking through the more official theme search tool. 

Turns out most of them are AWFUL for what I'm looking for. Either they change too little or change it in a boring direction or one I don't want at all. It was a STRUGGLE. Did end up on stumbling on the current template you see around this site. It's clean, gives the info about me concise and clean. Massive fan. Then I opened the documentation. There is a separate setup guide! Which is a good and a bad thing. Good because I get a working site faster and easier, bad because I learn less and could stumble into unique walls.

Thankfully that was not the case and I was happy to move on.

## Learning Hugo basics
Was not that bad, just plopped Go and Hugo into my Nix configs. Rebuilt and read the basic tutorial to start a project. Turns out said tutorial barely teaches you anything. That's fine, I have an example and installation docs from the template! 

I have never used this much '.yaml' in my life. Kinda cool, I like it, basically JSON but more readable in a way. Used the templates example sites data folder to modify and implement the features I wanted, had to make an index page and .gitignore, basic stuff really. Had the base site up and running relatively fast thanks to the node.js wrapper for Hugo commands that comes with the template.

## Folder structure pain
Each markdown file usually apparently has a subject and a topic for sorting reasons, "that's cool! Probably won't use it though" I thought. Until there was an element in the template that required both. I don't like it. I wish it was more dynamic, it was a struggle. But I got it working, I made it clear to me personally, it's cool.

## Modifying a part of the template
I LOVE the featured project cards. They're clean, they work well, except for the fact that they are not clickable by default. Had to pull the html for the cards from the template, put it in my own layouts and change it to take a post url. No big deal but should be mentioned

# The result
Look around!
