---
title: "Introducing Semester Scheduler"
tags: 
- Personal project
- Semester scheduler
date: 2024-02-19T11:32:56-05:00
draft: true
---
## It's Been a While
I started this site as a project over mid-term break last summer and then promptly forgot/didn't have time for it. Since then I've finished my first year of programming classes and have started my co-op workterms and while that's given me invaluable experience with coding in a professional setting I have been ignoring working on personal projects. 

I've kind of been bouncing around between Advent of Code, LeetCode, and Project Euler for getting my "reps" in, but they're one-off coding prompts which don't give me any experience in working on an actual project for myself. What I wanted was something a little bigger that I could chip away at and continually improve that solves a problem for myself and is just more useful than "find the largest common prefix of these words" or something like that. It's the same as the difference between cranking through math problems, and actually using math to solve a problem. 

## Enter the Semester Scheduler
In the first week of every semester I've found it useful to create a "Semester Schedule" which is a one-stop-shop for every due date, submission deadline and test for the next four months. 

![Last summer's schedule](/images/term-3-schedule.png)

Each row represents a week, and each column is for a course. On this one sheet I can see what's due this week, what's coming up in the next few weeks, and what the most important items are. It's been really helpful in planning my reading and studying, and what to prioritize. 

## The Project
Since I've been making these as Excel sheets, I thought creating a program to automate this would be a nice little project; it's useful to me, it's straight forward, and it should expose me to some new concepts. 

I really over complicated things and made this _way_ more difficult than it needed to be. Consequently, I gave up and put this on the backburner several times in the last few months and it's just kind of been nagging me in the back of my mind as something I _can_ do but haven't. 

So, I've rethought my approach to this and am just going to nuke what I have so far (which isn't much) and start fresh. I'm going simple to start: just read in a YAML of my schedule and output a formatted PDF. That's it. Future tasks will be to give it a GUI, do some error processing, and allow for interactive chagnes, but for now I'm just going to have a black box that takes in one thing and spits out another - no more, no less. 

## My Goals
Honestly, just finishing this before the summer semester starts is a big one, but this should also give me some experience building an actual application for myself. Most of what we've done in school have been labs or small assignments - nothing much more than a few hours of work, and pretty rigidly defined. Most of what I've done at work has been working on huge existing code bases. This should land somewhere in between - something I can start from scratch, plan out on my own, and build as a stand alone app. It's the first time I've really tried build tools and bringing in outside dependencies on my own, so that should be an experience. 