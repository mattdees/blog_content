Title: Why Static Generated Websites?
Slug: why-static-generated-websites
Date: 2014-02-10 22:57:56
Tags: hosting, future, tech, rant
Category: hosting
Author: Matt
Lang: en
Summary: Static Generated Sites!

One of the latest trends in the web tech scene is static site generation. Calling this a _recent_ trend isn't fair at all to old great static website generators like NewsPro that I was using to generate markup for sites in the late 90s.

There are quite a few articles out there discussing the *what* of static site generators, giving quick break downs of software like [jekyll](http://jekyllrb.com/) or [pelican](http://blog.getpelican.com/).  This article is going to focus on the *why* of static site generators.  So, pose the question *why* are static site generators a good solution for modern websites?

## Security!

If you work in the hosting industry, or perhaps even pay attention to the hosting industry, you're probably well aware of the various security concerns that the various blogging software, CMSes and forums all cause. The #1 source of exploits on any shared hosting platform is caused by out of date user software. There are steps that a host can take to avoid exploitation, such as mod_security, virtual environments and other mitigation techniques. At the end of the day, if an attacker can get your client's software to execute arbitrary code, you will eventually have to deal with it.

Static site generation works around this by generating raw HTML & CSS based off of a template and publishing it to a directory. This means that with a static generated site - one's website is not as open to attacks.

## Speed

One of the biggest sources of server-side slowdowns for websites is the reliance on mysql & having to perform multiple complex queries when rendering a page.  With a static generated site, the page is pre-rendered therefor no need for server-side processing or queries. An added side effect of this is that websites become easier to distribute via a CDN or to multiple locations as there is no need for complicated multi-tiered mysql setups.

## Simplicity (in a unix kinda way)

This blog post was written in markdown, from my editor of choice (sublime text).  This means that I wrote this blog post without the help of a web interface. As someone who is more at home using a bash terminal than a file browser, this is a *big* advantage.