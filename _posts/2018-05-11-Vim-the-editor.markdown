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
&nbsp;&nbsp;&nbsp;&nbsp;Only the people who really write texts themself know what a problem a _single_ screen is. When you write on paper - you have pages, you probably have a pile or several piles of drafts around you, maybe you have a notebook or a notepad and browse through its pages and leave it open on one of them... you have multiple parts of your composition that you can look at _simultaneously_ (at least from the corner of your eye). Of course this in not true with screens, they are only a small part of your field of vision, and it's even worse with a single screen that is just that - a _single_ screen occupying 10% of your field of vision or so. At some point in time long ago I realised how much of my precious time is being spent on this idiotic routine of opening and closing files, scrolling through directory trees and the texts themself and, most importantly, on what I would call 'aiming' at some particular single point on the screen where you need to place your cursor in order to start making corrections. Let me remind you that this precious time is gone forever and it's a big question whether you will be able to achieve the proverbial 'economy of scale' later by doing everything digitally and on the screen from the very beginning. It's important to understand that there are three interconnected tasks in this battle with the singularity of the screen, namely:
- making a part of text visible in the window. The trick is to keep the image of a very long 'page' that you can look at through a ordinary page size window. And this window is moving down/forward or up/backward along this very 'tall' page. In this process you don't care where the cursor is, you are looking at the text and reading it or rearranging the big blocks of it;
- 'aiming' at a point in text where you want to make a *correction*, *insertion* or *deletion*. By 'aiming' I mean making a __*particular*__ part of text __*with the cursor*__ visible in the window in order to be able to perform the surgery on it. This process in its turn consists of two parts:
  * reading the text that immediately precedes or/and follows the change that you have in mind;
  * puting the cursor into an __*exact*__ position required for the surgical intervention.<br>

&nbsp;&nbsp;&nbsp;&nbsp;I've already used twice the metaphor that I'm using to think about it - the surgic procedure with the help of a cursor/'scalpel'.<br>
&nbsp;&nbsp;&nbsp;&nbsp;To the point. Here are the important things that I learned about Vim/Neovim. <br>
## Navigation in file and on screens.
Once you've opened a file you can instantly move to the end of it and back.<br><br>
**gg** - beginning of the file;  **G** - last line of the file.<br><br>
### Moving the frame through which you see the text.
**Ctrl-f** - **f**orward full screen; **Ctrl-b** - **b**ackward full screen.<br><br>
**Ctrl-d** - **d**own half screen; **Ctrl-u** - **u**p half screen.<br><br>
### Shift content inside the window together with the cursor.
**zt** = **z + CR** - so that the cursor would be at the **t**op;<br><br>
**zb** = **z-** - so that the cursor would be at the **b**ottom;<br><br>
**zz** = **z.** - so that the cursor would be in the **middle**.<br><br>
### Shift the cursor only, keep the content as it is.
**H** - move the cursor to the **h**ighest line in the window;<br><br>
**L** - move the cursor to the **l**owest line in the window;<br><br>
**M** - move the cursor to the **m**iddle line in the window.<br><br>
## Windows.
The most important command for Vim's windows is a **Ctrl-w** two-finger movement of your left hand, you type another letter after doing it and you get a window action.<br><br>
#### Maximizing - minimizing.
**Ctrl-w + _** - maximize the hight of the current window;<br><br>
**Ctrl-w + |** - maximize the width of the current window;<br><br>
**Ctrl-w + =** - make all the windows the same size.<br><br>
Jumping between windows is done with the ordinary **h, j, k, l** preceded with **Ctrl-w**<br><br>
**Ctrl-w + <h, j, k, l>** - move to the window: on the left, below, above, on the right.<br>
#### Creation of new windows.
Besides that you only need to open a new window with another file in it by splitting the window horisontally:<br><br>
**:new** _filename.txt_ - open the filename.txt in a window split horisontally;<br><br>
**:vert new** _filename.txt_ - open the filename.txt in a window split vertically.<br><br>
#### Closing of a window.
A separate important way to think about all the realities inside Vim - the quit command, which closes the current window if there are several of them.<br><br>
**:q** - just quit;<br>
**:q!** - quit without saving whatever changes you have made (probably by accident);<br>
**:wq** - write the changes made in the current window into the file, then quit.
## Registers.
Registers are one of the biggest achievements of Vim even if not so many people understand that they can joggle their contence with the help of **:let @a=@b** assignments between the registers, the system clipboard **"+** and the text selected in the operating system which is accessible in __"*__.
#### Numbered
From **"0** to **"9**; **"0** is separate **"1** - **"9** are a stack. Vim fills this stack of registers with text from delete-like commands without an address of a target register and pops up the contence when the **u**ndo command is issued.<br>
**"0** - the most recent yank command...<br>
**"1** - the most recent delete or change command...<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;...unless another register was specified.<br>
With each successive deletion 1 is moved down the stack to 2 etc.etc., 9 is purged (and lost).
#### Named
From **"a** to **"z**. The main bunch, where you store the important chunks that you are planning to insert somewhere but don't know yet where it will go. As I've said, you can assign them to each other with the help of **:let ...**
#### Read-only
These can be used with the **p**ut and **P**ut commands only.<br>
**":** - the most recent executed command-line;<br>
**".** - the last inserted text;<br>
**"%** - the name of the current file;<br><br>
**"#** - bla-bla 'alternate file' and it is writable; //not for humans <br>
#### Expression
**"=** - is a way to use an expression in commands which use a register;
#### Selection and drop
__"*__ - in selection (in the system);<br>
**"+** - dropped to (system) clipboard;<br>
**"~** - read-only, the result o last drag-n-drop;
#### Search pattern
**"/** - ;
#### Small delete
**"-** - the 'small delete' register; the delete goes here if it is less than one line.
#### Programmer perversions
**""** - text deleted with the "d", "c", "s", "x" commands;<br>
**"_** - 'black hole' register;



