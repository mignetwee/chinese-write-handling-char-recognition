# chinese-write-handling-char-recognition
汉字手写识别

## 数据集
数据集来自于中科院自动化研究所，具体下载地址:
``http://www.nlpr.ia.ac.cn/databases/download/feature_data/HWDB1.1trn_gnt.zip``
``http://www.nlpr.ia.ac.cn/databases/download/feature_data/HWDB1.1tst_gnt.zip``

这个训练集和测试集是经过压缩的图片，需要解压出来转换图片，这里是转换好的文件包：https://pan.baidu.com/s/1o84jIrg
![数据集](https://github.com/Mignet/chinese-write-handling-char-recognition/blob/master/pic/%E6%95%B0%E6%8D%AE%E9%9B%86.png)
## 构建神经网络
![网络](https://github.com/Mignet/chinese-write-handling-char-recognition/blob/master/pic/png.png?raw=true)

## 训练
run the command ``python chinese_rec.py --mode=train --max_steps=16002 --eval_steps=100 --save_steps=500``

## 模型评估
run the command ``python chinese_rec.py --mode=validation``
![accuracy](https://github.com/Mignet/chinese-write-handling-char-recognition/blob/master/pic/accuracy.png)
## 测试
把要识别的图像丢到tmp目录下就行了
run the command ``python chinese_rec.py --mode=inference``
![result](https://github.com/Mignet/chinese-write-handling-char-recognition/blob/master/pic/result.png)

