Open Source Project Outline Template
====

This is a proof of concept for a method to provide general project outlines using [YAML](https://en.wikipedia.org/wiki/YAML) and [Markdown](https://en.wikipedia.org/wiki/Markdown) in a single text file.

## Problem and solution

Projects exist in all kinds of formats documented on the Internet. I want a way to look at a project and get a general snapshot of what a project is, what skills it requires of me, and what I can expect from it.

I don't want to create another web application to store this info in a database. I don't want to go to some walled garden to see projects.

The method within this repo provides an example of how one could document a project in a file much like software's standard README. Structured data is placed in a YAML header while free form data is written in Markdown.

## Background

This project was inspired by a drawing by [@jphoenix24](https://twitter.com/jphoenix24) from the [Open Source Hardward Documentation Jam](http://www.opensourcewarehouse.org/) on April 27, 2013 seen in [this tweet](https://twitter.com/aishyza/status/328200749999869953/photo/1)

# What's going on here

This is a basic starter template for Github pages. Just fork the code and run it as a github pages. You can see an example of this project at [dhornbein.github.io/project-outline](//dhornbein.github.io/project-outline)

## The project file

`test_project.md` is our example project. It provides a human readable file that gives a bunch of info about the project.

```
---
layout: project

title: Test Project
links:
 - name: Project Github Repo
   href: "//github.com/dhornbein/project-outline"
 - name: Drew's Twitter
   href: "//twitter.com/hornbein"
 - name: Drew's Blog
   href: "//blog.dhornbein.com"
image: "//placekitten.com/300/300"
author:
 name: Drew Hornbein
 link: "//dhornbein.com"
 social:
hashtag: oshwdocjam
date: 2013.04.25
ratings:
 - name: cost
   level: .4
   note: "The cost really depends on factors that this sentence would describe"
 - name: difficulty
   level: .2
 - name: assembly time
   level: .6
 - name: durability
   level: .8
 - name: scalability 
   level: .3
skills:
 - name: AutoCAD
   level: .5
 - name: Soldering
   level: .2
 - name: Schematic Capture
   level: .8
---

## Free Form Project Documentation

This area is the perfect place to write README style documentation.

There can be lists:
* That have points
* In a formate, much like a list
* A list of items
```

That's all. Just some YAML at the top and MarkDown underneath.