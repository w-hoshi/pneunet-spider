# Soft Robotic Spider

An eight legged soft robot with pneumatic bending legs and a variable stiffness body. The legs are PneuNet actuators cast from Ecoflex 00-30 with a fabric strain limiting layer. The body holds a laminar jamming pouch (TPE filled with sugar and paper sheets) that stiffens under vacuum, so the robot can stay compliant while crawling and lock up when it needs to hold a load.

Video of crawling and grasping: https://youtu.be/Sf3-M5LHtmc

## Results

- Crawl speed on a flat wood track: about 0.99 mm/s over five runs.
- Handles loose terrain (rice covered track) without trouble. Gets stuck in narrow passages where walls fold the legs under the body.
- Grasps by curling all eight legs around an object. Lifted up to 200 g.
- Modeling: fit a constant curvature model to the leg backbone at three pressures. The fit is tight at low pressure, still usable at medium, and RMS error roughly doubles at high pressure where the base bends more than the tip. A piecewise constant curvature model would be the next step.

## Repo contents

- `CAD/` STL files for the leg and body molds.

## Fabrication notes

Legs are cast in a 3D printed two part mold, then bonded to the strain limiting layer with a thin coat of uncured Ecoflex. Inspect the chambers for tears after demolding and again after bonding. The jamming pouch uses an "air mattress" column pattern so the sugar stays distributed along the length instead of pooling at one end.

## Credits

Course project. I designed the final leg geometry, made the molds in SolidWorks, and manufactured the legs. Several geometries were tested for inflation behavior before landing on this one. The variable stiffness components were developed by Erik Rodriguez-Canales.

## References

- Ilievski et al., Soft robotics for chemists, Angew. Chem. Int. Ed., 2011.
- Shepherd et al., Multigait soft robot, PNAS, 2011.
- Brown et al., Universal robotic gripper based on the jamming of granular material, PNAS, 2010.
- Amend et al., A positive pressure universal gripper based on the jamming of granular material, IEEE T-RO, 2012.
