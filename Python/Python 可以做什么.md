# Python 可以做什么

---

总所周知，Python 做爬虫很方便，有现成的库，这是很多从入门级选手到专业级选手都在做的。Python   也可以做游戏。Python 还很受黑客的青睐，在黑客领域的应用就不多说了。此外Python 做网站也无压力，比如知乎的主站后台就是基于 Python 的 $tornado$ 框架，豆瓣的后台也是基于 Python。可以不负责任地说，Python 几乎可以做任何事情。Python 还可以做桌面程序，Python 有很多 UI 库，可以很方便地完成一个 GUI 程序，比如大名鼎鼎的 Dropbox，就是用 Python 实现的服务器端和客户端程序。

## 爬虫
[Python爬虫基础](https://segmentfault.com/a/1190000008191015)
python爬虫基础知识，至此足够，接下来，在实战中学习更高级的知识。      

[精通Python网络爬虫(0):网络爬虫学习路线](https://segmentfault.com/a/1190000010160830)
随着大数据时代的到来，人们对数据资源的需求越来越多，而爬虫是一种很好的自动采集数据的手段。
那么，如何才能精通Python网络爬虫呢？学习Python网络爬虫的路线应该如何进行呢？        

[Python爬虫使用Selenium+PhantomJS抓取Ajax和动态HTML内容](https://segmentfault.com/a/1190000005151856)
在上一篇python使用xslt提取网页数据中，要提取的内容是直接从网页的source code里拿到的。但是一些Ajax动态内容是在source code找不到的，就要找合适的程序库把异步或动态加载的内容加载上来，交给本项目的提取器进行提取。
python可以使用selenium执行javascript，selenium可以让浏览器自动加载页面，获取需要的数据。selenium自己不带浏览器，可以使用第三方浏览器如Firefox，Chrome等，也可以使用headless浏览器如PhantomJS在后台执行。       

[Python爬虫项目整理](https://segmentfault.com/p/1210000009117809/read)      

爬虫实战系列
[Python爬虫实战（1）：爬取Drupal论坛帖子列表](https://segmentfault.com/a/1190000005654753)
[Python爬虫实战（2）：爬取京东商品列表](https://segmentfault.com/a/1190000005672011)
[Python爬虫实战（3）：安居客房产经纪人信息采集](https://segmentfault.com/a/1190000005929693)
[Python爬虫实战（4）：豆瓣小组话题数据采集—动态网页](https://segmentfault.com/a/1190000005972283)
      
## Web 程序开发
[开始Tornado的源码分析之旅](https://segmentfault.com/a/1190000003812354)
Tornado 是由 Facebook 开源的一个服务器“套装”，适合于做 python 的 web 或者使用其本身提供的可扩展的功能，完成了不完整的 wsgi 协议，可用于做快速的 web 开发，封装了 epoll 性能较好。文章主要以分析 tornado 的网络部分即异步事件处理与上层的 IOstream 类提供的异步IO，其他的模块如 web 的 tornado.web 以后慢慢留作分析。          

[tornado 源码阅读-初步认识](https://segmentfault.com/a/1190000002971992)
最近闲暇无事,阅读了一下tornado的源码,对整体的结构有了初步认识,与大家分享        

[我心中的 tornado 最佳实践](https://segmentfault.com/a/1190000008650442)
最近开发新项目一直在学习tornado的知识，在前人的基础上找了些最佳实践，记录如下，备查。       

Tornado 简单入门教程:
[Tornado 简单入门教程（零）——准备工作](https://segmentfault.com/a/1190000002703128)
这两天在学着用Python + Tornado +MongoDB来做Web开发（哈哈哈这个词好高端）。学的过程中查阅了无数资料，也收获了一些经验，所以希望总结出一份简易入门教程供初学者参考。完整的教程将尽可能（233）遵循下面的目录顺序。
[Tornado 简单入门教程（一）——Demo1](https://segmentfault.com/a/1190000002703321)
Demo1是一个简单的博客系统（=。=什么网站都叫系统）。我们从这个简单的系统入手，去了解P+T+M网站的内部逻辑，并记住一些“规则”，方便我们进一步自己开发。      

[Tornado 简单入门教程（二）——Demo2](https://segmentfault.com/a/1190000002705416)
在Demo1里面,我们练习了如何部署应用、tornado框架的基本结构以及应用如何处理请求。
其实Demo1算不上一个博客啦。一个最基本的信息系统一定要包含对数据库的增、删、改和查。所以这次，我们来将Demo1升级为Demo2，添加上基本的增删改查。          

## 图像与视频处理
一直断断续续的用过几次 OpenCV，感觉熟练掌握它的使用方法已经变的非常必要了，正好找到一个很不错的英文教程，就以此为起点，详细记录一下对 OpenCV 的学习过程吧。
准备工作
[安装Python OpenCV](https://segmentfault.com/a/1190000003742411)
### 图像处理
[第一节：图像基本操作](https://segmentfault.com/a/1190000003742422)     

[第二节：滤镜和图像运算](https://segmentfault.com/a/1190000003742433)   

[第三节：图像像素点操作](https://segmentfault.com/a/1190000003742442)       

[第四节：图像直方图和反向投影](https://segmentfault.com/a/1190000003742455)       

[第五节：图像中边界和轮廓检测](https://segmentfault.com/a/1190000003742455)       

[第六节：对象识别](https://segmentfault.com/a/1190000003755089)         

[第七节：图像灰度化处理](https://segmentfault.com/a/1190000003755100)        

[第八节：图像二值化处理(https://segmentfault.com/a/1190000003755100)             

### 视频处理
- 第一节：[输入输出](https://segmentfault.com/a/1190000003804797)
- 第二节：[视频处理](https://segmentfault.com/a/1190000003804807)
- 第三节：[标记运动轨迹](https://segmentfault.com/a/1190000003804820)
- 第四节：[运动检测](https://segmentfault.com/a/1190000003804835)
- 第五节：[运动方向判断](https://segmentfault.com/a/1190000003804867)


## 科学计算
[数据科学部门如何使用Python和R组合完成任务](https://segmentfault.com/a/1190000005053687)
和那些数据科学比赛不同，在真实的数据科学中，我们可能更多的时间不是在做算法的开发，而是对需求的定义和数据的治理。所以，如何更好的结合现实业务，让数据真正产生价值成了一个更有意义的话题。
数据科学项目的完整流程通常是这样的五步骤：
需求定义=》数据获取=》数据治理=》数据分析=》数据可视化     

[Python科学计算利器——Anaconda](https://segmentfault.com/a/1190000000591312)
最近在用Python做中文自然语言处理。使用的IDE是PyCharm。PyCharm确实是Python开发之首选，但用于科学计算方面，还略有欠缺。为此我尝试过Enthought Canopy，但Canopy感觉把问题搞得复杂化，管理Python扩展也不太方便。直到今天我发现了Anaconda。
Anaconda是一个和Canopy类似的科学计算环境，但用起来更加方便。自带的包管理器conda也很强大。

## 数据分析
[使用Python一步一步地来进行数据分析](https://segmentfault.com/a/1190000004839710)
你学习Python时能犯的最简单的错误之一就是同时去尝试学习过多的库。当你努力一下子学会每样东西时，你会花费很多时间来切换这些不同概念之间，变得沮丧，最后转移到其他事情上。
所以，坚持关注这个过程：
理解 Python 基础
学习 Numpy
学习 Pandas
学习 Matplolib          
[numpy：python数据领域的功臣](https://segmentfault.com/a/1190000006912539)
numpy对python的意义非凡，在数据分析与机器学习领域为python立下了汗马功劳。现在用python搞数据分析或机器学习经常使用的pandas、matplotlib、sklearn等库，都需要基于numpy构建。毫不夸张地说，没有numpy，python今天在数据分析与机器学习领域只能是捉襟见肘。         

## 机器学习
[0x01 念念Python，必有回响](https://segmentfault.com/a/1190000004230792)
真若有心于数据领域，甚或欲从事数据科学之职业。请对Python有信心，值得你付出时间。想走机器学习之路，Scikit-learn是你最好的选择，一边操作实例，一边阅读文档，再辅助以相关的理论基础，持之数日，则大业可成也。        

[Python机器学习工具：Scikit-Learn介绍与实践](https://segmentfault.com/a/1190000008764845)
官方的解释很简单: Machine Learning in Python, 用python来玩机器学习。
Scikit-learn的优点：
构建于现有的NumPy(基础n维数组包)，SciPy(科学计算基础包), matplotlib(全面的2D/3D画图)，IPython(加强的交互解释器)，Sympy(Symbolic mathematics)， Pandas(数据结构和分析)之上，做了易用性的封装。
简单且高效的数据挖掘、数据分析的工具。
对所有人开放，且在很多场景易于复用。
BSD证书下开源。     

[教程 | 如何用Python和机器学习炒股赚钱？](https://segmentfault.com/p/1210000010054515/read)
相信很多人都想过让人工智能来帮你赚钱，但到底该如何做呢？瑞士日内瓦的一位金融数据顾问 Gaëtan Rickter 近日发表文章介绍了他利用 Python 和机器学习来帮助炒股的经验，其最终成果的收益率跑赢了长期处于牛市的标准普尔 500 指数。虽然这篇文章并没有将他的方法完全彻底公开，但已公开的内容或许能给我们带来如何用人工智能炒股的启迪。机器之心对本文进行了编译介绍，代码详情请访问原文。        

[欧拉函数(Euler' totient function )](https://segmentfault.com/a/1190000010301273)
gamma函数的求导会出现所谓的欧拉函数（phi），在一篇论文中我需要对好几个欧拉函数求值，结果不能理解，立即去google，发现了一个开源的python库可以用来计算欧拉函数            

[Python 机器学习入门资料整理](https://segmentfault.com/a/1190000004285821)
