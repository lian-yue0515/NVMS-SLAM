<div align="center">
  <h1>NVMS-SLAM</h1>
  <h2>a normal vector-based multi-session LiDAR SLAM system tailored for indoor environments</h2>
  <p><strong>Official implementation of our paper in <i>IEEE Transactions on Automation Science and Engineering (T-ASE), 2026</i></strong></p>
  <br>
  <a href="https://arxiv.org/pdf/2503.19506v1"><img src="https://img.shields.io/badge/arXiv-2503.19506-b31b1b.svg" alt="arXiv"></a>
  <a href="https://github.com/lian-yue0515/MM-LINS"><img src="https://img.shields.io/badge/GitHub-Code-blue.svg" alt="GitHub"></a>
  <a href="https://www.bilibili.com/video/BV1eC4y1Z7qk/"><img src="https://img.shields.io/badge/Bilibili-Video-00A1D6.svg" alt="Bilibili"></a>
  <a href="https://youtu.be/F3Tsls_ypUU"><img src="https://img.shields.io/badge/YouTube-Video-ff0000.svg" alt="YouTube"></a> -->
</div>

<div align="center">
  <img src="IMAGE/motivations.png" width="70%">
</div>
<div align="center">
  <img src="IMAGE/partitioning.png" width="70%"> 
</div>

## Abstract
Multi-session SLAM is essential for long-term robotic operations in indoor environments such as warehouses and office buildings. However, the thin walls separating enclosed spaces in such environments introduce a challenge known as the double-sided issue, where point clouds from opposite sides are mistakenly associated as a single surface during single-session mapping, and are prone to being grouped into the same voxel during voxelization in multi-session map fusion, leading to poor voxel planarity, which causes voxel invalidation and reduces the available constraints for global optimization. To address this, we propose NVMS-SLAM, a normal vector-based multi-session LiDAR SLAM system tailored for indoor environments. For single-session mapping, an extended voxel map is designed to preserve normal vector information and to distinguish between visible and non-visible surfaces, thereby improving data association. At the multi-session level, a density-encoded indoor scan-context descriptor is introduced for robust loop closure. In addition, a two-stage global map fusion strategy is adopted, combining joint pose graph optimization and normal vector-based bundle adjustment to ensure globally consistent mapping. Experiments on simulated datasets and real-world environments demonstrate that NVMS-SLAM can effectively resolve the double-sided issue at both the single-session and multi-session stages.

**Contributors**: [Yongxin Ma](https://github.com/lian-yue0515), [Chengwei Zhao](https://github.com/chengwei0427), [Jie Xu](https://github.com/jiejie567), Yixuan Li, Xuanxuan Zhang, Shenghai Yuan,  Lihua Xie 

## 1. Prerequisites
### 1.1 Ubuntu and ROS

Ubuntu >= 18.04.

ROS >= Melodic. [ROS](http://wiki.ros.org/ROS/Installation)

### 1.2 PCL && Eigen && gtsam

PCL >= 1.8, Follow [PCL](http://www.pointclouds.org/downloads/linux.html).

Eigen >= 3.3.4, Follow [EIGEN](http://eigen.tuxfamily.org/index.php?title=Main_Page).

gtsam >= 4.0.0, Follow [gtsam](https://gtsam.org/get_started/).

### 1.3 livox_ros_driver

Follow [livox_ros_driver Installation](https://github.com/Livox-SDK/livox_ros_driver).


## 2. Build

## 3. Directly run

## 4. Rosbag Example
### 4.1 Simulated Dataset

<div align="center">
  <img src="IMAGE/Simulated.png" width="70%">
</div>

Download our test bags here: [geogle](https://drive.google.com/drive/folders/1iaKaGEEDXGvJZKw0zyqs2RxRnA0hLK1N).

### 4.2 Real-world Dataset
<div align="center">
  <img src="IMAGE/Real-world.png" width="70%"> 
</div>

Download our test bags here: [geogle](https://drive.google.com/drive/folders/1TYzT7nnJ6DlOu12cMFRslhtsvF8Fu-dj).

### 5. Example results 


### Citation
If you use NVMS-SLAM for any academic work, please cite our original [paper](https://ieeexplore.ieee.org/document/11479301)
```
@ARTICLE{11479301,
  author={Ma, Yongxin and Zhao, Chengwei and Xu, Jie and Li, Yixuan and Zhang, Xuanxuan and Yuan, Shenghai and Xie, Lihua},
  journal={IEEE Transactions on Automation Science and Engineering}, 
  title={NVMS-SLAM: Normal Vector-based Multi-Session LiDAR SLAM in Indoor Environments}, 
  year={2026},
  volume={},
  number={},
  pages={1-1},
  keywords={Kalman filters;Filters;Central Processing Unit;Indoor environment;Electronic mail;Product development;Graphical user interfaces;Indoor communication;Location awareness;High frequency;Double-sided issue;LiDAR simultaneous location and mapping;multi-session;normal vector},
  doi={10.1109/TASE.2026.3682733}}


```
### Acknowledgements 


### License 
The source code is released under [GPLv2](http://www.gnu.org/licenses/) license.


