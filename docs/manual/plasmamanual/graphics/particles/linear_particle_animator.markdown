The linear particle animator give particles the ability to move.  It adds an integration step which allows particles to have some physically based motion.  The [LinearParticleAnimator](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/linearparticleanimator.markdown) component is required to generate particles and and to move them.

(NOTE)**Where to set particle velocity?** Properties relating to velocity are not found on the `LinearParticleAnimator`, but are instead on the emitter component.  The reason for this property placement is that all properties on the [emitter](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/graphics/particles/emitters.markdown) component are applied when a particle is created, whereas the properties from `LinearParticleAnimator` are applied every frame.

 # Forces
Both Force  and RandomForce  are used to apply forces to a particle.  The force will effect the velocity, which in turn effects the position of each particle.  If the RandomForce  defines the half-vector for a bounding box, then the random component of this frames Force is confined to this box.


 # Growth
The Growth  property can change the size of particles over time.  Set Growth  to a positive number to make it grow, and a negative number to make it shrink.



![ParticleSystems_Growth](https://raw.githubusercontent.com/PlasmaEngine/PlasmaDocs/master/media/46666.gif)


 # Related Material
 ## Manual
- [Physics Effects and Regions](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/plasmamanual/physics/physicseffectsandregions.markdown)

 ## Code Reference
- [SpriteParticleSystem](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/plasma_editor_documentation/code_reference/class_reference/spriteparticlesystem.markdown)
- [LinearParticleAnimator](https://github.com/PlasmaEngine/PlasmaDocs/blob/master/code_reference/class_reference/linearparticleanimator.markdown) 

 