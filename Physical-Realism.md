# Towards physical realism in VR environments
Lawrence Angrave's Guest VR Lecture Oct 17, 2018 and Oct 23, 2019

How can we create a shared VR immersive realistic emotive experience?

Bandwidth 1 particle x,y,z position x 100 players x 100 hz ?

Need to simulate on client. Dead reckoning
Physics sim particles. 
Sun-Earth 
Rigid bodies. 
Euler Integeration. More stable (more accurate for same computational time) - RK4 Integeration. 

Collisions. 
Atomic Pauli exclusion. Leonard Jone potential is too stiff. Repulsion r^-12

Geometric representations. 
Height maps
Geom primitives to full mesh. 
Spring vs constraint solver to handle/prevent penetration of solid objects.
With force-based approaches, large restorative forces due to collisions cause objects to spin rapidly andfly to infinity. 
Multiple sim steps per graphics update. 
So far all examples of Forward Kinematics 
Inverse Kinematics.

Realtime Fluids.
Surface & volume models. 
Innacurate approximations to Navier Stokes. 

Realtime (40ms) Hair demo. 
Impressive but not real. Reminder that we tend to accomodate graphical weaknesses.

Sound rendering. Eg. Microsoft acoustic demo for a static environment.

# External Videos
https://www.youtube.com/watch?v=2gUtfBmw86Y
	
Fortnite Battle Royale - Gameplay Trailer
https://www.youtube.com/watch?v=2gUtfBmw86Y
Download Fortnite Battle Royale for free today on PC, PS4, Xbox and Mac. 100 players. One giant map. Last one standing wins. Song Featured "Destruction" by Joywave Fortnite Battle Royale is the 100-player PvP mode in Fortnite. One giant map. A battle bus. Fortnite building skills and destructible environments combined with intense PvP combat ...

100 players in Fortnite. How can we share all of their positions? 

http://slither.io
A simpler example of a shared experience. How can we update the position
of ~100 players have a shared experience?

https://youtu.be/kHBcVlqpvZ8?t=35
Uptown spot (Boston Dynamics); Inverse Kinematics Calculate positions
while keeping the effector at the same location

https://www.youtube.com/watch?v=YcfcFqaPcFU
Inverse Kinematics using position of head and hand controllers (HTC Vive)

Classic realtime GPU simulation of Navier-Stokes fluid using a GPU
https://www.youtube.com/watch?v=lqPa389vi4s

Physics simulation loop in Unity -
https://docs.unity3d.com/ScriptReference/Physics.Simulate.html

https://www.youtube.com/watch?v=cN2phdi1AB0
A Reduced Model for Interactive Hairs (SIGGRAPH 2014)

https://www.youtube.com/watch?v=8CU0zRfuhdc
Precomputed Wave Simulation for Real-Time Sound Propagation of Dynamic
Sources in Complex Scenes (Microsoft Research 2016)


Expressing emotions and facial muscles, using a neural net-

https://youtu.be/Aj-zNjff7wY?t=1804
Believable Humans (GDC 2015)


Further reading. (I didn't mention this paper in the talk; just that
physics simulation started with  force-based / impulse (change in
momentum)/ and now position-based dynamics models, in the continued
quest for stability and sufficient accuracy with a limited budget.

http://matthias-mueller-fischer.ch/publications/posBasedDyn.pdf
Position Based Dynamics
