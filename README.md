# Holistic 3D Reconstruction
A list of papers and resources for holistic 3D reconstruction.

## Related Tutorials and Courses

 - ICCV 2019 Tutorial: [Holistic 3D Reconstruction: Learning to Reconstruct Holistic 3D Structures from Sensorial Data](https://holistic-3d.github.io/iccv19/)
 
## Datasets

### Scene level

| Datasets      |#Scenes| #Rooms | #Frames | Annotated Structures |
|------------|---------|---------|---------|---------|
| [PlaneRCNN](https://github.com/NVlabs/planercnn)      | - | - | 100,000 | planes |
| [Wireframe](https://github.com/huangkuns/wireframe) | - | - | 5,462 | wireframe (2D) |
| [SUN Primitive](http://3dvision.princeton.edu/projects/2012/SUNprimitive/) | - | - | 785 | cuboids, pyramids, cylinders, spheres, etc. |
| LSUN Room Layout | - | n/a | 5,396 | cuboid layout |
| [PanoContext](http://panocontext.cs.princeton.edu/) | - | n/a | 500 (pano) | cuboid layout |
| [LayoutNet](https://github.com/zouchuhang/LayoutNet) | - | n/a | 1,071 (pano) | cuboid layout |
| MatterportLayout | - | n/a | 2,295 (RGB-D pano) | Manhattan layout |
| [Raster-to-Vector](https://github.com/art-programmer/FloorplanTransformation) | 870 | - | - | floorplan |
| [Structured3D](https://structured3d-dataset.org/) | 3,500 | 21,835 | 196,515 | "pritimitve + relationship"|

### Object level

| Datasets      |#Images | #Categories | #3D models | Annotated Structures | Notes |
|------------|---------|---------|---------|---------|---------|
| [Keypoint-5](http://3dinterpreter.csail.mit.edu/) | 8,649 | 5 | - | keypoints | | 
| [IKEA Keypoints](http://3dinterpreter.csail.mit.edu/) | 759 | | 219 | keypoints | derived from [IKEA 3D](http://ikea.csail.mit.edu/) |
| [ANSI Mechanical Component](https://github.com/lingxiaoli94/SPFN) | - | 504 | 17,197 | plane, sphere, cylinder, cone, etc.| |
| [PartNet](https://cs.stanford.edu/%7Ekaichun/partnet/) | - | 24 | 26,671 | fine-grained, instance-level, and hierarchical 3D parts | derived from ShapeNet |
| [PartNet-Symh](https://github.com/kevin-kaixu/partnet-symh) | - | 24 | 22,699 | Symmetry hierarchical 3D parts | derived from ShapeNet |

## References

### Books

### Papers
