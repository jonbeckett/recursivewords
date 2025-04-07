---
title: Hours And Hours
date: 2017-07-25
categories: [life]
tags: [life]
author: Jonathan Beckett
---

A support call came in late yesterday - reporting that something didn't appear to be working correctly on a client site. It got assigned to me. Everything gets assigned to me at the moment, on account of me having the most flame retardant underpants, it seems. The project involved wasn't written by me (they never are), and the original developer no longer works here (thank f*ck). I promised to look into it first thing this morning. While I said "first thing", I actually meant "when I get around to it" - and because of the curiously stupid kind of person I am, that really was first thing, and I then spent FIVE HOURS looking into it.

Looking at other people's programming is interesting - and by "interesting", I really mean "horrifying". I'm not going to get all lofty and long haired lecturer about it - let's just say it wasn't good in a "I didn't write it, therefore it is rubbish" kind of way. I ended up re-building the client system from scratch inside a virtual machine to replicate the problem - and I *did *replicate it - but evidently not caused by the same root cause, because when I triumphantly announced I had solved it, the client quietly emailed me back with words to the effect of "erm. Nope."

Another hour later I finally stumbled upon the cause of ALL of it.

It transpired that somebody had been fiddling. A setting had been changed deep in the innards of the system the software was installed on, which caused it to go spectacularly, and silently wrong. Nobody could have guessed of course that flicking a certain switch would have caused everything to start misbehaving - much like nobody has ever understood why a certain light switch in our kitchen causes the fuse box to trip.

Now please excuse me while I go and headbutt a wall somewhere for a while.