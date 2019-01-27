# feriCopterV1
Model and 3D printing resources for student project.

### What is it?
Specialized quadcopter frame designed around STM32F3Discovery development board with ease of assembly in mind.
Assembly video for the project can be found on [YouTube](https://youtu.be/s-TGnOwG-w0).

## Content
- `blender/` - 3D model of the frame
- `meta/` - FreeCAD project for the documentation/assembly handout
- `stl/` - 3D printer ready STL files
- `feriCopter_assembly.pdf` - documentation/assembly handout

## Board Compatibility

Currently feriCopter supports the following boards:
- STM32F3DISCOVERY with `STM32F303VC` MCU
- STM32F411EDISCOVERY with `STM32F411VE` MCU

Frame compatibility for both targets is in the same Blender project, with the only change being the toggle of following modifiers on `Frame` object:
- `Boolean_cutout_pins_1_f3`
- `Boolean_cutout_pins_1_f411`

STL files are exported and corrected for both variants.

## Notes

Blender project contains base parts of the frame, however they were merged into `Frame`/`MotorMount` objects and further modified. Base objects are there for reference when needed, but should not be used for further editing.
