To a pretty good approximation, in modeling some number of bodies that are far enough apart, we can neglect any forces except gravity. We can also consider them to be point particles for simplicity.

There are about 100 billion stars in our galaxy.

> The sun is unremarkable in its properties. Its mass is in the mid range of what is normal for stars: there are others more than ten times more massive, and there are also stars more ten times less massive, but the vast majority of stars have a mass within a factor ten of that of the sun. Our home star is also unremarkable in its location, at a distance of some thirty thousand light years from the center of the galaxy. Again, the number of stars closer to the center and further away from the center are comparable. Our closest neighbor, Proxima Centauri, lies at a distance of a bit more than four light years.

In a scale model, if we would represent each star as a cherry, an inch across, the separation between the stars would be many hundreds of miles. It is clear from these numbers that collisions between stars in the solar neighborhood must be very rare. Although the stars follow random orbits without any traffic control, they present such tiny targets that we have to wait very long indeed in order to witness two of them crashing into each other. A quick estimate tells us that the sun has a chance of hitting another star of less than 10 ?16 per year. In other words, we would have to wait at least 10^16 years to have an appreciable chance to witness such a collision. Given that the sun?s age is less than five Gigayears, 5.10 9 years, it is no surprise that it does not show any signs of a past collision: the chance that that would have happened was less than one in a million. Life in our galactic suburbs is really quite safe



constant time step => adaptive universal time step (binary stars need faster clocks since their calculations are more sensitive to roundoff error) => adaptive individual time step


Another software technique is introducing a local coordinate system for binary star systems so that we aren't subtracting two nearly identical numbers, which poses numerical problems due to lack of floating point precision.

The Hermite scheme is a modern integrator the book focuses on. It's adaptive universal time step.
