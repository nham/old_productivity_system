The first step in solving the n-body problem is to solve the 2-body problem. One way of solving it is by using relative coordinates. "we can transform the two-body problem into a one-body problem"

This wasn't in chapter 3, but I want to solve it analytically before I proceed to using the approximation below.

Here's a diagram:

(F1 and F2 diagram goes here)

$$F_1 = m_1 a_1$$
$$F_2 = m_2 a_2$$

So $F_1 + F_2 = m_1 a_1 + m_2 a_2$

First step is to calculate c.o.m. of the two particles. We are assuming that the two body-system is isolated w.r.t. to everything else, so that the c.o.m. has no net force on it and thus moves with constant velocity in any inertial frame of reference.


## Approximation

Consider the problem where we have one massive stationary body and another much smaller body moving w.r.t. the first body, then the problem is easy to solve: we assume the massive body never moves, and then we just solve newton's equation for one body.

(This is an approximation? Do both bodies always move w.r.t. the center of mass in a two-body interaction?)


A new origin changes the actual geometric vector. A rotation or reflection doesnt actually change what arrow it is, geometrically, just its coordinate representation.


We also will be sticking with inertial frames of reference for now.




So we have a non-rotating coordinate system fixed to the c.o.m.So we have a single coordinate system and the trajectories $r_1$ and $r_2$, each w.r.t. the coordinate system. We can compute c.o.m. Note that

$$r := r_2 - r_1$$

is the same no matter what the origin of the coordinate system is.
