# Computer Graphics

* 吴雨婷
  * 办公室: 逸夫西
  * 邮箱: ytwu1@bjtu.edu.cn
* 考核
  * 平时成绩
    * 4次课后作业, 包含课程小测试
    * 2次大作业
    * 5~6人一组
    * 分配分数, 但是浮动上下不超过4
* 课程内容及安排

## 1. Transformation

### 1.1 2D

* 线性变换
  * 满足可加性, 齐次性
    * <=> 线性变换保持向量加法和标量乘法不变
* Scale Transformation 缩放变换
  * 【变换矩阵】
* Reflection Transformation 反射矩阵
  * 【变换矩阵】
* Shear Transformation 切变变换
  * 【变换矩阵】
* Rotate Transformation 旋转矩阵
  * 【变换矩阵】
  * How to get Rotate Transformation
    * 方法一：待定系数法
  * 性质
    * $R_{-\theta} = R_{\theta}^{-1} = R_{\theta}^{T}$​
    * 旋转矩阵是一个正交矩阵
* Homogenous Coordinates
  * Affine Transformation
  * Affine = Linear + Translate
* Inverse Transform
* Composite Transform

### 1.2 3D

* 3D Rotate
  * Rodrigues' Rotation Formula
* 四元数
  * 四元数不会万向节死锁、支持插值

## 2. MVP

### 2.1 View T.

* Definition of Camera
  * position
  * gaze
  * up
* How to get View T.
  1. Translate e to origin
  2. rotates g to -Z
  3. rotate t to Y
  4. rotate (g x t) to X

### 2.2 Projection T.

* Orthographic Projection
  * 根据L、R、B、T、N、F六个值，得到Orthographic P.T.
* Perspective Projection
  * 

