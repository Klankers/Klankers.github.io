---
layout: post
title: "My First Blog Post"
date: 2024-08-12
categories: blog
---
Here it is! The website is finally live.

I've wanted a website for a long time and - even if this is just a Github pages site - I've finally got a little corner of the world wide web. Glad to finally have something sorted out, as I've experimented with university-provided domains in the past that have quickly killed off my HTML/CSS/JS upon graduating.

A few years back, I visited Guatemala with a handful of volunteers to [build homes with a volunteer agency](https://www.fromhousestohomes.org/aboutus) (which you should definitely check out). On the flight back, I read through the Spanish translation of [Michael Hyatt's *"Hazte Oír"*](https://books.google.com.gt/books?id=QjAQ8PGHhFEC&printsec=frontcover#v=onepage&q&f=false) ("Make yourself heard"), which basically boiled down to two things:

1. Make a blog
2. Have a Twitter

At present, Twitter (known as *X*) is a dumpster fire. In addition, I didn't get too much from the book as it felt as if technology had sprinted by it in the 9 years since it was originally published in 2012. However, it rekindled my interest in an internet presence. 

At the time, I was also getting ready to wrap up on my Master's thesis and take a break from academia. A personal site is pretty professional and shows at least a little technical competency. But how to start? Do I buy the domain first and then figure out how to upload files to it? How did the page render itself? By 2021, there were dozens of ways to build a site and it was a proverbial firehose to the face of information.

##  Setting up this site

Getting the site live took some trial and error. I saw "github.io" in the site urls of some collaborators and discovered that Github could host not just a page, but a whole site of pages, media, and plugins. I started with the default Jekyll installation, [as recommended by Github](https://docs.github.com/en/pages/getting-started-with-github-pages) (as of 2024). Building everything from scratch in Jekyll took a lot of time and reminded me that I have little to no sense of complementary colors, so I started looking into [a template](https://pages.github.com/themes/). Dinky was first, then I tried out Slate, and finally decided to go with [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/). Minimal Mistakes supports a lot of stuff that I like, such as a banner and concurrent sidebars. The documentation is also better than I experienced with Dinky and Slate, which made it much easier to set up.

That being said, blog setup was slow. By default, Github pages updates whenever a push passes its tests, which is dependent on Github's status. It also took a while. Running Jekyll locally was a lot faster and made it easier to diagnose errors without congesting the repository.

But man, the Jekyll installation was weird. Jekyll is dependent on Ruby, and a specific version of Ruby. Working on a Unix system, [Ruby 2.6 comes pre-installed](https://www.moncefbelyamani.com/why-you-shouldn-t-use-the-system-ruby-to-install-gems-on-a-mac/) and needs to be overridden for any sort of functionality. This also introduced me to the two types of MacOS shells ([Zsh](https://en.wikipedia.org/wiki/Z_shell) and [Bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell))), which was actually pretty helpful as I've been almost exclusively using zsh for my day-to-day work and I didn't really understand what was meant in older forum posts by "Bash". Both shells are pretty old (predating my parents' marriage), but MacOS has used zsh since 2019. Anywho, I don't remember where but someone suggested using Bash for Jekyll installations and another person said zsh for Macs with non-Intel chipsets. I stuck with zsh and it's working for me so far. Jekyll's instructions [strongly recommend](https://jekyllrb.com/docs/installation/) Chruby as a Ruby manager to toggle versions (system-default 2.6 vs website 3.1+). Then there were a number of required "Gems", or library packages, which needed installation and a final setup of [GCC](https://gcc.gnu.org/install/) and [Make](https://www.gnu.org/software/make/). But in the end, we're left with a terminal that can build the site locally in about a second and a half and all my immediate changes are visible. From there, I copied a template to save a lot of work and am periodically looking through the stuff that might be considered superfluous for my simple operations on this site.

While this setup has been a very enlightening on the innerworkings of the MacOS system, the Ruby programming language, and Github pages, I don't think an everyday person will need this. It's much easier to simply clone or fork another repository and modify a few key files here and there, rather than build entirely from scratch. Like, my non-coding friends wouldn't value the local build options at all and would probably just build their modified files in ChatGPT or something along those lines.

But for me, this is great.

<div style="text-align: center;">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/uRGljemfwUE?si=zwaV6HAWzo3Uycl2" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    <p style="margin-top: 10px; font-style: italic;">How I thought I'd have to set up a website.</p>
</div>

