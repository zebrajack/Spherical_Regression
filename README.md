


# Spherical_Regression


This code contains 3 parts:

- **S1.Viewpoint**      [To be cleaned up and released soon]- **S2.Surface_Normal** [To be cleaned up and released soon]- **S3.3D_Rotation**


## Dataset:

**ModelNet10-SO3** 

- In lmdb format, and to be read by `pylibs/lmdb_util/imagedata_lmdb.py`
- [Download](https://drive.google.com/file/d/17GLZbNTDq8B_MOgrV1TiJPoqcm_oQ_mK/view?usp=sharing) (2.4G)



### TODO
- Upload the caffe imagenet pretrain weights:  "pylibs/pytorch\_util/libtrain/init\_torch.py",
there's caffe_models.


## Cite

```
@INPROCEEDINGS{LiaoCVPR19, 
  author = {Shuai Liao and Efstratios Gavves and Cees G. M. Snoek}, 
  title = {Spherical Regression: Learning Viewpoints, Surface Normals and 3D Rotations on n-Spheres}, 
  booktitle = {Proceedings of the {IEEE} Conference on Computer Vision and Pattern Recognition}, 
  month = {June}, 
  year = {2019}, 
  address = {Long Beach, USA}, 
  pdf = {}, 
  abstract = { Many computer vision challenges require continuous outputs, but tend to be solved by discrete classification. The reason is classification's natural containment within a probability n-simplex, as defined by the popular softmax activation function. Regular regression lacks such a closed geometry, leading to unstable training and convergence to suboptimal local minima. Starting from this insight we revisit regression in convolutional neural networks. We observe many continuous output problems in computer vision are naturally contained in closed geometrical manifolds, like the Euler angles in viewpoint estimation or the normals in surface normal estimation. A natural framework for posing such continuous output problems are n-spheres, which are naturally closed geometric manifolds defined in the R^{(n+1)} space. By introducing a spherical exponential mapping on n-spheres at the regression output, we obtain well-behaved gradients, leading to stable training. We show how our spherical regression can be utilized for several computer vision challenges, specifically viewpoint estimation, surface normal estimation and 3D rotation estimation. For all these problems our experiments demonstrate the benefit of spherical regression. All paper resources are available at https://github.com/leoshine/Spherical_Regression. }
}
```