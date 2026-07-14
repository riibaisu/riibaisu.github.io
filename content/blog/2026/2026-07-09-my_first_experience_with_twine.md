+++
title = 'My First Experience with Twine'
date = 2026-07-09T19:48:37-03:00
draft = false
tags = ['twine', 'gamedev', 'game jam', 'game engine']
listIcon = "/ph--gear-fill.svg"
teaser = "tl;dr: Good for its purpose, writing text-focused interactive stories. Would use it again in writing or planning games or for tight game jam deadlines."
+++

tldr: Good for its purpose, writing text-focused interactive stories. Would use it again in writing or planning games or for tight game jam deadlines.

## What is Twine?

In its website, Twine is defined as "*an open-source tool for telling interactive, nonlinear stories*". I like to think about it as a branching dialog game creator.

## My Experience

After finishing the [[Customer Cat Postmortem|last game jam]], I was eager to participate in another one, but I only had 8 hours to submit something. With my current skill set, I knew I couldn't make a polished graphical game in that time, so I decided to write an interactive story instead. It's a game after all, right?
### The Good

It is straightforward to use and start creating a story and the branching paths. Besides that, you can structure your story however you want, make a choice based game or a linear one; you're in control of how it works. 

Writing was the easiest part, I simply typed and I had a functional text game in an hour or so. And the editor lets me see how my planning is structured and where I should put more effort into.

### The Downsides

Everything outside of writing text is not so clear. The documentation is not easy to navigate and there are talks about plugins, story formats and all that when I just want to play a sound or insert an image. Basically, to make anything else, I had to browse reddit answers and keep trying their code.

Yes, I know, Twine scripting is basically [[HTML]], [[CSS]] e [[JavaScript]]. Even so, why can't I preview the images I want to put in my game? I have to export the game to .html file, create a folder and put the images in it, and I still can't see the images inside the editor itself!

#### Audio

To play audio like music, sfx or ambience, you need a plugin. And to install that plugin you have to insert a huge .js and .css file in your project and even then you can't just activate it, you have to create an invisible special path for it to work. Furthermore, there's a lot of "um, actually" things to work on still. I just wanted to play some music…

## Conclusion

It is a good tool for interactive stories; you can have something working in 10 minutes and make something fun with it. But I expected more ease of use and established practices (don't get me wrong, the software is amazing). I would only use for tight game jam deadlines or strictly text-focused ideas, though; for something more elaborate, I would prefer [[Ren'Py]].