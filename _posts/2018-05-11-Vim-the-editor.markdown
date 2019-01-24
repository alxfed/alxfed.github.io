---
layout: post
title:  "Vim - the editor for the people who think before doing."
excerpt: "Or: your adult life begins when you permanently remap CapsLock to Esc and live happily ever after. And I will tell you how to do that on Ubuntu too."
date:   2018-05-11  9:00 am
categories: blog posts
---

&nbsp;&nbsp;&nbsp;&nbsp;For many years after the untimely death of Word 5.0 for DOS around the year 1995 I've been using editors with graphical user interfaces but I always craved for the software that operates instantaneously and there was no way to get it anymore.<br>
&nbsp;&nbsp;&nbsp;&nbsp;For a totally different reason I dove into the world of Linux and surely enough I bumped into the 'cult of Emacs' but didn't notice the much quieter crowd of Vim users. Yes, **Vim**! Here you are! I want to say a few words about my new friend.<br><br>
### Moving through texts
&nbsp;&nbsp;&nbsp;&nbsp;Only the people who really write texts themself know what ~ problem a _single_ screen is. When you write on paper - you have pages, you probably have a pile or several piles of drafts around you, maybe you have a notebook or a notepad... you have multiple parts of your composition that you can look at _simultaneously_ (at least from the corner of your eye). Of course this in not true with screens that are only a small part of your field of vision, and it's even worse with a single screen that is just that - a _single_ screen. At some point in time long ago I realised how much of my precious time is being spent on this idiotic routine of opening and closing files, scrolling through texts and, most importantly, on what I would call 'aiming' at some particular single point on the screen where you need to place your cursor in order to start making corrections. Let me remind you that this precious time is gone forever and it's a big question whether you will be able to achieve the proverbial 'economy of scale' later by doing everything digitally and on the screen from the very beginning.<br>
&nbsp;&nbsp;&nbsp;&nbsp;To the point. Here are the important things that I learned about Vim/Neovim. <br>
## Navigation in file and on screens.
**gg** - beginning of the file;  **G** - last line of the file.
### Scrolling
**Ctrl-f** - **f**orward full screen; **Ctrl-b** - **b**ackward full screen.<br><br>
**Ctrl-d** - **d**own half screen; **Ctrl-u** - **u**p half screen.<br><br>
### Shift content inside the window together with the cursor
**zt** = **z<CR>** - so that the cursor would be at the **t**op;<br><br>
**zb** = **z-** - so that the cursor would be at the **b**ottom;<br><br>
**zz** = **z.** - so that the cursor would be in the **middle**.<br><br>
### Shift the cursor only, keep content as it is
**H** - move the cursor to the **h**ighest line in the window;<br><br>
**L** - move the cursor to the **l**owest line in the window;<br><br>
**M** - move the cursor to the **m**iddle line in the window.<br><br>
## Windows
**Ctrl-w + _** - maximize the hight of the current window;<br><br>
**Ctrl-w + |** - maximize the width of the current window;<br><br>
**Ctrl-w + =** - make all the windows the same size.<br><br>


