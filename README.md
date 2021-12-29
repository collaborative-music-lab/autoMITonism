# autoMITonism

This is a fork of Johan Eriksson's excellent Automatonism library for PureData:
https://www.automatonism.com
The purpose of this fork is to enable for community improvements to the existing library, notably fleshing out parameter receives for working with external controllers.

In addition, the possibility exists to modify the library to improve parameter storage, and potentially remove the requirement for the core automonatism modules to be in a strict folder hierarchy.

### what is and isn't being changed
* new modules are not being added to main automatonism interface. e.g. to use them you will have to create them yourself and give them a unique instance number
* new modules *should* use state and preset management correctly
* parameter nudging is not being implemented for new modules

## Changes

* 16steps - extension to 8-steps, with receives to set sequencer values remotely
* pd303 - now receives load messages to directly set sequence presets
* wave-sampler - load a sample and flexible change loop points (even preserving pitch, kinda)
* cartesian - cartesian sequencer (similar to make noise rené or NE mutatis digitalis)
