# Resume

Flow sensors are really expensive, so we used the Venturi principle to calculate the flow knowing the pressure drop between two different sections of a tube. It worked really well. The tube is 3d printed, the pressure is measured with a differential sensor and wired into an Arduino... so, what time is it??? IT'S...!

 <img src="/images/venturitime.png" width="500">

# Some physics

Suppose a pipe with a constriction, like this:

 <img src="/images/tube.png" width="500">

 In the ideal and magical world of physics there is no friction, the flow inside a pipe is laminar and incompressible. So, assuming all of that nonsense and something less crazy, conservation of mass, we get that at any point, as the density is the same:

 A1V1=A2V2

 Now, due to conservation of energy (more magical stuff), when the kinematic energy increases (the velocity) the potential energy decreases (the pressure), so there is a pressure drop between the larger section of the tube and the constriction when the fluid accelerates, which can be calculated using the Bernoulli equation, which relates two different points of fluid in a stream:

the bernoulli equation will be here 

Now, the idea is that we want to know the flow, so, knowing the shape of the tube and the pressure drop should provide the data, solving for the flow we get:

more equations i guess

# Design

As we want to measure the pressure difference we need a differential pressure sensor. The pressure drop will be a parameter for choosing a sensor with the right range and precision, and the pressure drop will depend on the sections of the tube. 

We are designing this device for a mechanical respirator that uses some medical tubing and adapters, the diameters are usually 22 or 25 mm. This give us some starting point for the larger section, which will have an inner diamater of 22 mm. The outer diameter along the tube was designed to fit in our specific machine, so it does not really matter to you. Now, the goal is to choose 

 <img src="/images/cad.png" width="500">

# Manufacturing

The tube was printed with a 0.1 mm layer height in a Form2 SLA printer, from Formlabs. The material used whas tough resin, as the standard resine is too brittle and we did not want that the piece brake apart if dropped by accident. The hoses to joint the tube with the sensor are size 8 supply suction tubes, fits just right. A small pcb was made for the sensor to keep it static, as it is really small and fragile. 

 <img src="/images/printed.png" width="500">

# Programming

We used an Arduino to get the data, as is really easy to use, all hail our God Arduino! before knowing it my life was only of pain and misery. Now i have some joys now and then when the code compiles. 

The first step is to get the reading from the sensor, which has two analog outputs.

# Tests

SOON

