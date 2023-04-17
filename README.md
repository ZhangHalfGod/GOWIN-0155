# GOWIN-0155
Recognition and tracking of high-speed moving objects based on GW2A
# project introduce
设计方案：使用RISC-V架构的gowin ip软核，在GoAI平台在板上部署CNN来运行深度训练过的模型，GoAI扩展了TensorFlow软件开发环境，部分神经网络模型可以直接引用，其他用opencv和numpy工具，传统方式是利用目标的特征点进行匹配，但是opencv已经引入了接口使用，用三个操作：特征提取(feature extraction)、特征匹配(feature matching)、目标识别(Object Detection)提升，特征提取(feature extraction)，用SIFT算法，Opencv SIFT函数库，实现。第二步，使用TinyMaix框架将学习后的目标二次推理后，输入到资源有限的板上。
实现功能：通过舵机移动led屏，通过返回的信息，舵机带动led识别目标，同时输出深度学习的实时信息。
