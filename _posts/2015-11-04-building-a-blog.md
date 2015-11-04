---
title: Building a Jekyll blog (part 1)
layout: post
---

I'll use this as an opportunity to explain how I built this blog.

As you can see in the About section in the sidebar, this blog was built with a content management system called Jekyll.
It is a very powerful but simple tool.
The idea is to create the content of the site in a readble way, and then generate a proper website from it.

<!--jump-->

Ok! Let's get started! First we need to install Jekyll.
There are several ways: you could install it via the ruby package `gem install jekyll`,
or you could use some other package manager, like `yaourt -S ruby-jekyll` on Arch Linux.

Got it? Great! Now we create something!

Normally you'd run `jekyll new <path>` to create a project skeleton at `<path>`. But to get a running start, we'll employ something else.
Navigate to [this repository](https://github.com/poole/hyde). 
This is a ready theme for Jekyll, giving us a lot for free.

We simply clone the repository

``` bash
mkdir blog
git clone git@github.com:poole/hyde.git blog
cd blog
```

If we run `jekyll serve` (or `jekyll s`), we'll get the site served at `localhost:4000`.
If we visit it with a browser, it looks something like

![Screenshot of Hyde](/assets/hyde.jpg)

Nice! That's it for this part, but stay tuned for the next!

Take a look in the `_posts` folder, and try to modify them. See what the console says, and what happens when you refresh the browser!
