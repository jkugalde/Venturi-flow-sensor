## Resume

Flow sensors are really expensive, so we used the Venturi principle to calculate the flow knowing the pressure drop between two different sections of a tube. It worked really well. The tube is 3d printed, the pressure is measured with a differential sensor and wired into an Arduino... so, what time is it??? IT'S...!

 <img src="/images/venturitime.png" width="500">

# Some physics

Suppose a pipe with a constriction, like this:

 <img src="/images/tube.png" width="500">

 In the ideal and magical world of physics there is no friction, the flow inside a pipe is laminar and incompressible. So, assuming all of that nonsense and something less crazy, conservation of mass, we get that at any point, as the density is the same:

 A1V1=A2V2

 Now, due to conservation of energy (more magical stuff), when the kinematic energy increases (the velocity) the potential energy decreases (the pressure), so there is a pressure drop between the larger section of the tube and the constriction when the fluid accelerates, which can be calculated using the Bernoulli equation, which relates two different points of fluid in a stream:

bernoulli equation

Now, the idea is that we want to know the flow, so, knowing the shape of the tube and the pressure drop should provide the data, solving for the flow we get:

more equations.

# Design

# Manufacturing

# Programming

# Tests

