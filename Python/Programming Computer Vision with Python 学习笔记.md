《Programming Computer Vision with Python》是一本介绍计算机视觉底层基本理论和算法的入门书，通过这本收可以学到有关对象识别、基于内容的图像搜索、光学字符识别、光流法、跟踪、三维重建、立体成像、增强现实、姿态估计、全景创建、图像分割、降噪、图像分组等技术的实现原理。

[英文版PDF下载](https://it-ebooks.info/book/836/)
[中文版介绍](https://book.douban.com/subject/25906843/)


1. [Programming Computer Vision with Python （学习笔记一）](https://segmentfault.com/a/1190000003941588)
先介绍基本的图像处理，包括图像的读取、转换、缩放、导数计算、画图和保存，这些知识将为后面内容的学习打下基础。        

2. [Programming Computer Vision with Python （学习笔记二）](https://segmentfault.com/a/1190000003946953)      

首先介绍跟图像处理、显示有关两个库：NumPy和Matplotlib，然后介绍增强图像对比度的实现原理。      

3. [Programming Computer Vision with Python （学习笔记三）](https://segmentfault.com/a/1190000003950550)    
原书对于PCA的讲解只有一小节，一笔带过的感觉，但我发现PCA是一个很重要的基础知识点，在机器机视觉、人脸识别以及一些高级图像处理技术时都被经常用到，所以本人自行对PCA进行了更深入的学习。       

4. [Programming Computer Vision with Python （学习笔记四）](https://segmentfault.com/a/1190000003989791)
上一个笔记主要是讲了PCA的原理，并给出了二维图像降一维的示例代码。但还遗留了以下几个问题：

在计算协方差和特征向量的方法上，书上使用的是一种被作者称为compact trick的技巧，以及奇异值分解（SVD），这些都是什么东西呢？
如何把PCA运用在多张图片上？         
    
所以，我们需要进一步的了解，同时，为示例对多张图片进行PCA，我选了一个跟书相似但更有趣的例子来做——人脸识别。        
5. [Programming Computer Vision with Python （学习笔记五）](https://segmentfault.com/a/1190000004002685)

SciPy库，与之前我们使用的NumPy和Matplotlib，都是scipy.org提供的用于科学计算方面的核心库。相对NumPy，SciPy库提供了面向更高层应用的算法和函数(其实也是基于NumPy实现的），并以子模块的形式组织，每个子模块对应不同的应用领域。          

6. [Programming Computer Vision with Python （学习笔记六）](https://segmentfault.com/a/1190000004033826)
边缘检测（edge detection）是最重要的图像处理技术之一，图像边缘检测大幅度地减少了数据量，并且剔除了可以认为不相关的信息，保留了图像重要的结构属性，为后续图像理解方法提供了基础。

7. [Programming Computer Vision with Python （学习笔记七）](https://segmentfault.com/a/1190000004048075)
数学形态学（mathematical morphology）关注的是图像中的形状，它提供了一些方法用于检测形状和改变形状。起初是基于二值图像提出的，后来扩展到灰度图像。二值图像就是：每个像素的值只能是0或1，1代表描绘图像的点，0代表背景。

基本的形态学运算包括：腐蚀（erosion）、膨胀（dilation）、开（opening）、闭（closing），对于这些运算，都需要用到被称为结构元素(Structuring element)的模板，一般为方形，以小矩阵的形式表示，但它的元素的值只能是0或1，它代表的是一个集合，这个集合罩在原图像上，可以跟原图像的形状进行集合运算。

8. [Programming Computer Vision with Python （学习笔记八）](https://segmentfault.com/a/1190000004051795)

图像去噪(Image Denoising)的过程就是将噪点从图像中去除的同时尽可能的保留原图像的细节和结构。这里讲的去噪跟前面笔记提过的去噪不一样，这里是指高级去噪技术，前面提过的高斯平滑也能去噪，但高斯平滑去噪的同时也把边缘模糊化了，另外使用形态学的方法去噪是指去除一些粗的椒盐噪声。对于一幅密布噪点的图像，如果使其变得清晰又保留边缘细节，这是高级去噪技术所要解决的问题。          

9. [Programming Computer Vision with Python （学习笔记九）](https://segmentfault.com/a/1190000004055633)
角检测（Corner detection）是指检测图像中具有代表性的（我们感兴趣的）角点，一般讲为形状或边缘的拐角处，这些点可以大略标记对象在图像中的轮廓和位置，如果从一个图像序列中检测每个图像的角点，就可以找出图像之间存在的相关和相对应的角点，这对比如全景拼接（多张图片拼接成一张全景图片）很有用。
角检测还可以用在运动检测、物体识别等方面。       

10. [Programming Computer Vision with Python （学习笔记十）](https://segmentfault.com/a/1190000004091583)
现在考虑一个全景图拼接的应用场景，假设现有两张图片需要拼接成一张全景图，这两张图片是通过相机右转一定角度拍摄出来的，两张图片有部分取景是重叠的。如何实现拼接？当然这是一个不简单的问题，我们现在只考虑实现拼接目标的第一步：找出图像中重叠的内容，以及分别在两张图片中的位置。        

11. [Programming Computer Vision with Python （学习笔记十一）](https://segmentfault.com/a/1190000004149225)
尺度不变特征变换(Scale-invariant feature transform， 简称SIFT)是图像局部特征提取的现代方法——基于区域/图像块的分析。在上篇笔记里我们使用的图像之间对应点的匹配方法，不适用于不同尺度的图像。有许多应用场景需要对不同尺度（即分辨率、缩放、旋转角度、亮度等都可能存在不同）的图像进行特征识别和匹配，这就需要一种特征提取方法，通过这种方法提取出来的特征描述，可以不受尺度的影响，SIFT算法就是这种方法的实现。

SIFT算法的应用非常广泛，包括物体识别、机器人地图感知与导航、全景拼接、3D建模、手势识别、影像追踪和动作比对等,原书后面章节的算法也会多次用到它。SIFT算法的过程较复杂，本文只是粗略介绍其关键步骤，以便引出SURF——基于SIFT的改进算法。        

12. [Programming Computer Vision with Python （学习笔记十二）](https://segmentfault.com/a/1190000004200111) 
ORB（Oriented FAST and Rotated BRIEF）可用来替代SIFT（或SURF），它对图像更具有抗噪特性，是一种特征检测高效算法，其速度满足实时要求，可用于增强图像匹配应用。

ORB的算法基于FAST角检测（Features from accelerated segment test）和BRIEF(Binary Robust Independent Elementary Features)特征描述符，这也是它名字的由来。
