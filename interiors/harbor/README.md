# Project Harbor interiors

Original interior scenes for Project Harbor. Each `.blend` is the editable Blender source and the matching `.glb` is the game export. Coordinates are metric (one unit per metre).

| Scene | Room footprint | Height |
| --- | --- | --- |
| Customs Exchange Cafe | 17 × 13 m | 4.15 m |
| Atlantic Repair | 19.5 × 26 m | 6.15 m |
| Alderwash Lodge | 28 × 20 m | 5.4 m |

The room dimensions describe the architectural shell; fixtures and exterior trim may extend beyond it. Game-specific collision and light definitions are maintained in the Project Harbor repository alongside its interior build script.

Floor slabs and roofs were generated with [Building Tools](https://github.com/ranjian0/building_tools) at commit `0216534645b15b3f8aac0bd1d7e6674e2972b9b3` (MIT license), using its floorplan and roof generators. The cafe has a flat roof; the repair shop and lodge have box gable roofs.
