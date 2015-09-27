---
layout: post
title: Developing From a Chromebook
---

### What I've learned since I started using a Chromebook for web development

I know there are probably thousands of articles and blog posts out there about doing design and development work on a Chromebook. I'm not out to compete with any of those posts or change anyone's view on the subject. The purpose of this post is simply to share my experiences so far since I've been working almost entirely from my Chromebook for the last six months.

![Chromebook](https://c2.staticflickr.com/6/5322/10187219156_2f9c270a1e.jpg)

##### Initial Thoughts

At first glance, it is a little offputting to think about a $200 laptop running a fringe operating system that hasn't been around long being your primary workhorse computer. I have always worked from my desktop computer until I started getting tired of being anchored to the desk and not being able to take my work everywhere.

Enter the [Chromebook](https://www.google.com/chromebook/). I don't even own one of the new Chromebooks. I'm using the Samsung Chromebook 1st generation which has an ARM processor rather than an Intel processor. That is the only drawback of Samsung's model. However, performance has always been nearly flawless. I frequently have a text editor, a Slack app, Evernote, Chrome with 10 or so tabs open, a couple Youtube videos open, and be running background processes in the terminal. All the while, I notice very little performance reduction doing anything other than loading websites with tons of animations.

It took me about two months to get fully integrated into using a "cloud only" computer. You're also restricted to web applications or applications from the [Chrome Web Store](https://chrome.google.com/webstore/category/apps). Within the app store, there are a large amount of apps that are really just shortcuts to web applications. I try and steer clear of those apps and use only "desktop" applications that are installed and (usually) usable offline.

It might seem annoying to have to search through an app store to find the tools you need to replace what you probably already have installed on your PC or Mac. The truth is, just about everything you could ever want for web development can be obtained or has a valid alternative on ChromeOS. One prime example is [Caret Text Editor](http://thomaswilburn.net/caret/). I'm currently writing this post from Caret. It's a fantastic, customizable, offline text editor for ChromeOS that I have never had a single issue with. It's perfect and does everything I need it to do.

##### Setting Everything Up

I won't go into the complete details on how to set everything up exactly how I have it but I will link to the places where I learned how to set it up this way. The first thing to do is enable developer mode on the Chromebook. This is done by holding Esc and Refresh, then pressing the power button. More information on that can be found [here](http://www.cnet.com/how-to/how-to-enable-developer-mode-on-a-chromebook/).

With developer mode enabled, you now have root access to the Chromebook. Once this was done, I downloaded [Crouton](https://github.com/dnschneid/crouton) and set up a Linux Unity operating system that runs alongside ChromeOS.

> "Why would I want to do this?"

When you have everything set up, all you have to do is open the terminal (CTRL + ALT + T), type "shell", then type "sudo enter-chroot". You're now controlling your Linux operating system from a terminal session in ChromeOS. This means you never have to switch out of ChromeOS to do powerful things like install dependencies and use Git for version control management in the terminal.

Some of the things I installed for work on web design through the terminal:
* Git
* Nodejs and NPM
* Bower
* Grunt
* VIM
* Ruby and RubyGems
* Less and Sass

Your two operating systems have root access to the Downloads folder, which is shared. You can do all of your work in there as long as you use some kind of version control to make sure your files get backed up to the cloud regularly. You can always install [Dropbox](https://chrome.google.com/webstore/detail/file-system-for-dropbox/hlffpaajmfllggclnjppbblobdhokjhe) to sync files to and from your local directories or use Github to store all of your code projects. As long as your work is being uploaded to the cloud, there is no danger of losing anything ever.

##### What Apps I Use

I love trying out different apps. It's not usually because I really need them and I usually uninstall apps that I download on a whim a week later. I just like to see what they look like and how they work because I always enjoy checking out the interface design work of the developers. There are some that are really good and some that seem to be poorly ported from mobile apps or web-based applications.

Here are some that I love and use often:
* Caret
* Slacky
* Evernote
* Sunrise Calendar
* File System for Dropbox
* Gravit
* Google Keep

There are quite a lot of other apps that I've tried and loved but just didn't have a use for really. Or I already had something that does it better. One example of this is [StackEdit](https://stackedit.io/). It's a beautiful editor for Markup that I think would be great for managing large-scale projects like wikis. However, for writing smaller markdown documents like blogs posts, I just use my everyday text editor.

##### Conclusion

All in all, working from a Chromebook has been great. The battery charges quickly and lasts a long time. The performance is solid, and the developer support is there. I get around by bike so it's nice to have my work computer be light and fit in my bookbag. If something ever happens to it, everything is already in the cloud so I never have to worry about losing files again. For me, that's a nice feeling.