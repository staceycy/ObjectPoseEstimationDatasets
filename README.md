# ObjectPoseEstimationDatasets
A repo to summarize datasets used for object pose estimation

**model**: 3D CAD object model

**object**: 2D pictured object

## Datasets with exact 3D models for objects
| Dataset | Sample image | Annotation | Statistics | Reference |
| :-----: | :-----: | :-----: | :-----: | :-----: |
| [HomebrewedDB](https://arxiv.org/abs/1904.03167) | ![](https://github.com/YoungXIAO13/6DPoseEstimationDatasets/blob/master/img/HomebrewedDB.png) | 6D pose + Depth + BoundingBox| **33** models in **13** videos with **17,420** frames| [Preprint 2019](https://arxiv.org/abs/1904.03167)| 
| [YCB-Video](https://rse-lab.cs.washington.edu/projects/posecnn/) | ![](https://github.com/YoungXIAO13/6DPoseEstimationDatasets/blob/master/img/YCB-Video.png) | 6D Pose + Depth + Mask | **21** models in **92** videos with **133,827** frames| [RSS 2018](https://arxiv.org/abs/1711.00199) |
| [T-LESS](http://ptak.felk.cvut.cz/6DB/public/datasets/t-less/)| ![](https://github.com/YoungXIAO13/6DPoseEstimationDatasets/blob/master/img/T-LESS.png) | 6D Pose + Depth | **30** models in **20** videos with **~49K** frames | [WACV 2017](http://cmp.felk.cvut.cz/t-less/)|
| [Doumanoglou](http://ptak.felk.cvut.cz/6DB/public/datasets/doumanoglou/)| ![](https://github.com/YoungXIAO13/6DPoseEstimationDatasets/blob/master/img/Doumanoglou.png)| 6D Pose + Depth | **2** models in **3** videos with **183** frames| [CVPR 2016](http://rkouskou.gitlab.io/research/6D_NBV.html)|
| [Tejani](http://ptak.felk.cvut.cz/6DB/public/datasets/tejani/) | ![](https://github.com/YoungXIAO13/6DPoseEstimationDatasets/blob/master/img/Tejani.png) | 6D Pose + Depth | **6** models in **6** videos with **2,067** frames | [ECCV 2014](http://rkouskou.gitlab.io/research/LCHF.html)|
| [Occluded-LINEMOD](http://ptak.felk.cvut.cz/6DB/public/datasets/hinterstoisser/) | One Video of LINEMOD | 6D Pose + Depth | **8** models in **1,214** frames with **8,992** objects | [ECCV 2014](http://wwwpub.zih.tu-dresden.de/~cvweb/publications/papers/2014/PoseEstimationECCV2014.pdf) | 
| [LINEMOD](http://ptak.felk.cvut.cz/6DB/public/datasets/hinterstoisser/) | ![](https://github.com/YoungXIAO13/6DPoseEstimationDatasets/blob/master/img/LINEMOD.png) | 6D pose + Depth for one object | **15** models in **15** videos with **18,273** frames | [ACCV 2012](http://www.stefan-hinterstoisser.com/papers/hinterstoisser2012accv.pdf) |



## Datasets without exact 3D models for objects in the wild

| Dataset | Sample image | Annotation | Statistics | Reference |
| :-----: | :-----: | :-----: | :-----: | :-----: |
| [ApolloCar3D](http://apolloscape.auto/car_instance.html) | ![](https://github.com/YoungXIAO13/6DPoseEstimationDatasets/blob/master/img/ApolloCar3D.png) | 6D Pose + Mask | **34** car models with **60K+** objects in **5,277** images | [CVPR 2019](https://arxiv.org/abs/1811.12222) |
| [ObjectNet3D](http://cvgl.stanford.edu/projects/objectnet3d/) | ![](https://github.com/YoungXIAO13/6DPoseEstimationDatasets/blob/master/img/ObjectNet3D.png) | Euler Angles + BoundingBox | **100** categories with **201,888** objects in **90,127** images | [ECCV 2016](http://cvgl.stanford.edu/papers/xiang_eccv16.pdf) |
| [PASCAL3D+](http://cvgl.stanford.edu/projects/pascal3d.html) | ![](https://github.com/YoungXIAO13/6DPoseEstimationDatasets/blob/master/img/Pascal3D.png) | Euler Angles + BoundingBox | **12** categories with **36,292** objects in **30,889** images | [WACV 2014](https://www-cs.stanford.edu/~roozbeh/papers/wacv14.pdf) |
| [KITTI](http://www.cvlibs.net/datasets/kitti/eval_object.php) | ![](https://github.com/YoungXIAO13/6DPoseEstimationDatasets/blob/master/img/KITTI.png) | 3D BoundingBox | **80,256** objects in **14,999** images | [CVPR 2012](http://www.cvlibs.net/publications/Geiger2012CVPR.pdf) |


## 3D model datasets for generating synthetic data
In order to testify the network **generalization** ability (training and testing on images from different domains with different models),
the following dataset could be used to generate synthetic training data.

| Dataset | Number of categories | Number of models | Reference |
| :-----: | :-----: | :-----: | :-----: |
| [ABC](https://deep-geometry.github.io/abc-dataset/) | - | 1 million | [CVPR 2019](https://arxiv.org/pdf/1812.06216.pdf) |
| [ShapeNetCore](https://www.shapenet.org/download/shapenetcore) | 55 | ~51,300 | [ArXiv 2015](https://arxiv.org/abs/1512.03012) | 
| [ModelNet-40](http://modelnet.cs.princeton.edu/) | 40 | 26,960 | [CVPR 2015](https://3dshapenets.cs.princeton.edu/paper.pdf) |



## Attention
While wandering through the different datasets, 3D models should be aligned in the same way through **meshlab** to ensure the consistent orientation.