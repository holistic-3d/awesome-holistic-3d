# Holistic 3D Reconstruction
A list of papers and resources for holistic 3D reconstruction.

## Related Tutorials and Workshops

 - ECCV 2020 Workshop: [Holistic Scene Structures for 3D Vision](https://holistic-3d.github.io/eccv20/)
 - ICCV 2019 Tutorial: [Holistic 3D Reconstruction: Learning to Reconstruct Holistic 3D Structures from Sensorial Data](https://holistic-3d.github.io/iccv19/)

 
## Datasets

### Scene level

| Datasets      |#Scenes| #Rooms | #Frames | Annotated Structures |
|------------|---------|---------|---------|---------|
| [PlaneRCNN](https://github.com/NVlabs/planercnn)      | ~1,500 | ~1,500 | 100,000 (randomly sampled from 1 million) | planes |
| [Replica](https://github.com/facebookresearch/Replica-Dataset) | 18 | n/a | - | planes |
| [Wireframe](https://github.com/huangkuns/wireframe) | - | - | 5,462 | wireframe (2D) |
| [Wireframe Reconstruction](https://yichaozhou.com/publication/1811learning/) | synthetic and real images | - | - | wireframe (3D) |
| [SUN Primitive](http://3dvision.princeton.edu/projects/2012/SUNprimitive/) | - | - | 785 | cuboid, pyramid, cylinder, sphere, etc. |
| LSUN Room Layout | - | n/a | 5,396 | cuboid layout |
| [PanoContext](http://panocontext.cs.princeton.edu/) | - | n/a | 500 (pano) | cuboid layout |
| [LayoutNet](https://github.com/zouchuhang/LayoutNet) | - | n/a | 1,071 (pano) | cuboid layout |
| [MatterportLayout](https://github.com/ericsujw/Matterport3DLayoutAnnotation) | - | n/a | 2,295 (RGB-D pano) | Manhattan layout |
| [Floor-SP](https://github.com/woodfrog/floor-sp) | 100 | 707 | ~1500 (every scene has a set of RGB-D pano) | floorplan (with non-Manhattan structures) |
| [FloorNet](https://github.com/art-programmer/FloorNet) | ~150 | ~1000 | - | floorplan |
| [Raster-to-Vector](https://github.com/art-programmer/FloorplanTransformation) | 870 | - | - | floorplan |
| [3RScan](https://waldjohannau.github.io/RIO/) | 478 | - | - | objects |
| [Structured3D](https://structured3d-dataset.org/) | 3,500 | 21,835 | 196,515 | pritimitves (points/lines/planes) and relationships, 3D object instance bounding boxes|

### Object level

| Datasets      |#Images | #Categories | #3D models | Annotated Structures | Notes |
|------------|---------|---------|---------|---------|---------|
| [Keypoint-5](http://3dinterpreter.csail.mit.edu/) | 8,649 | 5 | - | keypoints | | 
| [IKEA Keypoints](http://3dinterpreter.csail.mit.edu/) | 759 | | 219 | keypoints | derived from [IKEA 3D](http://ikea.csail.mit.edu/) |
| [ANSI Mechanical Component](https://github.com/lingxiaoli94/SPFN) | - | 504 | 17,197 | plane, sphere, cylinder, cone, etc.| |
| [PartNet](https://cs.stanford.edu/%7Ekaichun/partnet/) | - | 24 | 26,671 | fine-grained, instance-level, and hierarchical 3D parts | derived from ShapeNet |
| [PartNet-Symh](https://github.com/FoggYu/PartNet_symh/) | - | 24 | 22,369 | Symmetry hierarchical 3D parts | derived from PartNet |
| [StructureNet](https://cs.stanford.edu/~kaichun/structurenet/) | - | 6 | - | Symmetry hierarchical 3D parts | derived from PartNet |

### Datasets examples
[PlaneRCNN](https://github.com/NVlabs/planercnn)

<div align="center">
<img src=figures/PlaneRCNN.jpg>
</div>

<div align="center">From left to right: input RGB image, planar segmentation, depthmap</div>

[Wireframe](https://github.com/huangkuns/wireframe)

<div align="center">
<img src=figures/Wireframe.jpg>
</div>

<div align="center">First row: manually labelled line segments. Second row: groundtruth junctions</div>

[Wireframe Reconstruction](https://yichaozhou.com/publication/1811learning/)

<div align="center">
<img src=figures/Wireframe_reconstruction.jpg>
</div>

<div align="center">From left column to right column: input image with groundtruth wireframes, predicted 3D wireframe and alternative view of the same image</div>

[SUN Primitive](http://3dvision.princeton.edu/projects/2012/SUNprimitive/)

<div align="center">
<img src=figures/SUN_Primitive.jpg>
</div>

<div align="center">Yellow: groundtruth, green: correct detection, red: false alarm</div>

LSUN Room Layout

<div align="center">
<img src=figures/LSUN_room.png>
</div>

<div align="center">From left right: input RGB image, room layout (corner-representation), room layout (segmentation-representation)</div>

[PanoContext](http://panocontext.cs.princeton.edu/)

<div align="center">
<img src=figures/PanoContext.jpg>
</div>

<div align="center">From left to right: a single-view panorama, object detection and 3D reconstruction</div>

[LayoutNet](https://github.com/zouchuhang/LayoutNet)

<div align="center">
<img src=figures/LayoutNet.jpg>
</div>

<div align="center">Orange lines: predicted layout, Green lines: groundtruth layout</div>

[Raster-to-Vector](https://github.com/art-programmer/FloorplanTransformation)

<div align="center">
<img src=figures/Raster_to_vector.jpg>
</div>

<div align="center">From left to right: an input floorplan image, reconstructed vector-graphics representation visualized by custom renderer, and a popup 3D model</div>

[Floor-SP](https://github.com/woodfrog/floor-sp)

<div align="center">
<img src=figures/Floor-SP.png>
</div>

<div align="center">From left to right: stitched RGB-D panorama of indoor scenes & top-view point density/normal map, vector-graphics floorplan with non-Manhattan structures</div>

[Structured3D](https://structured3d-dataset.org/)

<div align="center">
<img src=figures/Structured3D.jpg>
</div>

<div align="center">(a) house designs (b) ground truth 3D structure annotations (c) photo-realistic 2D images</div>

[Keypoint-5](http://3dinterpreter.csail.mit.edu/) and [IKEA Keypoints](http://3dinterpreter.csail.mit.edu/)

<div align="center">
<img src=figures/Keypoints_5_input.jpeg>
<img src=figures/Keypoints_5_label.jpeg>
</div>

<div align="center">Left: input image, right: labeled 2D keypoints</div>

[ANSI Mechanical Component](https://github.com/lingxiaoli94/SPFN)

<div align="center">
<img src=figures/ANSI.jpg>
</div>

<div align="center">Up to down: input point cloud and geometric primitives</div>

[PartNet](https://cs.stanford.edu/%7Ekaichun/partnet/)

<div align="center">
<img src=figures/PartNet.jpg>
</div>

<div align="center">From left column to right column:Three levels(from coarse to fine-grained) of segmentation annotations in the hierarchy,for three segmentation tasks</div>

[PartNet-Symh](https://github.com/FoggYu/PartNet_symh/)

<div align="center">
<img src=figures/PartNet_Symh.jpg>
</div>

<div align="center">Odd rows: groundtruth fine-grained segmentation results, even rows: prediction fine-grained segmentation results</div>

## References

### Books

- Y. Ma, S. Soatto, J. Kosecka, and S. S. Sastry. An Invitation to 3D Vision: From Images to Geometric Models. Springer Verlag, 2003.
- R. I. Hartley and A. Zisserman. Multiple View Geometry in Computer Vision. Cambridge University Press, 2000.

### Papers - Scene level

2019
- Y. Zhou, H. Qi, and Y. Ma. NeurVPS: Neural Vanishing Point Scanning via Conic Convolution. In NeurIPS, 2019.  [[project](https://github.com/zhou13/neurvps)]
- Y. Zhou, H. Qi, and Y. Ma. End-to-End Wireframe Parsing. In ICCV, 2019. [[project](https://github.com/zhou13/lcnn)]
- Y. Zhou, H. Qi, Y. Zhai, Q. Sun, Z. Chen, L. Wei, and Y. Ma. Learning to Reconstruct 3D Manhattan Wireframes from a Single Image. In ICCV, 2019. [[project](https://arxiv.org/abs/1905.07482)]
- J. Chen, C. Liu, J. Wu, and Y. Furukawa. Floor-SP: Inverse CAD for Floorplans by Sequential Room-wise Shortest Path. In ICCV, 2019. [[project](https://github.com/woodfrog/floor-sp)]
- J. Wald, A. Avetisyan, N. Navab, F. Tombari, and M. Niessner. RIO: 3D Object Instance Re-Localization in Changing Indoor Environments. In ICCV, 2019. [[project](https://waldjohannau.github.io/RIO/)]
- C. Zou*, J.-W. Su*, C.-H. Peng, A. Colburn, Q. Shan, P. Wonka, H.-K. Chu, and D. Hoiem. 3D Manhattan Room Layout Reconstruction from a Single 360 Image, 2019. arXiv:1910.04099, 2019. [[project](https://github.com/ericsujw/Matterport3DLayoutAnnotation)]
- J. Zheng*, J. Zhang*, J. Li*, R. Tang, S. Gao, and Z. Zhou.  Structured3D: A Large Photo-realistic Dataset for Structured 3D Modeling. arXiv:1908.00222, 2019. [[project](https://structured3d-dataset.org/)]
- C. Liu, K. Kim, J. Gu, Y. Furukawa, and J. Kautz. PlaneRCNN: 3D Plane Detection and Reconstruction from a Single Image. In CVPR, 2019. [[project](https://research.nvidia.com/publication/2019-06_PlaneRCNN)]
- Z. Yu*, J. Zheng*, D. Lian, Z. Zhou, and S. Gao. Single-Image Piece-wise Planar 3D Reconstruction via Associative Embedding. In CVPR, 2019. [[project](https://github.com/svip-lab/PlanarReconstruction)]
- Z. Zhang*, Z. Li*, N. Bi, J. Zheng, J. Wang, K. Huang, W. Luo, Y. Xu, and S. Gao. PPGNet: Learning Point-Pair Graph for Line Segment Detection. In CVPR, 2019. [[project](https://github.com/svip-lab/PPGNet)]

2018
- F. Yang and Z. Zhou. Recovering 3D planes from a single image via convolutional neural networks. In ECCV, 2018. [[project](https://github.com/fuy34/planerecover)]
- H. Zeng, J. Wu, and Y. Furukawa. Neural Procedural Reconstruction for Residential Buildings. In ECCV, 2018. [[paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Huayi_Zeng_Neural_Procedural_Reconstruction_ECCV_2018_paper.pdf)]
- C. Liu*, J. Yu*, and Y. Furukawa. FloorNet: A Unified Framework for Floorplan Reconstruction from 3D Scans. In ECCV 2018. [[project](https://github.com/art-programmer/FloorNet)]
- C. Zou, A. Colburn, Q. Shan, and D. Hoiem. LayoutNet: Reconstructing the 3d room layout from a single RGB image. In CVPR, 2018. [[project](https://github.com/zouchuhang/LayoutNet)]
- C. Liu, J. Yang, D. Ceylan, E. Yumer, and Y. Furukawa. PlaneNet: Piece-wise Planar Reconstruction from a Single RGB Image. In CVPR, 2018. [[project](https://github.com/art-programmer/PlaneNet)]
- K. Huang, Y. Wang, Z. Zhou, T. Ding, S. Gao, and Y. Ma. Learning to parse wireframes in images of man-made environments. In CVPR, 2018. [[project](https://github.com/huangkuns/wireframe)]
- H. Fang, F. Lafarge and M. Desbrun. Planar Shape Detection at Structural Scales. In CVPR, 2018.


2017
- L. Nan and P. Wonka. PolyFit: Polygonal Surface Reconstruction from Point Clouds. In ICCV, 2017.
- C. Liu, J. Wu, P. Kohli, and Y. Furukawa. Raster-to-Vector: Revisiting Floorplan Transformation. In ICCV, 2017. [[project](https://github.com/art-programmer/FloorplanTransformation)]
- C. Lee, V. Badrinarayanan, T. Malisiewicz, and A. Rabinovich. RoomNet: End-to-end room layout estimation. In ICCV, 2017. [[paper](https://arxiv.org/abs/1703.06241)]
- H. Izadinia, Q. Shan, and S. M. Seitz. IM2CAD. In CVPR, 2017. [[project](https://homes.cs.washington.edu/~izadinia/im2cad.html)]
- E. Wijmans and Y. Furukawa. Exploiting 2D Floorplan for Building-scale Panorama RGBD Alignment. In CVPR, 2017. [[project](https://cvpr17.wijmans.xyz/)]
- T. Kelly, J. Femiani, P. Wonka, and N. Mitra. BigSUR: Large-scale Structured Urban Reconstruction. In SIGGRAPH Asia, 2017.

2016
- M. Li, P. Wonka, and L. Nan. Manhattan-world Urban Reconstruction from Point Clouds. In ECCV, 2016.
- C. Zhu, Z. Zhou, Z. Xing, Y. Dong, Y. Ma, and J. Yu. Robust Plane-based Calibration of Multiple Non-Overlapping Cameras. In 3DV, 2016. [[paper](https://faculty.ist.psu.edu/zzhou/paper/3dv16-calibration.pdf)]
- C. Liu, P. Kohli, and Y. Furukawa. Layered Scene Decomposition via the Occlusion-CRF. In CVPR, 2016. [[project](https://sites.wustl.edu/chenliu/layered-scene/)]
- S. Dasgupta, K. Fang, K. Chen, and S. Savarese. Delay: Robust spatial layout estimation for cluttered indoor scenes. In CVPR, 2016. [[paper](http://cvgl.stanford.edu/papers/delay-robust-spatial.pdf)]
- S. Oesau, F. Lafarge and P. Alliez. Planar Shape Detection and Regularization in Tandem. Computer Graphics Forum, 2016.

2015
- S. Ikehata, H. Yan, and Y. Furukawa. Structured Indoor Modeling. In ICCV, 2015. [[paper](https://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Ikehata_Structured_Indoor_Modeling_ICCV_2015_paper.pdf)]
- O. Haines and A. Calway. Recognising planes in a single image. IEEE TPAMI, 2015. [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6987324)]
- A. Monszpart, N. Mellado, G. J. Brostow, and N. J. Mitra. RAPTER: Rebuilding Man-made Scenes with Regular Arrangements of Planes. In SIGGRAPH, 2015. [[paper](https://geometry.cs.ucl.ac.uk/projects/2015/regular-arrangements-of-planes/paper_docs/RAPter_MonszpartEtAl_SIGGRAPH_2015.pdf)]

2014
- D. F. Fouhey, A. Gupta, and M. Hebert. Unfolding an indoor origami world. In ECCV, 2014. [[paper](https://ri.cmu.edu/pub_files/2014/7/dfouhey_origami.pdf)]
- R. Cabral and Y. Furukawa. Piecewise Planar and Compact Floorplan Reconstruction from Images. In CVPR 2014. [[paper](https://www.andrew.cmu.edu/user/rcabral/CabralFurukawaCVPR2014.pdf)]
- D. Ceylan, N. J. Mitra, Y. Zheng, M. Pauly. Coupled Structure-from-Motion and 3D Symmetry Detection for Urban Facades. ACM Transactions on Graphics, 2014.

2013
- S. Ramalingam and M. Brand. Lifting 3D manhattan lines from a single image. In ICCV, 2013. [[paper](https://www.merl.com/publications/docs/TR2013-110.pdf)]
- S. Ramalingam, J. K. Pillai, A. Jain, and Y. Taguchi. Manhattan junction catalogue for spatial reasoning of indoor scenes. In CVPR, 2013. [[paper](https://ieeexplore.ieee.org/document/6619238)]
- Z. Zhou, H. Jin, and Y. Ma. Plane-Based Content-Preserving Warps for Video Stabilization. In CVPR, 2013. [[paper](https://www.cv-foundation.org/openaccess/content_cvpr_2013/papers/Zhou_Plane-Based_Content_Preserving_2013_CVPR_paper.pdf)]
- N. J. Mitra, M. Pauly, M. Wand, and D. Ceylan. Symmetry in 3D Geometry: Extraction and Applications. Computer Graphics Forum, 2013.

2012
- J. Xiao, B. C. Russell, and A. Torralba. Localizing 3d cuboids in single-view images. In NIPS, 2012. [[paper](http://papers.nips.cc/paper/4842-localizing-3d-cuboids-in-single-view-images.pdf)]
- J. Xiao and Y. Furukawa. Reconstructing the World's Museums. In ECCV, 2012. [[paper](https://vision.princeton.edu/projects/2012/museum/paper.pdf)]
- Z. Zhou, H. Jin, and Y. Ma. Robust Plane-Based Structure From Motion. In CVPR, 2012. [[paper](https://faculty.ist.psu.edu/zzhou/paper/1442.pdf)]
- A. Cohen, C. Zach, S. N. Sinha and M. Pollefeys. Discovering and exploiting 3D symmetries in structure from motion. In CVPR, 2012.
- C. A. Vanegas, D. G. Aliaga, and B. Benes. Automatic Extraction of Manhattan-World Building Masses from 3D Laser Range Scans. IEEE TVCG, 2012.

2011
- H. Mobahi, Z. Zhou, A. Y. Yang, and Y. Ma. Holistic Reconstruction of Urban Structures from Low-rank Textures. In ICCV-3dRR, 2011. [[paper](https://ieeexplore.ieee.org/abstract/document/6130297)]
- Z. Zhang, X. Liang, and Y. Ma. Unwrapping Low-rank Textures on Generalized Cylindrical Surfaces. In ICCV, 2011. [[paper](https://ieeexplore.ieee.org/document/6126388)]
- A. Flint, D. W. Murray, and I. Reid. Manhattan scene understanding using monocular, stereo, and 3D features. In ICCV, 2011. [[paper](https://ieeexplore.ieee.org/document/6126501)]
- C. Wu, J.-M. Frahm, and M. Pollefeys. Repetition-based dense single-view reconstruction. In CVPR, 2011. [[paper](https://inf.ethz.ch/personal/pomarc/pubs/WuCVPR11.pdf)]
- A. Elqursh and A. M. Elgammal. Line-based relative pose estimation. In CVPR, 2011. [[paper](https://www.cs.rutgers.edu/~elgammal/pub/CVPR11_Elqursh.pdf)]
- Z. Zhang, Y. Matsushita, and Y. Ma. Camera Calibration with Lens Distortion from Low-rank Textures. In CVPR, 2011. [[paper](http://people.csail.mit.edu/zhangzd/papers/calibration_cvpr11.pdf)]

2010 and before
- D. Gallup, J.-M. Frahm, and M. Pollefeys. Piecewise Planar and Non-Planar Stereo for Urban Scene Reconstruction. In CVPR, 2010. [[paper](https://ieeexplore.ieee.org/document/5539804)]
- Y. Furukawa, B. Curless, S. M. Seitz and R. Szeliski. Reconstructing Building Interiors from Images. In ICCV, 2009. [[paper](http://grail.cs.washington.edu/wp-content/uploads/2016/09/furukawa2009rbi.pdf)]
- V. Hedau, D. Hoiem, and D. A. Forsyth. Recovering the spatial layout of cluttered rooms. In ICCV, 2009. [[paper](http://dhoiem.cs.illinois.edu/publications/iccv2009_hedau_indoor.pdf)]
- Y. Furukawa, B. Curless, S. M. Seitz, and R. Szeliski. Manhattan-world stereo. In CVPR, 2009. [[paper](http://grail.cs.washington.edu/projects/manhattan/manhattan.pdf)]
- D.C. Lee, M. Hebert, and T. Kanade. Geometric Reasoning for Single Image Structure Recovery. In CVPR, 2009. [[paper](https://www.ri.cmu.edu/pub_files/2009/6/cvpr09lee.pdf)]
- G. Schindler, P. Krishnamurthy, R. Lublinerman, Y. Liu, and F. Dellaert. Detecting and Matching Repeated Patterns for Automatic Geo-tagging in Urban Environments. In CVPR, 2008. [[paper](https://www.ri.cmu.edu/pub_files/pub4/schindler_grant_2008_1/schindler_grant_2008_1.pdf)]
- B. Micusik, H. Wildenauer, and J. Kosecka. Detection and matching of rectilinear structures. In CVPR, 2008. [[paper](https://ieeexplore.ieee.org/document/4587488)]
- D. Hoiem, A. A. Efros, and M. Hebert. Recovering surface layout from an image. IJCV, 2007. [[paper](http://dhoiem.cs.illinois.edu/publications/hoiem_ijcv2007SurfaceLayout.pdf)]
- G. Schindler, P. Krishnamurthy, and F. Dellaert. Line-Based Structure From Motion for Urban Environments. In 3DPVT, 2006. [[paper](https://www.cc.gatech.edu/projects/4d-cities/dhtml/pubs/Schindler06-3dpvt.pdf)]
- J. M. Coughlan and A. L. Yuille. Manhattan world: Orientation and outlier detection by bayesian inference. Neural Computation, 2003. [[paper](https://ieeexplore.ieee.org/document/6790299)]
- A. Bartoli and P. Sturm. Constrained structure and motion from multiple uncalibrated views of a piecewise planar scene. IJCV, 2003. [[paper](https://link.springer.com/article/10.1023/A:1022318524906)]
- J. Kosecka, and W. Zhang. Video Compass. In ECCV, 2002. [[paper](https://link.springer.com/chapter/10.1007/3-540-47979-1_32)]
- A. P. Witkin and J. M. Tenenbaum. On the role of structure in vision. In J. Beck, B. Hope, and A. Rosenfeld, editors, Human and Machine Vision, pages 481–543. Academic Press, 1983. [[paper](http://cvcl.mit.edu/SUNSeminar/BarenholtzTarr_2007.pdf)]

### Papers - Object level

2019
- K. Mo, P. Guerrero, L. Yi, H. Su, P. Wonka, N. J. Mitra, and L. Guibas. StructureNet: Hierarchical Graph Networks for 3D Shape Generation. In SIGGRAPH Asia, 2019. [[project](https://cs.stanford.edu/~kaichun/structurenet/)]
- C. Sun, Q. Zou, X. Tong, and Y. Liu. Learning Adaptive Hierarchical Cuboid Abstractions of 3D Shape Collections. In SIGGRAPH Asia, 2019. [[project](https://isunchy.github.io/projects/cuboid_abstraction.html)]
- D. Paschalidou, A. O. Ulusoy, and A. Geiger. Superquadrics Revisited: Learning 3D Shape Parsing beyond Cuboids. In CVPR, 2019. [[paper](https://arxiv.org/abs/1904.09970)]
- L. Li, M. Sung, A. Dubrovina, L. Yi, and L. Guibas. Supervised Fitting of Geometric Primitives to 3D Point Clouds. In CVPR, 2019. [[paper](https://arxiv.org/abs/1811.08988)]

2018
- J. Wu, T. Xue, J. J. Lim, Y. Tian, J. B. Tenenbaum, A. Torralba, and W. T. Freeman. 3d interpreter networks for viewer centered wireframe modeling. IJCV, 2018. [[project](http://3dinterpreter.csail.mit.edu/)]
- C. Niu, J. Li, and K. Xu. Im2struct: Recovering 3d shape structure from a single RGB image. In CVPR, 2018. [[code](https://github.com/chengjieniu/Im2Struct)]

2017
- C. Zou, E. Yumer, J. Yang, D. Ceylan, and D. Hoiem. 3D-PRNN: Generating Shape Primitives with Recurrent Neural Networks. In ICCV, 2017. [[paper](http://openaccess.thecvf.com/content_ICCV_2017/papers/Zou_3D-PRNN_Generating_Shape_ICCV_2017_paper.pdf)]
- S. Tulsiani, H. Su, L. J. Guibas, A. A. Efros, and J. Malik. Learning Shape Abstractions by Assembling Volumetric Primitives. In CVPR, 2017. [[project](https://shubhtuls.github.io/volumetricPrimitives/)]

2013
- L. Yang, J. Liu, and X. Tang. Complex 3D General Object Reconstruction from Line Drawings. In ICCV, 2013. [[paper](https://www.cv-foundation.org/openaccess/content_iccv_2013/papers/Yang_Complex_3D_General_2013_ICCV_paper.pdf)]
- N. J. Mitra, M. Wand, H. Zhang, D. Cohen-Or, and M. Bokeloh. Structure-Aware Shape Processing. In EUROGRAPHICS, 2013. [[project](http://vecg.cs.ucl.ac.uk/Projects/SmartGeometry/structure_survey/structureSurvey_eg13.html)]

2012
- S. N. Sinha, K. Ramnath, and R. Szeliski. Detecting and Reconstructing 3D Mirror Symmetric Objects. In ECCV, 2012.
- T. Xue, Y. Li, J. Liu, and X. Tang. Example-Based 3D Object Reconstruction from Line Drawings. In CVPR, 2012. [[paper](http://mmlab.ie.cuhk.edu.hk/pdf/XueCVPR12.pdf)]

2011
- Y. Li, X. Wu, Y. Chrysathou, A. Sharf, D. Cohen-Or, and N. J. Mitra. GlobFit: Consistently Fitting Primitives by Discovering Global Relations. In SIGGRAPH, 2011. [[project](http://vecg.cs.ucl.ac.uk/Projects/SmartGeometry/globFit/globFit_sigg11.html)]

2010 and before
- T. Xue, J. Liu, and X. Tang. Object Cut: Complex 3D object reconstruction through line drawing separation. In CVPR 2010. [[paper](http://mmlab.ie.cuhk.edu.hk/pdf/XueCVPR10.pdf)]
- M. Bokeloh, A. Berner, M. Wand, H. P. Seidel, and A. Schilling. Symmetry Detection Using Feature Lines. In EUROGRAPHICS, 2009.
- L. Cao, J. Liu, and X. Tang. What the Back of the Object Looks Like: 3D Reconstruction from Line Drawings without Hidden Lines. PAMI 2008. [[paper](http://mmlab.ie.cuhk.edu.hk/pdf/CaoTPAMI08.pdf)]
- M. Pauly, N. J. Mitra, J. Wallner, H. Pottmann, and L. J. Guibas. Discovering Structural Regularity in 3D Geometry. In SIGGRAPH, 2008. [[paper](https://lgg.epfl.ch/publications/2008/pauly_2008_DSR.pdf)]
- Y. Wang, Y. Chen, J. Liu, and X. Tang. 3D Reconstruction of Curved Objects from Single 2D Line Drawings. In CVPR, 2008. [[paper](http://mmlab.ie.cuhk.edu.hk/pdf/yzWangCVPR08.pdf)]
- Y. Chen, J. Liu, and X. Tang. A Divide-and-Conquer Approach to 3D Object Reconstruction from Line Drawings. In ICCV 2007. [[paper](http://mmlab.ie.cuhk.edu.hk/pdf/ChenICCV07.pdf)]
- N. J. Mitra, L. Guibas, and M. Pauly. Partial and Approximate Symmetry Detection for 3D Geometry. ACM ToG, 2006. [[paper]()]
- J. Malik. Interpreting line drawings of curved objects. IJCV, 1987. [[paper](https://people.eecs.berkeley.edu/~malik/papers/malik87.pdf)]
- K. Sugihara. Mathematical structures of line drawings of polyhedrons-toward man-machine communication by means of line drawings. IEEE TPAMI, 1982. [[paper](https://ieeexplore.ieee.org/document/4767289)]
