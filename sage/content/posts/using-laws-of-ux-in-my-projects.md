---
date: '2024-12-27T12:26:44+05:30'
draft: false
title: 'Using Laws of UX in My Experience'
tags: ['ui/ux']
categories: ['cs']
showtoc: true
cover:
    image: cover/abc.png
    alt: 'What da hell?'
---


You can check the all the laws of UX [here](https://lawsofux.com/).

I've followed these practices for a while now.
## Aesthetic-Usability Effect
Users often perceive aesthetically pleasing design as design that’s more usable.

*It is for this reason that I tend to use **Tailwind** for all my projects.*

The mobile first approach not only makes the apps responsive without much trouble (that's the secondary benefit), it actually ensures that all the components are aesthetically pleasing to mobile users and not just a bunch of divs forced to fit into the mobile screen.

## Doherty Threshold
Productivity soars when a computer and its users interact at a pace (<400ms) that ensures that neither has to wait on the other.

This is the most obvious one of them all. Your APIs should (and I make this my ground rule) not take more than 500ms to respond. Beyond that, if B2C product, you might have just lost a potential customer's attention.

Even if you're B2B product, sub-second APIs tend to give a better customer experience.

That being said, it isn't always possible to improve API performance, maybe you're stuck with an old framework or you have self hosted the backend.

In such a case, you can do these things:
- Add an animation while they wait for the API to resolve (not a plain progress bar or spinner).
- Turn the API into a stream or paginate the response
- Add a caching layer like [redis](https://redis.io/).
