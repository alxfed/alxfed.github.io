---
layout: post
title:  "Decompositions of Data and Models."
excerpt: "In the same way as popularization of Fourier transform and operational calculus by Weiner changed the technology of the 20-th century the 21-st century is calling for another type of decomposition techniques that will help solve many similar problems."
date:   2020-03-02  7:50 am
categories: blog posts
---
### "Norbert Wiener did a great job." (This is 'Trump' joke)
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
information from the input data is by accumulation of 'effects' (caused by 'causes') in the
eigenfunctions of the learning system. In this way it's like a 'spectrometer' with a comb of
band-pass filters or resonant LC contours. The accumulation of 'knowledge' during 'learning'
is _non-linear_ the signal changes the properties of the resonant circuit that is excites.

### Explanation.
&nbsp;&nbsp;&nbsp;&nbsp;The main idea of usefullness of Fourier transform comes from the fact that if 
you substitute an eigenfunction into a differential equation it is satisfied (by
definintion of an eigenfunction); if the equation is linear a substitution of any 
multiple of the eigenfunction has the same effect, the equation is satisfied. Then
why not 'decompose' the 'force', acting upon the system into a _linear_ combination
of eigenfunctions and watch their evolution separately, right? We will see 'resonances'
of 'harmonics' and all that stuff. That's how decomposition is usefull.
&nbsp;&nbsp;&nbsp;&nbsp;So in this scheme, which is just a continuation of the idea of finding a particular 
solution of differential equation with initial conditions by using the 'undetermined 
coefficients', of more generally, for a 'force' on the right, a 'variation of 
parameters' (Euler, Lagrange, Duhamel or whoever) we seriously rely upon the 
superposition principle. And that's exactly why the Fourier series is a sum 
(superposition) of terms.<br><br>
<br><br>Later.
