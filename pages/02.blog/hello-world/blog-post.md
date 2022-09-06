---
title: 'Hello World'
content:
    pagination: true
taxonomy:
    category:
        - Blog
    tag:
        - Misc.
---

**This website has been 4 years in the making. A long 4 years filled with dead ends and procrastination. And because it took me 4 years, I think it gives me free license to use up some of your time if you do choose to read further.**

### [WordPress absolutely sucks](https://hackernoon.com/this-is-why-wordpress-sucks-and-you-should-probably-stop-using-it-v697y30v7)
For some reason, even with all the one click install solutions, auto-management plugins which add bloatware, one thing never changes.

**WordPress just sucks**.

Things are constantly breaking, the one theme you like is either out of date or they now want money or they'll hide the best features of the theme that made you like it in the first place.

WordPress is also, at it's core, a blogging platform. Try to do anything even slightly different, and you'll run into problem after problem. It's like trying to fight the government for their archaic laws; there's no winning.

So obviously, I wanted to be able to switch out of WordPress. The only requirements that I had for myself were:
* The website should act as a short portfolio
* The website should house a simple blogging interface.

### I'm the smartest man in the world.
The hubris of a programmer knows no bounds.

Around this time I was looking at some c# code which would parse [html](https://en.wikipedia.org/wiki/HTML) and construct a website based on the html being presented to it, and I thought _"Wouldn't it be great if I could write something so that I could just host my website content as plain text, and a converter would make nice HTML pages out of it?"_

If you have ANYTHING to do with web development (I don't) you'll realise that all this has been already invented quite a few years ago and I was just feeling like a genius a decade too late.

Anyway, this led me to two different solutions for my new website, things which do precisely what I was thinking of above (again, in a much better way than I could have ever written it).
1. [A static site generator](https://www.cloudflare.com/learning/performance/static-site-generator/), which allows me to keep all of my website content local, and just compiles everything down to html which can then be uploaded and updated every time I need to make a change to the website. SSGs are really popular, and you can find frameworks and website themes for everything from landing pages to beautiful blog and portfolio sites.
2. [A flat-file CMS](https://freelancewritingpros.com/flat-file-cms/), which, while can be used to generate static sites, is best suited for content management without a database (i.e. all your content is plain text and easy to sync and back up). Flat-file CMS options are definitely less popular than SSGs and have less community support, but they allow you to do more interesting things with your site. And you don't have to recompile your entire website every time you want to update some content.

With all this knowledge, I first tried my hand at a static site generator (I used one called [Hugo](https://gohugo.io/)), and IMMEDIATELY hated it. Don't get me wrong, I got a really good looking website out of it, but compiling HTML every time I have to correct a grammatical error?! COME ON MAN. Nobody has time for that shit.

So because I'm not an absolute Neanderthal, I chose to try out [Grav](https://getgrav.org/), a flat-file CMS. I loved (still do) Grav. The amount of stuff you can do with a flat file CMS is incredible.

### Always do things the hard way, even if easier solutions exist
The thing is, Grav is amazing for creating simple sites with a lot of static and some dynamic content. And most themes you find for it reflect that. I had to find a theme I liked not just for the landing page, but something that would work well for putting up blog posts. Maybe not to the degree of a full blog site, but something that I could call my own. The only thing that I found that fit the bill was [Webfolio](https://github.com/jasonccox/grav-theme-webfolio), and I decided to use it.

... but I wasn't super happy with the blog page, and the fact that it had no links to other posts, and no tags. And I didn't quite like how it looked either, but it had all the functionality I wanted.

So.

I decided that I was going to learn the basics of html, twig, CSS and the Grav framework to edit the theme, add support for a few plugins that would make adding a sidebar on blog posts and possibly comments in the future. I didn't even know that something like [Sass](https://sass-lang.com/dart-sass) existed before this. And this theme uses Sass EXTENSIVELY. Shit's wild man.

### In Finé
I've given up on this website THREE SEPARATE TIMES since I decided on Grav. I was just not able to get shit working. In the interim, I had a weird hacky solution where my website would go to a Grav landing page, but the `Blog` link would redirect to a _🤢🤢WordPress blog🤢🤢_. At that point my blog was clearly only up for the sake of completeness (sentimentality maybe?), because I never put up a post on it since probably 2015. Why bother, since I was gonna be taking it offline anyway? But I never did.

Then a couple of months ago, WordPress did as WordPress does, and my blog just stopped working. All the content is in there, but there's some errors on the site. That was the kick to my ass that I needed to just finish this blog part of the Grav site, no matter what.

I feel I have finally reached that goal and my [old blog](https://archive.aashishvasudevan.com) can finally be retired.
(Don't actually click that link, it doesn't really work.)

I have published [my fork of the Webfolio theme on GitHub](https://github.com/aashishvasu/grav-theme-webfolio), and I hope that whoever finds themselves in a similar situation to me (all 3 of you out there), this post at least points you in the right direction.