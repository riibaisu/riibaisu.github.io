+++
title = 'My first experience with Defold'
date = 2026-07-08T09:00:00-07:00
draft = false
tags = ['defold', 'gamedev', 'gamejam']
listIcon = ""
teaser = "tl;dr: I like Defold, and I will use it when I think it is suited for the project or idea I have."
+++

![Defold Logo](https://raw.githubusercontent.com/defold/assets-defold/master/assets-defold/logo_with_text/logo-hor-classic-white.svg)

## What is Defold?

[Defold](https://defold.com/) defines itself as "*a free, powerful, all-in-one game engine for development of 2D and 3D truly cross-platform games.*"

## My Experience

My main engine is Godot. It’s the engine I’ve been trying to make games with for the past few years, watching tutorials and experimenting since 2020. However, it is not a perfect game engine, there's no such thing, and it is natural for me, a not so talented gamedev, to try and search for better tools.

In a GameFromScratch's video, I heard about Defold for the first time and always wanted to make a game with it. The thought of a no-setup cross-platform and open-source (enough) engine that uses a real programming language is attractive. A lot of the other options have few contributors, and lack support for some kind of platform; sometimes it is web, sometimes it is mobile, or maybe one of them is broken because no one is using the tool enough to actually know if it is working after a lot of breaking changes.

Still, every Defold project I tried to make until now started poorly. I gave up on it a few times, because I am too used to the Godot way of thinking. Then, for a game jam, I wanted to make a bitsy game and I realized: *Wait, maybe doing something so simple would be a good opportunity for Defold* and here we are.

### What I like about it

A lot to like.

#### Decent Hot Reload

The iteration speed that a working hot reload gives is amazing. Godot does have hot reload, but it always works weird for me, and I end up just restarting the scene. With Defold, I don't have this problem and can just let the game run while changing scripts and when I'm ready I just trigger the reload.

#### Lua

I'm Brazilian, and that is already a reason for me to like Lua, but when they say you can learn this language in an afternoon, they're right. In a few hours I was already scripting without having to check the syntax and all that. The fact that everything is a table is kind of fun to script with and handle data.

#### Message System

I'm a fan of the observer pattern overall, so I use Godot signals a lot. The problem is, you always have to catch a reference of the emitter so you can receive a signal. I'm not a fan of that. Defold's message pattern is a really smart way to have something similar but easier to use based on the game's hierarchy. This lets me script and test things a lot faster and without having to switch from the code editor to the game editor all the time. I'm not fully used to it but I enjoy the feature.

#### Build Times and Export

This is super important to me. Having to wait MINUTES for a game to build is maddening; Unity devs know that. Gladly, Defold has super fast build times for occasions when hot reload won't work in the feature you're testing. And the sizes are super small too.

I like making games, but I hate exporting them. Anyone who participated in a jam knows the feeling of working in a game, rushing because you have little time left and when you're ready to export, the editor says you have to install some things or says certain feature you're using is not supported in the platform you're exporting to. I hate that. Defold doesn't seem to have that problem, which is amazing.

#### Documentation

It is one of the best documentations for game engines I have ever used. It is beautiful, clean, has examples and it is detailed. Where to start? Check the manuals. Still have doubts? Just look at the API. It makes the process of learning and discovering the engine a joy.

#### Collection Proxies

Okay, this one I wasn't expecting to like. Collection is basically a prefab, and a collection proxy is a way to instantiate a prefab when it is actually ready to spawn in the game world. This was fun to work with to make the transitions between the screens. In Godot the scene transition isn't quite optimized unless you make a system on top of it.

### What I didn't like

Mostly solvable with best practices.

#### I dislike Strings everywhere

When scripting in Defold, you have to use a lot of strings. Ids, urls, hashes and so on. Strings are a nightmare to reference and debug. One typo and your code doesn't work and you don't know why and keep trying different things because the compiler trusts you so it keeps its mouth shut about the fact that the object id you're referencing to doesn't exist.

##### Also Lua

Lua is a good thing and a bad thing. The lack of types creates this string problem, and you will also need to build a lot of things some other languages and game engines have built-in. I think it is one of the reasons Defold is almost a *pseudo-game engine*. Has too much stuff to be a game framework and too little to be the game engine for everyone.

#### Quality of life features

Don't get me wrong, the editor is nice and beautiful, but it lacks a lot of quality of life features that I got used from the Godot Editor. What do you mean I can’t drag a game object from the hierarchy into a file field and have the editor create the reference for me? That happened a lot, "*the editor will handle this for me*" and actually does nothing and wants you to setup a basic component.

## Conclusion

Defold is not for everyone, and is not for every project either. If you just want to make a game, have a specific platform in mind, and want to have it as fast as possible, you probably are better with Godot or Unity. But I think its benefits compound over time: **the more you build with it, the faster your next game will come out** and you will reap the small sized build, fully cross platform benefits.

The fact that it is so clean and clearly well thought makes me want to use it more for my next projects, when I feel like coding and want to post a game literally everywhere. But certainly with longer deadlines.
