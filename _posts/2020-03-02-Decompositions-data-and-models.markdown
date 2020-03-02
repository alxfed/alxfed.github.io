---
layout: post
title:  "Decompositions of Data and Models."
excerpt: "In the same way as popularization of Fourier transform and operational calculus by Weiner changed the technology of the 20-th century the 21-st century is calling for another type of decomposition techniques that will help solve many similar problems."
date:   2020-03-02  7:50 am
categories: blog posts
---
### "Norbert Wiener did a great job." 
(Sorry for the 'Trump' joke, I couldn't help it)<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;He started it in the 30-s by popularizing the "Generalized
 harmonic analysis", then, of course, wrote the bible of all 20-th century engineers
 "Extrapolation, Interpolation and Smoothing". Where are we now with all that?
### The analogy between the Fourier Transform and Models/Learning
&nbsp;&nbsp;&nbsp;&nbsp;I had this blurred understanding for quite a while that
"I've seen it all before" when I kept looking through the achievements of Machine
Learning, Deep Learning, Neural Network Training and all that. 
Here's the analogy:
1. 'Learning' lets the input data 'force' changes in the state of the 'learning system'. 
Then, when you apply other input to the trained system during the inference you are applying it
to a 'stationary state' achieved during the training. But the way, the system accumulates
information from the input data by accumulation of 'effects' (caused by 'causes') in the
eigenfunctions of the learning system. In this way it's like a 'spectrometer' with a comb of
band-pass filters or resonant LC contours. The accumulation of 'knowledge' during 'learning'
is _non-linear_, the signal changes the properties of the resonant circuit that is excites.
2. There are two possible mechanisms of accumulation of 'knowledge'/changes in the system: in the 
relative 'weights' of eigenfunctions and in changes of the eigenfunctions themselves. Changes in
weights would be purely 'spectral' or Fourier-like type of influence, while changes in the 'shape' of eigenfunctions
themselves is a different, non-Fourier decomposition and that's what we will be talking about
in a short while.
3. The main problem of 'trained systems' are, of course, their extensions and combinations. 
We typically need to start the training all over again if we add something to a 'taught' 
neural network or learning system. Why? Because of the non-linearity, of course! Moreover,
if we are using the 'variation of eigenfunctions' method of training the added part of the
network may change them altogether. It's like adding (or dropping) a couple of members of the
equation. It is not a 'changed' equation, it's a totally new equation. On top of that the
'coordinate system' of old eigenfunctions may or may not be able to develop 'projections' 
onto the new coordinate system of new eigenfunctions.<br>
### Explanation.
&nbsp;&nbsp;&nbsp;&nbsp;The main idea of usefullness of Fourier transform comes from the fact that if 
you substitute an eigenfunction into a differential equation it is satisfied (by
definintion of an eigenfunction); if the equation is linear a substitution of any 
multiple of the eigenfunction has the same effect, the equation is satisfied. Then
why not 'decompose' the 'force', acting upon the system into a _linear_ combination
of eigenfunctions and watch their evolution separately, right? We will see 'resonances'
of 'harmonics' and all that stuff. That's how decomposition is usefull.<br>
&nbsp;&nbsp;&nbsp;&nbsp;So in this scheme, which is just a continuation of the idea of finding a particular 
solution of differential equation with initial conditions by using the 'undetermined 
coefficients', of more generally, for a 'force' on the right, a 'variation of 
parameters' (Euler, Lagrange, Duhamel or whoever) we seriously rely upon the 
superposition principle. And that's exactly why the Fourier series is a sum 
(superposition) of terms.<br><br>
<br><br>Later.
