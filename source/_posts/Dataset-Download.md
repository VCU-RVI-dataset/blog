---
title: Dataset Download
date: 2020-08-14 15:10:57
tags: [Calibration, Dataset]
---

##  Calibration

Except for evaluation sequences, the calibration data sequences are made available, allowing users to perform their own calibration. Three sequences are provided in the dataset:

• **camera**: sequence with slow-motion viewing a grid of AprilTags for camera intrinsics calibration. 

• **camera-imu**: sequence with fast motion viewing a grid of AprilTags for camera-imu extrinsic calibration. [camera-imu](https://drive.google.com/drive/folders/1TzVq_GvnhUQSWwMMWM0rTgv4tmiJj1OI?usp=sharing)

• **hand-eye**: sequence with slow-motion viewing a checkboard for camera-marker extrinsic calibration. [hand-eye](https://drive.google.com/drive/folders/1diqBgnHguA5lumcUvXhmcOVzg-KTo2kw?usp=sharing)

## Handheld

According to the data recording conditions and environments, the data sequences can be divided into the following categories:
• **lab**: sequences completely inside the laboratory in which ground truth covers the full trajectory. 
	– **lab-easy**: move the SC with normal speed, constant illumination, and static objects. [simple1](https://drive.google.com/file/d/1_GItVMVem1Byt00QueeilfJAdz3UXcTl/view?usp=sharing) [simple2](https://drive.google.com/file/d/1QMuZMOAcmhLosBLX7nDdERKgwthzQHMi/view?usp=sharing) [simple3](https://drive.google.com/file/d/1ZxD-aD40OZt4OKrV1_DJ779QF1RqKdeN/view?usp=sharing)
	– **lab-motion**: move the SC with high speed, constant illumination and static objects. The mean and max of the rotation speed are about 35 and 120 degrees per second, respectively. [motion1](https://drive.google.com/file/d/1JseGcRS7nQypBtaNKqsCO5bbF7v3bu8E/view?usp=sharing) [motion2](https://drive.google.com/file/d/116cj7VIU8CW9BKYTxMSUQM8L69HMieuI/view?usp=sharing)[motion3](https://drive.google.com/file/d/11orqwnL-OVFmBr08gcey-qXWivcJwgi4/view?usp=sharing) [motion4](https://drive.google.com/file/d/18p2bLWdyIkWaHd9ZPPDcYNi-qV_MwLvH/view?usp=sharing) [motion5](https://drive.google.com/file/d/1FRgXcI6IXIgYjCLJCAUtE4Fqg8F2zJdV/view?usp=sharing) [motion6](https://drive.google.com/file/d/1bc5XMQXHBKD3e10NTEXXXb-YOEzaaZuE/view?usp=sharing)
	– **lab-light**: move the SC with normal speed, radical changing illumination, and static objects. In some sequences, the illumination condition changes from bright light to complete darkness for about 10 seconds. [light1](https://drive.google.com/file/d/1fnH9XpBbYTJ4ECCzgnaYLoxiV4xMJECa/view?usp=sharing) [light2](https://drive.google.com/file/d/1gGgb9r0m89seNxQY71jQHXSqTWieDbK-/view?usp=sharing) [light3](https://drive.google.com/file/d/1H4nmLB81ecmc_KQHdLwbaJ-LfVxazE8R/view?usp=sharing) [light4](https://drive.google.com/file/d/1G17HFiIB0z8ztaf5wKk2VUrtBXndGo_A/view?usp=sharing) [light5](https://drive.google.com/file/d/1gZt6nd853cYFugY8PXvN2V_W3zFNUIFO/view?usp=sharing) [light6](https://drive.google.com/file/d/14_aOlX_GspPVxmZZCoheuy1TEwCMAjps/view?usp=sharing)
	– **lab-dynamic**: move the SC with normal speed, constant illumination, and dynamic objects. The dynamic objects include one or two persons, a chair, a wheeled robot, or a rollator. [dynamic1](https://drive.google.com/file/d/1I3JX-0PmPQDbyxschKadhsp7YuJwJ2BA/view?usp=sharing) [dynamic2](https://drive.google.com/file/d/1VSK8pTlZFItJ2q6t5rlrJS93_B1VU4YN/view?usp=sharing) [dynamic3](https://drive.google.com/file/d/139en07SKlfZeUBB2tujucSUtv3wFhnl6/view?usp=sharing) [dynamic4](https://drive.google.com/file/d/1D45FbQgrttcQphCnu_9lPwsf4e1bKhm2/view?usp=sharing) [dynamic5](https://drive.google.com/file/d/1Ck4jAc-Y9EVTlI7mri5mpFJWzm8bvdCy/view?usp=sharing)
• **corridor**: sequences with camera motion along corridors. [corridor1](https://drive.google.com/file/d/1Rg8QnED0V1j1lCS38KDj_2e-djRqL2U3/view?usp=sharing) [corridor2](https://drive.google.com/file/d/11eRKYl_u-LY8VgYPfiSpfBI3aE-c9oyI/view?usp=sharing) [corridor3](https://drive.google.com/file/d/189lbBTXvGjRjxlbLMqQYf-GVdx6ir8m2/view?usp=sharing) [corridor4](https://drive.google.com/file/d/1VsW6ZKbHoqMDI9ZGlgThBlsdpkR1LWD4/view?usp=sharing) 
• **hall**: sequences with camera motion around one or two halls and the camera trajectory also covers corridors and stairways.  [hall1](https://drive.google.com/file/d/1t9ZpN4X2SHW_wJ88762lquT4eHJMCsFh/view?usp=sharing) [hall2](https://drive.google.com/file/d/14IPHtRWQrb54oLSEA_gJze5egPIJCL7A/view?usp=sharing) [hall3](https://drive.google.com/file/d/1DGhaAIw6f8X8uGiN8RYz2Ayx818VHTf9/view?usp=sharing) 

## Wheeled Robot
For the data sequences recorded with the mobile robot, they are captured in the laboratory and along the corridors. The wheeled robot is controlled by a BlueTooth connected gamepad to move linearly from point to point. Since the acceleration readings of the IMU installed on a wheeled robot have less variance when it is controlled to move linearly [<sup>1</sup>](#refer-anchor-1). This leads to insufficient IMU excitement, failing to provide sufficient conditions for initialization [<sup>2</sup>](#refer-anchor-2), [<sup>1</sup>](#refer-anchor-1). At the beginning of each sequence, we intentionally deal with this issue in two ways:  
• **manual**: handhold and rotate the SC for about five seconds to excite IMU measurements for a good system initialization; then put the SC on the robot and drive the robot to move. [lab1](https://drive.google.com/file/d/1h9YpH4lu3QVWC5jYBvlEPWnmhQDKaSNX/view?usp=sharing) [lab2](https://drive.google.com/file/d/1z2hSIwKdOnKZrx9jajicznsA50fN61-6/view?usp=sharing) [lab3](https://drive.google.com/file/d/1vOvHbLBJvii4yz69UZOcEXmKlENWrOSC/view?usp=sharing) [corridor1](https://drive.google.com/file/d/15x3f_0p886_cTpZnRVn8J96MXVq8Jsd1/view?usp=sharing) [corridor2](https://drive.google.com/file/d/1RnZJwiPDbdvl_Clr7BLt8rWfd6_Gsf2O/view?usp=sharing) 
• **bumper**: drive the robot along the bumpers to generate 6 DoF movements, producing more variance to the IMU measurements for initialization purpose; then drive it around the whole area. [lab1](https://drive.google.com/file/d/19asRb3Q3xnpXkRXwGJgQctbDmsGZDz-n/view?usp=sharing) [lab2](https://drive.google.com/file/d/1eSRcUt7giNrVRqyWOMJx-XvtaiWkmiTF/view?usp=sharing) [lab3](https://drive.google.com/file/d/1yEuyQar0fVJHLvcVxXxMVPQRCj3v7sud/view?usp=sharing) [lab4](https://drive.google.com/file/d/1rl8MCU3iqoaOqUatckmcA9bRstcVPrHz/view?usp=sharing) [lab5](https://drive.google.com/file/d/1pGmK0PoMPt6pFZrI6oa_on0ZNw6DFWDn/view?usp=sharing) [corridor1](https://drive.google.com/file/d/1_0UkvP1bafkZQn5UJG0xzRlQNY_Iyvx2/view?usp=sharing) [corridor2](https://drive.google.com/file/d/1SdzCdVj85VwI9eMTKAu1QFXljleQ-DGc/view?usp=sharing) 

## Download

| Dataset         	| ROS bag | Ground Truth | Comment |
| :---------------- | ------- | ------------ | :------ |
| lab-easy-01     	| [simple1](https://drive.google.com/file/d/1_GItVMVem1Byt00QueeilfJAdz3UXcTl/view?usp=sharing) | [simple1](https://drive.google.com/file/d/1KhzJiQxpYI6Iz5hbi6PATsUI9JFHhtCA/view?usp=sharing) | Handheld, lab, normal speed, static objects |
| lab-easy-02     	| [simple2](https://drive.google.com/file/d/1QMuZMOAcmhLosBLX7nDdERKgwthzQHMi/view?usp=sharing) | [simple2](https://drive.google.com/file/d/1jtEbcvWyRsbNIbOOql2FhrdXZS2S055D/view?usp=sharing) | Handheld, lab, normal speed, static objects |
| lab-easy-03     	| [simple3](https://drive.google.com/file/d/1ZxD-aD40OZt4OKrV1_DJ779QF1RqKdeN/view?usp=sharing) | [simple3](https://drive.google.com/file/d/1DfOyUvY45045_2xe8tup724xdTrZ4V6l/view?usp=sharing) | Handheld, lab, normal speed, static objects |
| lab-motion-01   	| [motion1](https://drive.google.com/file/d/1JseGcRS7nQypBtaNKqsCO5bbF7v3bu8E/view?usp=sharing) | [motion1](https://drive.google.com/file/d/1v2LNTEeGfRtUNsNHll8PY_QvuGYn9jmS/view?usp=sharing) | Handheld, lab, high speed, static objects |
| lab-motion-02   	| [motion2](https://drive.google.com/file/d/116cj7VIU8CW9BKYTxMSUQM8L69HMieuI/view?usp=sharing) | [motion2](https://drive.google.com/file/d/1Mm9u9BmcAfE0RAW20-kDXFtSws49Vy5R/view?usp=sharing) | Handheld, lab, high speed, static objects |
| lab-motion-03   	| [motion3](https://drive.google.com/file/d/11orqwnL-OVFmBr08gcey-qXWivcJwgi4/view?usp=sharing) | [motion3](https://drive.google.com/file/d/1sgPjWeNAIAOWnTm7YFz_XUKHPMEyPUtn/view?usp=sharing) | Handheld, lab, high speed, static objects |
| lab-motion-04   	| [motion4](https://drive.google.com/file/d/18p2bLWdyIkWaHd9ZPPDcYNi-qV_MwLvH/view?usp=sharing) | [motion4](https://drive.google.com/file/d/1iWsCz60OV5XFQ7QgWm1bnlVKTb6p9m4t/view?usp=sharing) | Handheld, lab, high speed, static objects |
| lab-motion-05   	| [motion5](https://drive.google.com/file/d/1FRgXcI6IXIgYjCLJCAUtE4Fqg8F2zJdV/view?usp=sharing) | [motion5](https://drive.google.com/file/d/1UCnOi75vraUssUNcXXD99s4JER6V0Zao/view?usp=sharing) | Handheld, lab, high speed, static objects |
| lab-motion-06   	| [motion6](https://drive.google.com/file/d/1bc5XMQXHBKD3e10NTEXXXb-YOEzaaZuE/view?usp=sharing) | [motion6](https://drive.google.com/file/d/173QPRJsgnnCRuJQ9YJu2s-9rYhWyqpXn/view?usp=sharing) | Handheld, lab, high speed, static objects |
| lab-light-01    	| [light1](https://drive.google.com/file/d/1fnH9XpBbYTJ4ECCzgnaYLoxiV4xMJECa/view?usp=sharing) | [light1](https://drive.google.com/file/d/1Bvg8J8qWTdR-5IOclRihMXRkeJd7mIrn/view?usp=sharing) | Handheld, lab, normal speed, static objects, varying illumination |
| lab-light-02    	| [light2](https://drive.google.com/file/d/1gGgb9r0m89seNxQY71jQHXSqTWieDbK-/view?usp=sharing) | [light2](https://drive.google.com/file/d/1LI8CQctsNWwpSygeXzCtozN1QbVATMe4/view?usp=sharing) | Handheld, lab, normal , static objects, varying illumination |
| lab-light-03    	| [light3](https://drive.google.com/file/d/1H4nmLB81ecmc_KQHdLwbaJ-LfVxazE8R/view?usp=sharing) | [light3](https://drive.google.com/file/d/1f9c-bpbH0-kxsaIcghCQCbTaLEtSYvdC/view?usp=sharing) | Handheld, lab, normal speed, static objects, varying illumination |
| lab-light-04    	| [light4](https://drive.google.com/file/d/1G17HFiIB0z8ztaf5wKk2VUrtBXndGo_A/view?usp=sharing) | [light4](https://drive.google.com/file/d/1TyYSM68R2pAmn5gEzRPG-1jli3jbw23y/view?usp=sharing) | Handheld, lab, normal speed, static objects, varying illumination |
| lab-light-05    	| [light5](https://drive.google.com/file/d/1gZt6nd853cYFugY8PXvN2V_W3zFNUIFO/view?usp=sharing) | [light5](https://drive.google.com/file/d/1pUQl73LC4ApFg6ePAc2eIaoEcAovvIbU/view?usp=sharing) | Handheld, lab, normal speed, static objects, varying illumination |
| lab-light-06    	| [light6](https://drive.google.com/file/d/14_aOlX_GspPVxmZZCoheuy1TEwCMAjps/view?usp=sharing) | [light6](https://drive.google.com/file/d/1O0ir74rD1BFRLlY1vCc1Et_jHaw3cls7/view?usp=sharing) | Handheld, lab, normal speed, static objects, varying illumination |
| lab-dynamic-01  	| [dynamic1](https://drive.google.com/file/d/1I3JX-0PmPQDbyxschKadhsp7YuJwJ2BA/view?usp=sharing) | [dynamic1](https://drive.google.com/file/d/1Eut3il5loxb4qvkhfb24HkORy5M07EQ-/view?usp=sharing) | Handheld, lab, normal speed, dynamic objects |
| lab-dynamic-02  	| [dynamic2](https://drive.google.com/file/d/1VSK8pTlZFItJ2q6t5rlrJS93_B1VU4YN/view?usp=sharing) | [dynamic2](https://drive.google.com/file/d/1wurIwsOr-APnAM7_YBWwea3L3N7W_Meq/view?usp=sharing) | Handheld, lab, normal speed, dynamic objects |
| lab-dynamic-03  	| [dynamic3](https://drive.google.com/file/d/139en07SKlfZeUBB2tujucSUtv3wFhnl6/view?usp=sharing) | [dynamic3](https://drive.google.com/file/d/1z2rq2_LPcB1hNFCDfX2gT5cHGtk3Ht_S/view?usp=sharing) | Handheld, lab, normal speed, dynamic objects |
| lab-dynamic-04  	| [dynamic4](https://drive.google.com/file/d/1D45FbQgrttcQphCnu_9lPwsf4e1bKhm2/view?usp=sharing) | [dynamic4](https://drive.google.com/file/d/1DZrVharNXO9OQir5wHMNVU7QGKMIKxUh/view?usp=sharing) | Handheld, lab, normal speed, dynamic objects |
| lab-dynamic-05  	| [dynamic5](https://drive.google.com/file/d/1Ck4jAc-Y9EVTlI7mri5mpFJWzm8bvdCy/view?usp=sharing) | [dynamic5](https://drive.google.com/file/d/1x3YW7ucpW4zvzbPGAMob6E1ZfAmZ2EBo/view?usp=sharing) | Handheld, lab, normal speed, dynamic objects |
| handheld-corridor-01 | [corridor1](https://drive.google.com/file/d/1Rg8QnED0V1j1lCS38KDj_2e-djRqL2U3/view?usp=sharing) | [corridor1](https://drive.google.com/file/d/13dhGgX-vXffRVCwtIjKyxJ6Gv8dBiZCJ/view?usp=sharing) | Handheld, corridor, normal speed, static objects |
| handheld-corridor-02 | [corridor2](https://drive.google.com/file/d/11eRKYl_u-LY8VgYPfiSpfBI3aE-c9oyI/view?usp=sharing) | [corridor2](https://drive.google.com/file/d/1o0_z2KLxvHACJtl69TwVt2ZRNLpO8Jpn/view?usp=sharing) | Handheld, corridor, normal speed, static |
| handheld-corridor-03 | [corridor3](https://drive.google.com/file/d/189lbBTXvGjRjxlbLMqQYf-GVdx6ir8m2/view?usp=sharing) | [corridor3](https://drive.google.com/file/d/1fjNewB97p2hVl7tPsshuRkVMhgn5OUWu/view?usp=sharing) | Handheld, corridor, normal speed, static objects |
| handheld-corridor-04 | [corridor4](https://drive.google.com/file/d/1VsW6ZKbHoqMDI9ZGlgThBlsdpkR1LWD4/view?usp=sharing) | [corridor4](https://drive.google.com/file/d/1NyI9fEt__s_vODFjzr-nzYVwsaeRNI_h/view?usp=sharing) | Handheld, corridor, normal speed, static objects |
| handheld-hall-01 | [hall1](https://drive.google.com/file/d/1t9ZpN4X2SHW_wJ88762lquT4eHJMCsFh/view?usp=sharing) | [hall1](https://drive.google.com/file/d/1-HSJEaTvX5knvB2lGRG_El7B_-iJ3NOL/view?usp=sharing) | Handheld, hall, normal speed, static objects |
| handheld-hall-02 | [hall2](https://drive.google.com/file/d/14IPHtRWQrb54oLSEA_gJze5egPIJCL7A/view?usp=sharing) | [hall2](https://drive.google.com/file/d/19UBy_tp1VbAlvCOa8ydRb5VObC3ytruh/view?usp=sharing) | Handheld, hall, normal speed, static objects |
| handheld-hall-03 | [hall3](https://drive.google.com/file/d/1DGhaAIw6f8X8uGiN8RYz2Ayx818VHTf9/view?usp=sharing) | [hall3](https://drive.google.com/file/d/1Jp8L1FDsBOVpBpdwF-r753eP1T7md-Lj/view?usp=sharing) | Handheld, hall, normal speed, static objects |
| robot-lab-01 | [lab1](https://drive.google.com/file/d/1h9YpH4lu3QVWC5jYBvlEPWnmhQDKaSNX/view?usp=sharing) | [lab1](https://drive.google.com/file/d/1lJKSPyK8TeT4d3t1c77qFkvGuQ7KveC5/view?usp=sharing) | robot, lab, normal speed, static objects |
| robotlab-02 | [lab2](https://drive.google.com/file/d/1z2hSIwKdOnKZrx9jajicznsA50fN61-6/view?usp=sharing) | [lab2](https://drive.google.com/file/d/1lbwlezNE4aBWbBj2yvZqiogzle34Ydj6/view?usp=sharing) | robot, lab, normal speed, static objects |
| robot-lab-03 | [lab3](https://drive.google.com/file/d/1vOvHbLBJvii4yz69UZOcEXmKlENWrOSC/view?usp=sharing) | [lab3](https://drive.google.com/file/d/17fQ2agllUlWrzwjxG5TGS1qcFm0JGcqA/view?usp=sharing) | robot, lab, normal speed, static objects |
| robot-corridor-01 | [corridor1](https://drive.google.com/file/d/15x3f_0p886_cTpZnRVn8J96MXVq8Jsd1/view?usp=sharing) | [corridor1](https://drive.google.com/file/d/1x3xyNHRp9jOwWNn5-Id7y26oFRjLcCD4/view?usp=sharing) | robot, corridor, normal speed, static objects |
| robot-corridor-02 | [corridor2](https://drive.google.com/file/d/1RnZJwiPDbdvl_Clr7BLt8rWfd6_Gsf2O/view?usp=sharing) | [corridor2](https://drive.google.com/file/d/1M-mHyF2ZMOYQKQwMgS2uyeY6zshT0Iko/view?usp=sharing) | robot, corridor, normal speed, static objects |
| bumper-lab-01			| [lab1](https://drive.google.com/file/d/19asRb3Q3xnpXkRXwGJgQctbDmsGZDz-n/view?usp=sharing) | [lab1](https://drive.google.com/file/d/1CkiI44uGYJt5_5_Tg2c8WR6U2jWioWKU/view?usp=sharing) | robot, lab, w/ bumper, static objects |
| bumper-lab-02			| [lab2](https://drive.google.com/file/d/1eSRcUt7giNrVRqyWOMJx-XvtaiWkmiTF/view?usp=sharing) | [lab2](https://drive.google.com/file/d/1QxgijyrJZR0SQqvQlbOo56os8FsUBpyz/view?usp=sharing) | robot, lab, w/ bumper, static objects |
| bumper-lab-03			| [lab3](https://drive.google.com/file/d/1yEuyQar0fVJHLvcVxXxMVPQRCj3v7sud/view?usp=sharing) | [lab3](https://drive.google.com/file/d/1tDwNwhXI4JQjg4Jx2Nd9lXq1rCzaBzDz/view?usp=sharing) | robot, lab, w/ bumper, static objects |
| bumper-lab-04			| [lab4](https://drive.google.com/file/d/1rl8MCU3iqoaOqUatckmcA9bRstcVPrHz/view?usp=sharing) | [lab4](https://drive.google.com/file/d/1tdq_M8B9C6Oe91eTVrFCLXJdIkQvB2yC/view?usp=sharing) | robot, lab, w/ bumper, static objects |
| bumper-lab-05			| [lab5](https://drive.google.com/file/d/1pGmK0PoMPt6pFZrI6oa_on0ZNw6DFWDn/view?usp=sharing) | [lab5](https://drive.google.com/file/d/1UwrD3ld6oY8RaStd_LNLM9T9hYIFaUSr/view?usp=sharing) | robot, lab, w/ bumper, static objects |
| bumper-corridor-01| [corridor1](https://drive.google.com/file/d/1_0UkvP1bafkZQn5UJG0xzRlQNY_Iyvx2/view?usp=sharing) | [corridor1](https://drive.google.com/file/d/1qEdxdNElTxeCzOjddgwUayxo3sBfxAI3/view?usp=sharing) | robot, corridor, w/ bumper, static objects |
| bumper-corridor-02| [corridor2](https://drive.google.com/file/d/1SdzCdVj85VwI9eMTKAu1QFXljleQ-DGc/view?usp=sharing) | [corridor2](https://drive.google.com/file/d/1sZXTufkgZplMqH4GNHWgsqiODqYFiY33/view?usp=sharing) | robot, corridor, w/ bumper, static objects |
| calibration-01 | [camera-imu](https://drive.google.com/drive/folders/1TzVq_GvnhUQSWwMMWM0rTgv4tmiJj1OI?usp=sharing) | --------- | Dataset for extrinsic calibration |
| calibration-02 | [hand-eye](https://drive.google.com/drive/folders/1diqBgnHguA5lumcUvXhmcOVzg-KTo2kw?usp=sharing) | --------- | Dataset for hand-eye calibration |






## References:

<div id="refer-anchor-1"></div>

- [1]:  Zeyong Shan, Ruijian Li, and Sören Schwertfeger.  Rgbd-inertial trajectory estimation and mapping for ground robots.   Sensors, 19(10):2251, 2019.

<div id="refer-anchor-2"></div>

- [2]: Tong Qin, Peiliang Li, and Shaojie Shen, “Vins-mono: A robust and versatile monocular visual-inertial state estimator,” IEEE Transactions on Robotics, 34(4):1004–1020, 2018.