---
layout: post
title:  "Google colab TPU, how many Cray-2s would that be?"
excerpt: "When I was leaving science in the 90-s the best supercomputer of the time was Cray-2 with 1.9 GFLOPS peak performance, now I bumped into a _free_ cloud service last night..."
date:   2019-01-29  10:11 am
categories: blog posts
---
&nbsp;&nbsp;&nbsp;&nbsp;The name of the cloud service is "Colaboratory" and it is here: [Google Colaboratory](https://colab.research.google.com/notebooks/welcome.ipynb) - this is a "Welcome notebook" that opens even if you are not logged into your Google account. The only thing that happens after you log in - it links the session with your "Google drive".<br>
&nbsp;&nbsp;&nbsp;&nbsp;The words that immediately stand out on this page are, of course the **GPU** and **TPU**. You probably know that Kaggle has added the GPU option to its kernels lately, which speeds up everything you do drammatically, but TPU? This is something new. Let's test it right away!<br>
&nbsp;&nbsp;&nbsp;&nbsp;I created this repo for my experiments with Colab here: [colab repo](https://github.com/alxfed/colab) and will be posting the notebooks from it there and loading whatever I post into this the repo to my alxfed gmail account in Colab.<br>
&nbsp;&nbsp;&nbsp;&nbsp;The first experiment is the notebook that they offer for testing the TPU. Is it worth the effort necessary to study their toy? Here's the result: [the TPU colab notebook that I saved from there to my repository](https://github.com/alxfed/colab/blob/master/Hello%2C_TPU_in_Colab.ipynb), and... Can you see the number? `TFlops: 165.54` Wow! Just wow!<br>
&nbsp;&nbsp;&nbsp;&nbsp;Let me remind you something: the first generation of supercomputers, which pretty much ended with Cray-2 reached the amazing result of 1.9 GFlops peak performance. And those were pretty unique super-embargo-we-will-not-give-it-to-anybody room-sized moster computers. And here, I was just browsing and bumped into this thing because somebody in a chat mentioned it... And it is free...Just think about it:<br><br>
**A HUNDRED THOUSAND Cray-2s!**<br><br>
That was impressive, Google!<br><br>
Later.
