# CarND PID Control
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)

Self-Driving Car Engineer Nanodegree Program

---

You can find the Clojure version of Udacity's PID controller project from term 2 of the self-driving
car engineer nanodegree [here.](https://github.com/ericlavigne/CarND-PID-Clojure)
All thanks to Eric Lavigne: He's a great software architect.

## How to find the right parameter for the PID-controler:
I did this process by hand. First search find good values for P and D while I is still zero at 30mph.
This is the case at 30mph for example 

####P = 0.1
####D = 2.0
####I = 0.0
 
For a speed of 60mph increase the D value, while lowering the P value.A small I value improves the result a bit.

####P = 0.05
####D = 4.0
####I = 0.001

Finaly at 70mph a optimal value of I is neccesary to drive around the corner.
 
####P = 0.025
####D = 5.0
####I = 0.002

##Speed = 70MPH:

![Car goes with 70MPH around the lake trac:](S70.gif)

## Conclusion
The new starter code in Clojure has a speed of 70mph for the lake trac, while the old starter code in C++ has a speed limet of 50mph only.

