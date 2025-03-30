本压缩包结构如下
dataset_for_DL_course
├ dataset
   ├ phantom_input_train.npy 2000组噪声模拟图，用于训练神经网络，形状为(2000, 2, 256, 256)
   ├ phantom_target_train.npy 2000组无噪声模拟图，为上述噪声图像一一对应的理想图像，用于训练神经网络, 形状为(2000, 2, 256, 256)
   ├ phantom_input_test.npy 25组噪声模拟图，用于测试神经网络，形状为(25, 2, 256, 256)
   └ real_input_test.npy 25组噪声图，来源于真实医疗数据集，用于测试神经网络，形状为(25, 2, 256, 256)
├ example
   ├ example_train.png 训练数据示例
   ├ example_test_phantom.png 测试模拟图数据示例
   └example_test_real.png 测试真实数据示例
└ readme.txt

数据集读取示例：
import numpy
phantom_input_train = numpy.load('path-to-your-dataset/dataset/phantom_input_train.npy')