---
layout: post
date-published: 2015-04-10
title: Formal Methods at Amazon
uuid: 915cc2e8-d190-4d54-b746-0e1c34dff835
---

I saw this paper being mentioned again and again in my Twitter
feed. Basically not even knowing what "formal methods" really means I
was intrigued by the claim that it's easy to read. And it has been.

The paper describes how Amazon used a specification language to
describe designs of complex concurrent fault tolerant systems finding
bugs and verifying changes in the process.

The specification language (TLA+) is not focus of the paper, rather
the authors concentrate on describing benefits, problems and the path
of adopting formal specification of system designs in an engineering
organization.

TLA+, stands for *Temporal Logic of Actions* and ["is especially well
suited for writing high-level specifications of concurrent and
distributed systems."][tla-intro]

Reading how they use it at Amazon I'm under the impression that it
works very similar to [generative testing] dumping a ton of basically
random (according to some rules) data into a system and checking if
the desired properties are maintained. Often the term *"model
checker"* is used.

Download the [original paper] or a copy of it [with some passages highlighted][highlights]
that I found particulary interesting.

[tla-intro]: http://research.microsoft.com/en-us/um/people/lamport/tla/tla-intro.html
[generative testing]: http://blog.8thlight.com/connor-mendenhall/2013/10/31/check-your-work.html
[original paper]: http://research.microsoft.com/en-us/um/people/lamport/tla/amazon.html
[highlights]: /images/formal-methods-amazon.pdf
