# Animals and VR

Building an adequate virtual experience for non-humans requires a strong understanding of the physical, 
perceptual and neurological systems that create their senses. 
This page details a few interesting case studies that have perceptual systems that have unusual differences from our human senses.


## Which way is North?

Birds appear to use their eyes to sense magnetic compass orientation. The "Cry4" protein is sensitive to Earth's weak magnetic fields. The exact mechanism is still under active research.

If the Cry4 protein modulates the brightness in part of a bird's eye, it may be possible to mimic this effect when rendering the scene by changing the displayed color depending on the bird's head orientation.

Alternatively the true Earth's magnetic field in a lab can be shielded and instead a magnetic field can be created
using a set of electromagnets.

## Echolocation - just as hard for VR as vision?

Bats and dolphins are examples of animals that can measure distances and shapes using acoustic reflections of an emitted pulse or click.
Dolphins emit high frequency ultrasound (40 to 150 KHz) to measure distance, relative position, shape, direction and internal 
structure of nearby objects.

Most humans do not use echolocation to construct a 3D view of their immediate surroundings. There are a few exceptions however,
including Ben Underwood who could use echolocation to ride a bicycle and avoid large obstacles.
https://en.wikipedia.org/wiki/Human_echolocation

A VR experience that supported echolocation would need to reproduce accurately model the reflection of the emitted sound.
This would be challenging to implement for dolphins because dolphins modify the subsequent emitted ultrasound pulses
based on the previous echos. Thus a VR experience for a dolphin would need to sample the emitted pulse, create an accurate 
model of the reflected pulse based on the materials, relative position and orientation of the object(s) in the scene, and render the sound at the correct numer of milliseconds after the original pulse was emitted.

## When is a red, green, and blue display insufficient?

This would be insufficient for pollen-gathering insects! Though honey bees for example, are also trichomatic like our eyes, the sensitivity of their 3 different photoreceptors extends into the high frequency ultraviolet (UV), which is not perceived by human eyes. 

Flowers use ultraviolet absorbing pigments to guide pollenators towards the pollen. As an example, here's the same petals when observed under UV compared to the same plant as observed in the human part of the visible spectrum

![FlowerVisibleVsUVspectrum](http://howplantswork.files.wordpress.com/2008/11/merge.jpg?w=250&h=423&zoom=2)

(Image attribution: howplantswork.wordpress.com)

Pythons, boas, rattlesnakes and pit viper snakes can locate and track prey using infrared signature.

## Further reading and references

https://www.sciencenews.org/article/birds-get-their-internal-compass-newly-id-eye-protein

A. Pinzon-Rodriguez, S. Bensch and R. Muheim. Expression patterns of cryptochrome genes in avian retina suggest involvement of Cry4 in light-dependent magnetoreception (cryptochrome expression in zebra finches). Journal of the Royal Society Interface. Published online March 28, 2018. doi: 10.1098/rsif.2018.0058

A. Günther et al. Double-cone localization and seasonal expression pattern suggest a role in magnetoreception for European robin cryptochrome 4. Current Biology. Vol. 28. January 22, 2018, p. 211. doi: 10.1016/j.cub.2017.12.003

https://howplantswork.wordpress.com/2008/11/30/flowers-what-you-see-versus-what-the-bees-see/
