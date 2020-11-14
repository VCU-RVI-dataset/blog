---
title: MoCap-IMU-extrinsics
date: 2020-08-14 13:15:56
tags: [Calibration, Dataset]
---

In order to obtain the ground truth trajectory in the IMU/body’s coordinate system, the extrinsic transformation matrix ($T_M^b$) from MoCap to IMU is required. MoCap can detect and track the LED markers which are installed on the SC, shown in figure below. 

![image-20200814130930340](https://tva1.sinaimg.cn/large/007S8ZIlgy1ghqu8zh0n1j30cq05qgp6.jpg)

The transformation matrix from MoCap to the marker’s coordinate system is described as $T_H^M$. Since the camera-IMU extrinsic transformation matrix ($T_c^b$) is known, we need the camera-maker transformation matrix ($T_c^H$) to compute $T_M^b$.  $T_c^H$ can be obtained through a hand-eye calibration approach [<sup>1</sup>](#refer-anchor-1). To solve $T_c^H$, we recorded a data sequence by moving the SC around a checkboard (maintaining the checkboard in the SC’s field of view). Then we employed Zhang’s method [<sup>2</sup>](#refer-anchor-2) to compute the camera poses. Given the camera poses and the marker’s poses observed from the MoCap, we used Daniilidis’ method [<sup>1</sup>](#refer-anchor-1) to estimate $T_c^H$ and achieved a final pose residual about 0.6703 mm. Given $T_c^H$ , $T_M^b$ is given by $T_{M}^{b}=T_{c}^{b}\left(T_{c}^{H}\right)^{-1}\left(T_{H}^{M}\right)^{-1}$

**Dataset download** [hand-eye - Google Drive](https://drive.google.com/drive/folders/1diqBgnHguA5lumcUvXhmcOVzg-KTo2kw?usp=sharing)



## References:

<div id="refer-anchor-1"></div>

- [1]: Daniilidis, K. “Hand-eye calibration using dual quaternions,” The International Journal of Robotics Research, 18(3), 286-298.

<div id="refer-anchor-2"></div>

- [2]: Zhang, Zhengyou. "A flexible new technique for camera calibration." IEEE Transactions on pattern analysis and machine intelligence 22.11 (2000): 1330-1334.