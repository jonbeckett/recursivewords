---
title: Unfathomable
date: 2019-04-29
categories: [life]
tags: [life]
author: Jonathan Beckett
---

After a self-imposed seclusion from the internet for the majority of today - while attempting to shield myself from any and all spoilers about Game of Thrones - it's finally safe to re-appear. We just finished watching it. I'm not going to write anything about it though, because the internet seems to be awash with it.

Why does everybody need to publish their opinion about something at the same time that everybody else is publishing their opinion? Surely after the first few voices speak up it all just becomes noise? Sometimes the behaviour of people on the internet reminds me of a saying I once heard - "it's better to be on the train, pissing out the window, than on the platform, trying to piss in".

Anyway.

I've been busy building software again - working on the hidden under-pinnings of the giant project I'm working on in the evenings. I suppose in laymans terms you might say I'm building the insides of the engine of a car - which will be covered with several layers of other stuff before the user interface is plastered on top. I sometimes wonder how much people really understand about what goes on when you use a web browser.

This might be fun.

You know when you're typing into a new blog post at WordPress? You're actually interacting with a piece of client-side software written in JavaScript that's running within the browser to "look" like a word processor. Of course browsers are not word processors - they don't even have scalable typefaces - it's all smoke and mirrors. Every keypress causes code to run that draws a curvy shape onto the screen - the characters of the font you so carefully chose for your blog design. Behind the scenes, the actual words are also being recorded as HTML - simultaneously rendered in front of your eyes with a blinking line to look like a cursor - so it looks like you're typing the characters onto the screen. You're not.

All of this happens inside the browser's artificial brain - holding the whole thing in short term memory. In WordPress case, while you're typing yet more code runs periodically to communicate with the server - sending messages back and forth - saving what you have done so far. It does this silently for the most part.

The browser packages up each message to the server as a stream of characters - which are then sent to the networking part of the operating system with a destination address, and a reminder to let it know when each message has been successfully received.

The networking part of the operating system is really rather clever (or at least, I think so). It splits messages up into small chunks - "packets". Each packet is sealed in a series of envelopes - each describing the place they need to go - the outer-most one addressed to the network, the next to a given computer, the next to a specific piece of software running on that computer, and so on. It's worth pointing out that I'm generalising A LOT. Some networking professional will no doubt point out that I've missed this or that - and I won't argue - I missed it on purpose.

So what happens once the pile of envelopes leaves your computer? It arrives at whichever switch your house is connected to on the internet, and a game of hot potato starts - which the internet is really good at - with each point of the network throwing millions of packets in all directions at once - each point of the network looking at each packet, checking a database of destinations, and sending them on. If an address is unknown, or a packet is lost, the system is self-healing to a certain extent - the packets can reach their destination in any order, and are re-assembled at the final destination. The "received your message OK" only goes back if the destination server knows it has all the pieces that were originally sent.

Once the WordPress servers receive your message (for this example at least), they are interpreted by the operating system on the server, given to the appropriate software application that deals with whatever the content was (web traffic goes to the web server, for example), and then other services might be programmed to get involved too - saving your words into a database for example. The server itself is simultaneously receiving requests from other people to READ your words - so the whole thing happens again in reverse for every person reading - they send a message asking for a page - which flies across the internet, arrives at the server and is processed - then the server constructs the page, and sends it back to each requester's computer - flying back across the internet, being deconstructed by the operating system, handed to the browser to be interpreted, and turned back into a blog post within the browser window. 

Think about that. Think about all the processing that goes on simultaneously all over the world - the millions of websites, millions of people looking at them, and billions of packets of information flying this way and that. And we complain when it takes more than a second or two for a page to appear in a browser.

I often laugh quietly to myself when I hear anybody say "my internet isn't working". It's not "their internet". It's nobody's internet. Nobody is really in control of it any more - it was designed to survive disruption. And yes, this is a huge headache for the world to deal with. People joke about the monolithic company in Terminator, and the "rise of the machines" - in many ways it happened thirty years ago - when the first true packet switching nodes on the internet connected to each other.