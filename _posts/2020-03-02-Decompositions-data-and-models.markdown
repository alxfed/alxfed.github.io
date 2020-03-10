---
layout: post
title:  "Decompositions of Data and Models."
excerpt: "In the same way as popularization of Fourier transform and operational calculus by Weiner changed the technology of the 20-th century the 21-st century is calling for another type of decomposition techniques that will help solve many similar problems."
date:   2020-03-02  7:50 am
categories: blog posts
---
### "Norbert Wiener did a great job." 
&nbsp;&nbsp;&nbsp;&nbsp;He started it in the 30-s by popularizing the "Generalized
harmonic analysis", then, of course, wrote the bible of all 20-th century electrical engineers
"Extrapolation, Interpolation and Smoothing". Where are we now with all that?
### The analogy between the Fourier Transform and Models/Learning
&nbsp;&nbsp;&nbsp;&nbsp;I had this blurred understanding for quite a while that
"I've seen it all before" when I kept looking through the achievements of Machine
Learning, Deep Learning, Neural Network Training and all that. 
Here's the analogy:
1. 'Learning' lets the input data 'force' changes in the state of the 'learning system'. 
Then, when you apply other input to the 'trained' system during the 'inference' you are applying it
to a 'stationary state' achieved during the training. The system that is being trained compounds
information from the input data by accumulation of 'effects' (caused by 'causes') in the
'eigenfunctions' of the learning system. In this way it's like a 'spectrometer' with a comb of
band-pass filters or resonant LC contours or interference of different 'rays' in a hologram.
The accumulation of 'knowledge' during 'learning' is, of course, _non-linear_, - 
the signal changes the properties of the 'resonant circuit' that it 'excites'.
2. (or 1') If you noticed I made (in the same way as many of them do) a 'shuffle' in this card cheat
hocus pocus. I started talking about the eigenfunctions which are _states_ of the system, then
said that information accumulates _in them_. This is not true, the states of the system are
transient, they come (when you input something to the system) and go (when you remove this
input), but the properties of the system can change. So the real way of saying what is happening
in the system would be: when an eigenfunction is 'excited' by the input this 'excitation' can
change the properties of the system so that the relative weight of this eigenfunction or its' 'shape'
will be different when it will be excited next time. So...
3. There are two possible mechanisms of accumulation of 'knowledge'/changes in the system: in the 
relative 'weights' of 'excited' eigenfunctions and in changes of the eigenfunctions themselves. 
Changes in weights would be purely 'spectral' or Fourier-like type of influence, while changes
in the 'shape' of eigenfunctions themselves is a different, non-Fourier decomposition and that's 
what we will be talking about shortly. But in any case the analogy is with integration/convolution 
of an input function with a sine harmonic which is obviously very similar to the 'training'.
4. The main problem of 'trained systems' though are their extensions and combinations. 
We typically need to restart 'training' all over again if we add something to a 'taught' 
neural network or learning system. Why? Because of the non-linearity, of course! Moreover,
if we are using the 'variation of eigenfunctions' method of training the added part of the
network may change them altogether. It's like adding (or dropping) a couple of members of the
equation. It is not a 'changed' equation, it's a totally _new_ equation with new eigenfunctions.
On top of that the 'coordinate system' of old eigenfunctions may or may not be able to develop 
'projections' onto the new coordinate system of new eigenfunctions. In this aspect 'training' is
_different_ from Fourier decomposition, there everything is linear and hence - additive and scalable.
5. Also, talking about the changes of functions for decompositions, I've had this idea in 
my head for quite a while, that sequences of random numbers are a perfect set of 'orthonormal'
functions necessary for decompositions. Now, if you are about to change one of the functions
in your 'basis', make sure that the new one is 'normal' to all the rest, and it's a condition
that is hard to satisfy with usual functions, but simple to satisfy with these random sequences.
But this is a method of finding 'orthogonal' functions quite different from the sine harmonics
of the same frequency or the natural numbers counts of an interval in Rademacher method<br>

### Explanation.
&nbsp;&nbsp;&nbsp;&nbsp;The main idea of usefullness of Fourier transform comes from the fact that if 
you substitute an eigenfunction into a differential equation it is satisfied (by
definintion of an eigenfunction); if the equation is linear a substitution of any 
multiple of the eigenfunction has the same effect, the equation is satisfied. Then
why not 'decompose' the 'force', acting upon the system into a _linear_ combination
of eigenfunctions and watch their evolution separately, right? We will see 'resonances'
of 'harmonics' and all that stuff. That's how decomposition is useful.<br>
&nbsp;&nbsp;&nbsp;&nbsp;So in this scheme, which is just a continuation of the idea of finding a particular 
solution of differential equation with initial conditions by using the 'undetermined 
coefficients', of more generally, for a 'force' on the right, a 'variation of 
parameters' (Euler, Lagrange, Duhamel or whoever) we seriously rely upon the 
superposition principle. And that's exactly why the Fourier series is a sum 
(superposition) of terms.<br>
&nbsp;&nbsp;&nbsp;&nbsp;The other property that is being used is the translational invariance
of linear operators, which, if you think about it clearly, is a 'superposition' principle of sorts
too, it describes the behavior of the function of a sum or arguments, in this way there is a 
'superposition' of the initial value of the argument and the 'additional' part of the argument.
As we all know for linear differential operators of wave equation this leads to a function that
is a product of functions with these parts of the value.<br>
<br>Later.
