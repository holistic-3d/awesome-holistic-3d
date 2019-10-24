# Holistic 3D Reconstruction
A list of papers and resources for holistic 3D reconstruction.

## Related Tutorials and Courses

 - ICCV 2019 Tutorial: [Holistic 3D Reconstruction: Learning to Reconstruct Holistic 3D Structures from Sensorial Data](https://holistic-3d.github.io/iccv19/)
 
## Datasets

### Scene level

| Datasets      |#Scenes| #Rooms | #Frames | Annotated Structures |
|------------|---------|---------|---------|---------|
| [PlaneRCNN](https://github.com/NVlabs/planercnn)      | ~1,500 | ~1,500 | 100,000 (randomly sampled from 1 million) | planes |
| [Wireframe](https://github.com/huangkuns/wireframe) | - | - | 5,462 | wireframe (2D) |
| [Wireframe Reconstruction](https://yichaozhou.com/publication/1811learning/) | synthetic and real images | - | - | wireframe (3D) |
| [SUN Primitive](http://3dvision.princeton.edu/projects/2012/SUNprimitive/) | - | - | 785 | cuboid, pyramid, cylinder, sphere, etc. |
| [LSUN Room Layout](https://github.com/leVirve/lsun-room) | - | n/a | 5,396 | cuboid layout |
| [PanoContext](http://panocontext.cs.princeton.edu/) | - | n/a | 500 (pano) | cuboid layout |
| [LayoutNet](https://github.com/zouchuhang/LayoutNet) | - | n/a | 1,071 (pano) | cuboid layout |
| MatterportLayout | - | n/a | 2,295 (RGB-D pano) | Manhattan layout |
| [Raster-to-Vector](https://github.com/art-programmer/FloorplanTransformation) | 870 | - | - | floorplan |
| [Structured3D](https://structured3d-dataset.org/) | 3,500 | 21,835 | 196,515 | pritimitves (points/lines/planes) and relationships|
| [Replica](https://github.com/facebookresearch/Replica-Dataset) | 18 | n/a | - | planes |
| [RIO](https://waldjohannau.github.io/RIO/) | - | - | - | objects |
| [FloorNet](https://github.com/art-programmer/FloorNet) | ~150 | ~1000 | - | floorplan |

### Object level

| Datasets      |#Images | #Categories | #3D models | Annotated Structures | Notes |
|------------|---------|---------|---------|---------|---------|
| [Keypoint-5](http://3dinterpreter.csail.mit.edu/) | 8,649 | 5 | - | keypoints | | 
| [IKEA Keypoints](http://3dinterpreter.csail.mit.edu/) | 759 | | 219 | keypoints | derived from [IKEA 3D](http://ikea.csail.mit.edu/) |
| [ANSI Mechanical Component](https://github.com/lingxiaoli94/SPFN) | - | 504 | 17,197 | plane, sphere, cylinder, cone, etc.| |
| [PartNet](https://cs.stanford.edu/%7Ekaichun/partnet/) | - | 24 | 26,671 | fine-grained, instance-level, and hierarchical 3D parts | derived from ShapeNet |
| [PartNet-Symh](https://github.com/kevin-kaixu/partnet-symh) | - | 24 | 22,699 | Symmetry hierarchical 3D parts | derived from ShapeNet |

### Datasets examples
[PlaneRCNN](https://github.com/NVlabs/planercnn)

<div align="center">
<img src=figures/PlaneRCNN.jpg>
</div>

<div align="center">From left to right:input RGB image,planar segmentation,depthmap</div>

[Wireframe](https://github.com/huangkuns/wireframe)

<div align="center">
<img src=figures/Wireframe.jpg>
</div>

<div align="center">First row:manually labelled line segments. Second row:groundtruth junctions</div>

[Wireframe Reconstruction](https://yichaozhou.com/publication/1811learning/)

<div align="center">
<img src=figures/Wireframe_reconstruction.jpg>
</div>

<div align="center">From left column to right column:input image with groundtruth wireframes,predicted 3D wireframe and alternative view of the same image</div>

[SUN Primitive](http://3dvision.princeton.edu/projects/2012/SUNprimitive/)

<div align="center">
<img src=figures/SUN_Primitive.jpg>
</div>

<div align="center">Yellow:groundtruth, green:correct detection, red:false alarm</div>

[LSUN Room Layout](https://github.com/leVirve/lsun-room)

<div align="center">
<img src=figures/LSUN_room.jpg>
</div>

<div align="center">Left:input RGB image,right:groundtruth room layout</div>

[PanoContext](http://panocontext.cs.princeton.edu/)

<div align="center">
<img src=figures/PanoContext.jpg>
</div>

<div align="center">From left to right:a single-view panorama,object detection and 3D reconstruction</div>

[LayoutNet](https://github.com/zouchuhang/LayoutNet)

<div align="center">
<img src=figures/LayoutNet.jpg>
</div>

<div align="center">Orange lines:predicted layout,Green lines:groundtruth layout</div>

[Raster-to-Vector](https://github.com/art-programmer/FloorplanTransformation)

<div align="center">
<img src=figures/Raster_to_vector.jpg>
</div>

<div align="center">From left to right:an input floorplan image, reconstructed vector-graphics representation visualized by custom renderer, and a popup 3D model</div>

[Structured3D](https://structured3d-dataset.org/)

<div align="center">
<img src=figures/Structured3D.jpg>
</div>

<div align="center">(a)house designs (b)ground truth 3D structure annotations (c)photo-realistic 2D images</div>

[Keypoint-5](http://3dinterpreter.csail.mit.edu/) and [IKEA Keypoints](http://3dinterpreter.csail.mit.edu/)

<div align="center">
<img src=figures/Keypoints_5_input.jpeg>
<img src=figures/Keypoints_5_label.jpeg>
</div>

<div align="center">Left:input image,right:labeled 2D keypoints</div>

[ANSI Mechanical Component](https://github.com/lingxiaoli94/SPFN)

<div align="center">
<img src=figures/ANSI.jpg>
</div>

<div align="center">Up to down:input point cloud and geometric primitives</div>

[PartNet](https://cs.stanford.edu/%7Ekaichun/partnet/)

<div align="center">
<img src=figures/PartNet.jpg>
</div>

<div align="center">From left column to right column:Three levels(from coarse to fine-grained) of segmentation annotations in the hierarchy,for three segmentation tasks</div>

[PartNet-Symh](https://github.com/kevin-kaixu/partnet-symh)

<div align="center">
<img src=figures/PartNet_Symh.jpg>
</div>

<div align="center">Odd rows:groundtruth fine-grained segmentation results,even rows:prediction fine-grained segmentation rows</div>

## References

### Books

- Y. Ma, S. Soatto, J. Kosecka, and S. S. Sastry. An Invitation to 3D Vision: From Images to Geometric Models. Springer Verlag, 2003.
- R. I. Hartley and A. Zisserman. Multiple View Geometry in Computer Vision. Cambridge University Press, 2000.

### Papers

2019
- Y. Zhou, H. Qi, and Y. Ma. NeurVPS: Neural Vanishing Point Scanning via Conic Convolution. In NeurIPS, 2019.  [[project](https://github.com/zhou13/neurvps)]
- Y. Zhou, H. Qi, and Y. Ma. End-to-End Wireframe Parsing. In ICCV, 2019. [[project](https://github.com/zhou13/lcnn)]
- Y. Zhou, H. Qi, Y. Zhai, Q. Sun, Z. Chen, L. Wei, and Y. Ma. Learning to Reconstruct 3D Manhattan Wireframes from a Single Image. In ICCV, 2019. [[project](https://arxiv.org/abs/1905.07482)]
- J. Chen, C. Liu, J. Wu, and Y. Furukawa. Floor-SP: Inverse CAD for Floorplans by Sequential Room-wise Shortest Path. In ICCV, 2019. [[project](https://github.com/woodfrog/floor-sp)]
- J. Zheng*, J. Zhang*, J. Li*, R. Tang, S. Gao, Z. Zhou.  Structured3D: A Large Photo-realistic Dataset for Structured 3D Modeling. arXiv:1908.00222, 2019. [[project](https://structured3d-dataset.org/)]
- C. Liu, K. Kim, J. Gu, Y. Furukawa, and J. Kautz. PlaneRCNN: 3D Plane Detection and Reconstruction from a Single Image. In CVPR, 2019. [[project](https://research.nvidia.com/publication/2019-06_PlaneRCNN)]
- Z. Yu*, J. Zheng*, D. Lian, Z. Zhou, S. Gao. Single-Image Piece-wise Planar 3D Reconstruction via Associative Embedding. In CVPR, 2019. [[project](https://github.com/svip-lab/PlanarReconstruction)]
- Z. Zhang*, Z. Li*, N. Bi, J. Zheng, J. Wang, K. Huang, W. Luo, Y. Xu, S. Gao. PPGNet: Learning Point-Pair Graph for Line Segment Detection. In CVPR, 2019. [[project](https://github.com/svip-lab/PPGNet)]

2018
- F. Yang and Z. Zhou. Recovering 3D planes from a single image via convolutional neural networks. In ECCV, 2018. [[project](https://github.com/fuy34/planerecover)]
- H. Zeng, J. Wu, and Y. Furukawa. Neural Procedural Reconstruction for Residential Buildings. In ECCV, 2018. [[paper](http://openaccess.thecvf.com/content_ECCV_2018/papers/Huayi_Zeng_Neural_Procedural_Reconstruction_ECCV_2018_paper.pdf)]
- C. Liu*, J. Yu*, and Y. Furukawa. FloorNet: A Unified Framework for Floorplan Reconstruction from 3D Scans. In ECCV 2018. [[project](https://github.com/art-programmer/FloorNet)]
- C. Zou, A. Colburn, Q. Shan, and D. Hoiem. Layoutnet: Reconstructing the 3d room layout from a single RGB image. In CVPR, 2018. [[project](https://github.com/zouchuhang/LayoutNet)]
- C. Niu, J. Li, and K. Xu. Im2struct: Recovering 3d shape structure from a single RGB image. In CVPR, 2018. [[project](https://github.com/chengjieniu/Im2Struct)]
- C. Liu, J. Yang, D. Ceylan, E. Yumer, and Y. Furukawa. PlaneNet: Piece-wise Planar Reconstruction from a Single RGB Image. In CVPR, 2018. [[project](https://github.com/art-programmer/PlaneNet)]
- K. Huang, Y. Wang, Z. Zhou, T. Ding, S. Gao, and Y. Ma. Learning to parse wireframes in images of man-made environments. In CVPR, 2018. [[project](https://github.com/huangkuns/wireframe)]
- J. Wu, T. Xue, J. J. Lim, Y. Tian, J. B. Tenenbaum, A. Torralba, and W. T. Freeman. 3d interpreter networks for viewer centered wireframe modeling. IJCV, 2018. [[paper](https://arxiv.org/abs/1804.00782)]

2017
- C. Liu, J. Wu, P. Kohli, and Y. Furukawa. Raster-to-Vector: Revisiting Floorplan Transformation. In ICCV, 2017. [[project](https://github.com/art-programmer/FloorplanTransformation)]
- C. Lee, V. Badrinarayanan, T. Malisiewicz, and A. Rabinovich. Roomnet: End-to-end room layout estimation. In ICCV, 2017. [[paper](https://arxiv.org/abs/1703.06241)]
- S. Tulsiani, H. Su, L. J. Guibas, A. A. Efros, and J. Malik. Learning Shape Abstractions by Assembling Volumetric Primitives. In CVPR, 2017. [[project](https://shubhtuls.github.io/volumetricPrimitives/)]
- H. Izadinia, Q. Shan, S. M. Seitz. IM2CAD. In CVPR, 2017. [[project](https://homes.cs.washington.edu/~izadinia/im2cad.html)]
- E. Wijmans and Y. Furukawa. Exploiting 2D Floorplan for Building-scale Panorama RGBD Alignment. In CVPR, 2017. [[project](https://cvpr17.wijmans.xyz/)]

2016
- C. Zhu, Z. Zhou, Z. Xing, Y. Dong, Y. Ma, and J. Yu. Robust Plane-based Calibration of Multiple Non-Overlapping Cameras. In 3DV, 2016. [[paper](https://faculty.ist.psu.edu/zzhou/paper/3dv16-calibration.pdf)]
- C. Liu, P. Kohli, and Y. Furukawa. Layered Scene Decomposition via the Occlusion-CRF. In CVPR, 2016. [[project](https://sites.wustl.edu/chenliu/layered-scene/)]
- S. Dasgupta, K. Fang, K. Chen, and S. Savarese. Delay: Robust spatial layout estimation for cluttered indoor scenes. In CVPR, 2016. [[paper](https://www.google.com/search?q=Delay%3A+Robust+spatial+layout+estimation+for+cluttered+indoor+scenes&oq=Delay%3A+Robust+spatial+layout+estimation+for+cluttered+indoor+scenes&aqs=chrome..69i57j69i58.406j0j4&sourceid=chrome&ie=UTF-8)]

2015
- S. Ikehata, H. Yan, and Y. Furukawa. Structured Indoor Modeling. In ICCV, 2015. [[paper](https://www.cv-foundation.org/openaccess/content_iccv_2015/papers/Ikehata_Structured_Indoor_Modeling_ICCV_2015_paper.pdf)]
- O. Haines and A. Calway. Recognising planes in a single image. IEEE TPAMI, 2015. [[paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=6987324)]
- A. Monszpart, N. Mellado, G. J. Brostow, and N. J. Mitra. RAPTER: Rebuilding Man-made Scenes with Regular Arrangements of Planes. SIGGRAPH, 2015. [[paper](https://geometry.cs.ucl.ac.uk/projects/2015/regular-arrangements-of-planes/paper_docs/RAPter_MonszpartEtAl_SIGGRAPH_2015.pdf)]

2014
- D. F. Fouhey, A. Gupta, and M. Hebert. Unfolding an indoor origami world. In ECCV, 2014. [[paper](https://ri.cmu.edu/pub_files/2014/7/dfouhey_origami.pdf)]
- R. Cabral and Y. Furukawa. Piecewise Planar and Compact Floorplan Reconstruction from Images. In CVPR 2014. [[paper](https://www.andrew.cmu.edu/user/rcabral/CabralFurukawaCVPR2014.pdf)]

2013
- S. Ramalingam and M. Brand. Lifting 3D manhattan lines from a single image. In ICCV, 2013. [[paper](https://www.merl.com/publications/docs/TR2013-110.pdf)]
- S. Ramalingam, J. K. Pillai, A. Jain, and Y. Taguchi. Manhattan junction catalogue for spatial reasoning of indoor scenes. In CVPR, 2013. [[paper](https://ieeexplore.ieee.org/document/6619238)]
- Z. Zhou, H. Jin, and Y. Ma. Plane-Based Content-Preserving Warps for Video Stabilization. In CVPR, 2013. [[paper](https://www.cv-foundation.org/openaccess/content_cvpr_2013/papers/Zhou_Plane-Based_Content_Preserving_2013_CVPR_paper.pdf)]

2012
- J. Xiao, B. C. Russell, and A. Torralba. Localizing 3d cuboids in single-view images. In NIPS, 2012. [[paper](http://papers.nips.cc/paper/4842-localizing-3d-cuboids-in-single-view-images.pdf)]
- J. Xiao and Y. Furukawa. Reconstructing the World's Museums. In ECCV, 2012. [[paper](https://vision.princeton.edu/projects/2012/museum/paper.pdf)]
- Z. Zhou, H. Jin, and Y. Ma. Robust Plane-Based Structure From Motion. In CVPR, 2012. [[paper](https://faculty.ist.psu.edu/zzhou/paper/1442.pdf)]

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
- M. Pauly, N. J. Mitra, J. Wallner, H. Pottmann, and L. J. Guibas. Discovering Structural Regularity in 3D Geometry. SIGGRAPH, 2008. [[paper](https://lgg.epfl.ch/publications/2008/pauly_2008_DSR.pdf)]
- G. Schindler, P. Krishnamurthy, R. Lublinerman, Y. Liu, and F. Dellaert. Detecting and Matching Repeated Patterns for Automatic Geo-tagging in Urban Environments. In CVPR, 2008. [[paper](https://www.ri.cmu.edu/pub_files/pub4/schindler_grant_2008_1/schindler_grant_2008_1.pdf)]
- B. Micusik, H. Wildenauer, and J. Kosecka. Detection and matching of rectilinear structures. In CVPR, 2008. [[paper](https://ieeexplore.ieee.org/document/4587488)]
- D. Hoiem, A. A. Efros, and M. Hebert. Recovering surface layout from an image. IJCV, 2007. [[paper](http://dhoiem.cs.illinois.edu/publications/hoiem_ijcv2007SurfaceLayout.pdf)]
- G. Schindler, P. Krishnamurthy, and F. Dellaert. Line-Based Structure From Motion for Urban Environments. In 3DPVT, 2006. [[paper](https://www.cc.gatech.edu/projects/4d-cities/dhtml/pubs/Schindler06-3dpvt.pdf)]
- J. M. Coughlan and A. L. Yuille. Manhattan world: Orientation and outlier detection by bayesian inference. Neural Computation, 2003. [[paper](https://ieeexplore.ieee.org/document/6790299)]
- A. Bartoli and P. Sturm. Constrained structure and motion from multiple uncalibrated views of a piecewise planar scene. IJCV, 2003. [[paper](https://link.springer.com/article/10.1023/A:1022318524906)]
- J. Kosecka, and W. Zhang. Video Compass. In ECCV, 2002. [[paper](https://link.springer.com/chapter/10.1007/3-540-47979-1_32)]
- J. Malik. Interpreting line drawings of curved objects. IJCV, 1987. [[paper](https://people.eecs.berkeley.edu/~malik/papers/malik87.pdf)]
- A. P. Witkin and J. M. Tenenbaum. On the role of structure in vision. In J. Beck, B. Hope, and A. Rosenfeld, editors, Human and Machine Vision, pages 481–543. Academic Press, 1983. [[paper](http://cvcl.mit.edu/SUNSeminar/BarenholtzTarr_2007.pdf)]
- K. Sugihara. Mathematical structures of line drawings of polyhedrons-toward man-machine communication by means of line drawings. IEEE TPAMI, 1982. [[paper](https://ieeexplore.ieee.org/document/4767289)]


