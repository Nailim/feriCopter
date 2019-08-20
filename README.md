# feriCopter

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

## Parts

- Motors (Brushless, 2300 KV, ~30g):
  - 2x [Clockwise](https://hobbyking.com/en_us/brushless-motor-d2205-2300kv-cw.html)
  - 2x [Counter-Clockwise](https://hobbyking.com/en_us/brushless-motor-d2205-2300kv-ccw.html)
- 4x Electronic Speed Controller (~12 A): [Multistar 32bit](https://hobbyking.com/en_us/multistar-32bit-12a-0-lite.html) or [Multistar Mini](https://hobbyking.com/en_us/mini-blheli-multi-12a-opto.html)
- 1x [Power Distribution Board](https://hobbyking.com/en_us/pdb-xt60-w-bec-5v-12v.html)
- 4x [Propeller (2x Clockwise, 2x Counter-Clockwise, ~10 cm)](https://hobbyking.com/en_us/dys-t4045-r-4x4-5-cw-ccw-pair-2-pairs-pack-red.html)
- 2x [Gold Connectors (2mm, 2x 10 pairs)](https://hobbyking.com/en_us/2mm-gold-connectors-10-pairs-20pc-1.html)
- 1x [Radio Control System (Controller)](https://hobbyking.com/en_us/i6s-afhds-2a-white-mode2-6ch-radio-with-colour-box.html)
- 1x LiPo Battery (14.8V, 45C, 1300 mAh, 4S1P)
- 1x Velcro (Battery attachment)
- 1x [LiPo Charger](https://hobbyking.com/en_us/turnigy-e3-compact-2s-3s-lipo-charger-100-240v-us-plug.html)
- 1x [USB Simulator Cable (Controller PC Connection)](https://hobbyking.com/en_us/usb-simulator-cable-xtr-aerofly-fms.html)
- 1x [LiPo Bag](https://hobbyking.com/en_us/lithium-polymer-charge-pack-18x22cm-sack.html)
