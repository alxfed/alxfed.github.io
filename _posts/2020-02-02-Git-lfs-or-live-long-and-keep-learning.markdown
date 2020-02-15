---
layout: post
title:  "git lfs ! Or live long and keep learning"
excerpt: "It took me a couple of years of going on my own until I finally bumped into this git-lfs thingy!"
date:   2020-02-02  10:22 am
categories: blog posts
---

&nbsp;&nbsp;&nbsp;&nbsp;Wrangling with data and joggling with big CSV 
files is an everyday affair if you are doing something real. Sometimes 
I would _**die**_ for reverting what I've just done... to this 340Mb CSV 
file. Lately I started passing data between my applications and remote 
computers (like colab) in *.sqlite files, which are not much smaller but 
should be dealt with as (big) binary files. The version control is necessary!
Now, as it turns out there is this **git-lfs** 'extension' for git that 
had been designed a long time ago for just that. Duh!<br><br>
#### Where to find
&nbsp;&nbsp;&nbsp;&nbsp;I will write more about it later, but for now 
here's a couple of links:<br><br>
- https://git-lfs.github.com/
- [about it on GitLab](https://docs.gitlab.com/ee/administration/lfs/manage_large_binaries_with_git_lfs.html)
- [about it on GitHub](https://help.github.com/en/github/managing-large-files/about-storage-and-bandwidth-usage)<br>
#### Afterword
&nbsp;&nbsp;&nbsp;&nbsp;Almost immediately after I posted about this finding
on facebook, one of the 'maintainers' of [DVC](https://dvc.org/) commented on
my post and suggested their solution as a better one (for the data science)
scenarios. I'm not sure yet. I understand why the GitHub native solution is
good. I'm not quite sure where to put the 'extra flexibility' that makes you
do some of the _same_ work yourself... But I will try it some day.
 

