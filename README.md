## Inspiration
在米开朗基罗的《创造亚当》中，上帝与亚当即将碰触的指尖，喻示着人类将获得感受万物的六感之一——**触觉**。

![创造亚当](https://github.com/Chenglalala/Tiouch/blob/main/image/Adam.png)

Taichi的高性能物理方针，创造了丰富的视觉盛宴，但我们想告诉你的是，Taichi能做的绝不仅仅是视觉，因此我们有了一个idea——**Taihci+Haptics**，交织出视觉和触觉的双重合奏。

![触觉与视觉交织](https://github.com/Chenglalala/Tiouch/blob/main/image/combination.png)

## Pipline
我们通过**AOT**将Taichi的kernel部署到Unity当中，在Unity中基于Taichi C API和Taichi Unity Plugin构建Taichi runtime，这样就可以在Unity里启用我们的kernel运行啦。再通过Haptics Unity Plugin，用户就可以使用Haptics力反馈设备进行触觉的交互辣。

![Pipline](https://github.com/Chenglalala/Tiouch/blob/main/image/pipline.png)



## Timeline
* 前期准备
  * Taichi编译、C API、Unity Example
* Unity场景搭建（11.30）
  * 加入Hapitc插件
  * 加入Rigid cubes
* Taichi编写物理场景(11.30-12.1)
  * 实现Rigid cubes
* Unity场景中加入Taichi rigid cubes (12.2)
* Unity加入交互 (12.3)


## Challenges
* Unity中遇到帧率降低的问题
* V1.2.0和V1.3.0 向量之间外积行为不一致
* Dynamic index 开关行为不一致
* 碰撞处理

##Future Work
* 丰富场景
  * 增加柔体、流体、绳子、布料的仿真
  * 加入更丰富的力反馈效果，比如磁力
* 增加关卡
  * 设计有挑战性的关卡，提高可玩性和趣味性
  * 增加计分功能
  * 增加力反馈显示功能
  * 在VR环境中操作
* 提高性能
  * 提高场景性能和力触觉渲染的性能
  * 优化碰撞检测和碰撞处理


