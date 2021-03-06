# 🏂[Gardener](https://github.com/SUSTech-Gardener)

This is the page for  of [SUSTech-Gardener](https://github.com/SUSTech-Gardener)😊, which is An autonomous mobile agricultural robot can collect agriculture-related information, as well as weeding and other work to serve the future agriculture. 

## Good News!
Our team has won the only reward, the prize is [DJI OSMO Mobile 4](https://www.dji.com/cn/om-4)

![image-20210621155907137](https://raw.githubusercontent.com/zhuhu00/img/master/20210621155911.png)

### Video: [Youtube](https://youtu.be/GjDMmWxaL50), [bilibili](https://www.bilibili.com/video/BV1fB4y1u7dK)

<iframe src="//player.bilibili.com/player.html?aid=588441477&bvid=BV1fB4y1u7dK&cid=350209416&page=1" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> </iframe>

[![Watch the video](https://raw.githubusercontent.com/zhuhu00/img/master/20210607141359.png)](https://youtu.be/GjDMmWxaL50)

Some picture about Gardener.

<img src="https://raw.githubusercontent.com/zhuhu00/img/master/20210606134730.png" alt="image-20210606134722046" style="zoom: 8.5%;" /> <img src="https://raw.githubusercontent.com/zhuhu00/img/master/20210606134854.png" alt="image-20210606134850746" style="zoom:8.5%;" />

<img src="https://raw.githubusercontent.com/zhuhu00/img/master/20210606134534.png" alt="image-20210606134529791" style="zoom:100%;" />

The whole project has these parts. 

## Sensors

1. Camera: Realsense D435i: [https://www.intelrealsense.com/depth-camera-d435i](https://www.intelrealsense.com/depth-camera-d435i/)
2. Lidar: Livox avia: [https://www.livoxtech.com/avia](https://www.livoxtech.com/avia)
3. Soilsensor: [https://github.com/SUSTech-Gardener/Gardener/tree/main/soilsensor](https://github.com/SUSTech-Gardener/Gardener/tree/main/soilsensor)

## [3D-solidworks](https://github.com/SUSTech-Gardener/3d-solidworks)

![image-20210607224319348](https://raw.githubusercontent.com/zhuhu00/img/master/20210607224322.png)

1. Tracked car: In order to be able to operate on multiple terrain
2. Sprinkler control
3. Car bracket
4. Soil sensor telescopic mechanism
5. Motor

# Build and Run

## 1. Prerequisties

### 1.1 Ubuntu and ROS

Ubuntu 64-bit 16.04 or 18.04. ROS Kinetic or Melodic. Follow [ROS Installation](http://wiki.ros.org/ROS/Installation).

### 1.2 Deep Learning requirements

In this part, Using YOLO V3 to detect weed and crop. The learning model we also transfer to ROS package, it is very easy to use.

- ROS package:  [https://github.com/SUSTech-Gardener/WeedDetection_ros](https://github.com/SUSTech-Gardener/WeedDetection_ros)
- Without ROS: [https://github.com/SUSTech-Gardener/WeedDetection](https://github.com/SUSTech-Gardener/WeedDetection)

### 1.3 SLAM and other

- [x] (Livox SLAM)[https://github.com/SUSTech-Gardener/car_relocalization]
- [x] (Livox Autoware)https://github.com/SUSTech-Gardener/livox_autoware_driver

## 2. Build Gardener

### 2.1 3d_solidworks in Gardener

The whole 3d solidworks model is in the [repository](https://github.com/SUSTech-Gardener/3d-solidworks), contains these items:

- A some tracked car
- Some extended structure on the car
- Base for Livox lidar and RealSense camera D435i.
- The head of the sprinkler

### 2.2 Sensors

- Livox lidar: for SLAM and navigation.
- D435i: [detect weed and crop](https://github.com/SUSTech-Gardener/WeedDetection). 
- Soil moisture sensor: add the soil moisture data in map(In **soilsensor** fold).

## 3. Run with hardware

Follow other repository in this project.

# TODO 

- [x] 购买物资（全程）
- [x] 硬件部分：小车的速度，转向控制，(第3到第12周)
- [x] 杂草识别的模型，第八周结束需要搞完（第4到第十周）
- [x] SLAM和navigation（第九到第十六周）
- [x] 机械硬件结构搭建和喷头系统的构建（第四到第十六周）
- [x] 土壤检测器的插入设计及测试（第十三周）
- [x] 最终的系统框架构建！！（✌）

## Developers:

- [Shixing Jiang](https://github.com/RiggsChiang): Mechanical design, electrical selection and layout, video clip
- [Qiaowen Wang](https://github.com/linghushaoxia-wqw): Mechanical design and tracking trolley control
- [Haibiao Chen](https://github.com/Billchan9711): electrical design and implementation, embedded system construction
- [Hu Zhu](https://github.com/zhuhu00): YOLO V3 for weed detection, coordination between components, Github Main maintenance.
- [Wen Yang](https://github.com/yangwen-1102): Mapping, positioning and system communication

# Acknowledgment

This work was supported by SUSTech Course (SDM 5002) , [Professor Xiaoping Hong](https://github.com/xiaopinghong)

Visits:
<p>
  <a href="https://count.getloli.com/"><img src="https://count.getloli.com/get/@SUSTech-Gardener"></a>
</p>
