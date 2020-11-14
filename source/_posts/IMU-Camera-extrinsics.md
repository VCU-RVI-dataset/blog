---
title: IMU-Camera extrinsics
date: 2020-08-12 16:41:03
tags: [Calibration, Dataset]
---
We recorded a sequence about three minutes and employed the Kalibr toolbox [<sup>1</sup>](#refer-anchor-1) to estimate the extrinsic transformation matrix ($T_c^b$) between the color camera and the IMU. We also measured the translation from the color camera to the IMU with a vernier scale. The extrinsic $T_c^b$ provided by Occipital is more accurate than our calibration result, comparing to the ruler-measurement. Therefore, we used the extrinsic transformation matrix provided by Occipital in our evaluation.

```yaml
body_T_cam0: !!opencv-matrix # Timu2c_1 Tu2c
   rows: 4
   cols: 4
   dt: d
   data: [0.00193013, -0.999997, 0.00115338, -0.00817048,
      -0.999996, -0.0019327, -0.00223606, 0.015075,
      0.00223829, -0.00114906, -0.999997, -0.0110795,
      0, 0, 0, 1]

body_T_cam1: !!opencv-matrix # Timu2c_2, Tc1_2_c2 is a virtual transformation [I,t] t = [0.1, 0, 0], note "mbf" in estimator_dpt.cpp
   rows: 4
   cols: 4
   dt: d
   data: [0.00193013, -0.999997, 0.00115338, -0.007977467,
      -0.999996, -0.0019327, -0.00223606, -0.0849246,
      0.00223829, -0.00114906, -0.999997, -0.010855671,
      0, 0, 0, 1]
```



**Dataset download** [calibrate_imu_cam - Google Drive](https://drive.google.com/drive/folders/1TzVq_GvnhUQSWwMMWM0rTgv4tmiJj1OI?usp=sharing)



## References:

<div id="refer-anchor-1"></div>

- [1]: Paul Furgale, Joern Rehder, Roland Siegwart (2013). Unified Temporal and Spatial Calibration for Multi-Sensor Systems. In Proceedings of the IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS), Tokyo, Japan.


