# How can I build VR experience for my dog? A bird? My pet squid ...

Building an adequate virtual experience for non-humans requires a strong understanding of the physical, 
perceptual and neurological systems that create their senses. 
This page details a few interesting case studies that have perceptual systems that have unusual differences from our human senses.


## Which way is North?

Birds appear to use their eyes to sense magnetic compass orientation. The "Cry4" protein is sensitive to Earth's weak magnetic fields. The exact mechanism is still under active research.

https://www.sciencenews.org/article/birds-get-their-internal-compass-newly-id-eye-protein

If the Cry4 protein modulates the brightness in part of the eye, it may be possible to mimic this effect when rendering the scene.
Alternatively thetrue  Earth's magnetic field in a lab can be shielded and instead a magnetic field can be "displayed" 
using a local set of electromagnets.

## Echolocation - just as hard for VR as vision?

Bats and dolphins are examples of animals that can measure distances and shapes using acoustic reflections of an emitted pulse or click.
Dolphins emit high frequency ultrasound (40 to 150 KHz) to measure distance, relative position, shape, direction and internal 
structure of nearby objects.

Most humans do not use echolocation to construct a 3D view of their immediate surroundings. There are a few exceptions however,
including Ben Underwood who could use echolocation to ride a bicycle and avoid large obstacles.
https://en.wikipedia.org/wiki/Human_echolocation

A VR experience that supported echolocation would need to reproduce accurately model the reflection of the emitted sound.
This would be challenging to implement for dolphins because dolphins modify the subsequent emitted ultrasound pulses
based on the previous echos. Thus a VR experience for a dolphin would need to sample the emitted pulse and create an accurate an accurate
reflected sound based on the materials, position and orientation of the objects in the scene.

## Is a red green and blue display sufficient?

Not for pollen-gathering insects! Todo talk about flowers and leaves in ultraviolet
