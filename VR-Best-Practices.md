# VR Best Practices
(initial version based on Victor guest UIUC lecture 4/16/18)

## Best Practice Guides
Unity https://unity3d.com/learn/tutorials/topics/virtual-reality/optimisation-vr-unity
Oculus Best Practices Guide https://static.oculus.com/documentation/pdfs/intro-vr/latest/bp.pdf
Microsoft https://docs.microsoft.com/en-us/windows/mixed-reality/best-practices-for-working-with-unity-and-visual-studio

## Common mistakes
* It is easy to create bad VR!
* Use a flexible event based programming structure. write`actionPerformed` type of function which will automagically called by event manager. rather than directly gluing the cause to the otput.
`if(scene1victory) { startConfettiCanon(); fizzleSparkler();} etc`


## Use C# delegates
```C#
delegate void MyDelegate (); // can point to a function that takes no arguments and returns nothing

void iWantToBeCalled() { // does awesome stuff

MyD delege = new MyDelegate(iWantToBeCalled);
// Now I can run it
deleg();
```
## The Callback machine
Solves Non-blocking control flow, too many singletons, no need for global data, less messy code

Stores a map a string (the event name) to array of delegates (the callbacks to be executed)
RegisterListener - place delegate in the dictionary under an event name
TriggerEvent - iterate and call each delegate associated with the event name

# Other Unity dangers
## Fluid Component structures
Strict class heirachies have their benefits
Loading resource as needed, dynamic resultions
* Resources.Load, GameObject.Find can introduce lag
* Always Using basic Unity for everything. There are other tools that are more advanced e.g. Cry , unity
* Networking. Creating Networking games is hard. Reduce the complexity of the other components of your app.

## Mountain Goat VR

Todo youtube link
Elastic camera. Constant changing acceleration of camera. Does not seem to benefit from VR; no UI, no touch interaction.

## Lucky's tail VR
Todo youtube link

3D platform games carefully control the camera. In VR, user-controlled camera control makes it harder to judge distance.

## Testing concerns
Testing is expensive. Testers usually don't identify issues directly. e.g. "Camera is cutting" -> "It made me sick"

## Minimizing Latency
* FSP can't drop no matter what
* Games wih sandbox elements might have some issues. Add constraints

## Accelerations

* Understand vection and VOR effects
* Rotations are accelerations
* Teleportation effects
* Preparing users for motion

### Case study - Robo recall game. 

Visual effects to prepare player for teleportation. Teleportation effect fades to white then fades back in.
Some confusion about orientation after teleportation. The indicator indicates orientation as if player is at zero orientation.

### Case study - DOOM
Hybrid sidestepping and teleporting. Teleporting implemented as a short continuous motion dash. Maintains orientation. It is a trade-off -still some sickness effects after 30 minutes play. 

## Reduce Field of view
"The less they see, the less they feel"

### Case study Elite Dangerous
Lots of deliberate visual obstructions to remind user that they are in vehicle.
Interesting hybrid approach. If you the player looks up there is a greater field of view.

## Movement schemes
Movement inline with the viewing dir is optional.
Preparing the body for movement goes a long way

Case study - Sprint vector game
Breaks traditional rules but not uncofrtable. Tricks -

Large physical arm movement
Superman arms when traveling through air

## Third-person cameras

Subject to the same accelerations as first person
Camera swings can be large than first person when following another object
We lose some F of V control
Big advantage: We can decouple camera from avatar movement
Flight sims can benefit from this. e.g. if plane is rolling, you don't need to roll the third person camera!

## UI
Never be rigidly attached to user's head (ruins perception of motion). Use elastic attachment
Sit 2-3 meters in front of eyes
Should not require eye-swivels

## Sound cues

Place sound in 3D environment

## Content

Don't rely on stereoscopic vision. Create interesting lighting with shadows and other depth cues

## Altitude

Altitude strongly effects visual flow of pixel (e.g. low height racecar vs plane) 

## Further reading and references
