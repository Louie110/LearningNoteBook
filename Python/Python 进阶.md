
[[原] Python 开发者面向文档编程的正确姿势](https://segmentfault.com/a/1190000007055844)

在实际生产中，机器学习工作现在看起来，白天像是个算法工程师的活，晚上就变成运维+测试了。Python 一直以来也都受到测试工程师和运维工程师的偏爱，下面是几个经典的注释活用case。

[[译]让你的Python代码优雅又地道](https://segmentfault.com/p/1210000009953445/read)

在Python社区文化的浇灌下，演化出了一种独特的代码风格，去指导如何正确地使用Python，这就是常说的pythonic。一般说地道(idiomatic)的python代码，就是指这份代码很pythonic。Python的语法和标准库设计，处处契合着pythonic的思想。而且Python社区十分注重编码风格一的一致性，他们极力推行和处处实践着pythonic。所以经常能看到基于某份代码P vs NP (pythonic vs non-pythonic)的讨论。pythonic的代码简练，明确，优雅，绝大部分时候执行效率高。阅读pythonic的代码能体会到“代码是写给人看的，只是顺便让机器能运行”畅快。

[python高级特性](https://segmentfault.com/a/1190000010280700)
> python语言的一些高阶用法主要有以下几个特性：
generators生成器用法
collections包常见用法
itertools包常见用法
packing/unpacking封包/解包特性
Decorators装饰器
Context Managers上下文管理期
以上几个特性我会针对应用场景，使用注意事项，应用举例几个维度分别进行讲解，如果有同学对某个特性特别熟悉则可以直接跳过。


[深入浅出地，彻彻底底地理解python中的编码](https://segmentfault.com/p/1210000010035983/read)
>python处理文本的功能非常强大，但是如果是初学者，没有搞清楚python中的编码机制，也经常会遇到乱码或者decode error。本文的目的是简明扼要地说明python的编码机制，并给出一些建议。

[Python装饰器为什么难理解？](https://segmentfault.com/p/1210000009900857/read)
无论项目中还是面试都离不开装饰器话题，装饰器的强大在于它能够在不修改原有业务逻辑的情况下对代码进行扩展，权限校验、用户认证、日志记录、性能测试、事务处理、缓存等都是装饰器的绝佳应用场景，它能够最大程度地对代码进行复用。

[众里寻她千百度--正则表达式](https://segmentfault.com/a/1190000000644426)
简单来说，正则表达式就是用来匹配特定内容的字符串。举个例子来讲，如果我想找出由a、b组成的，以abb结尾的字符串，比如ababb，那么用正则表达式来表示就是[ab]*abb。

[【Python3】Python面向对象的程序设计](https://segmentfault.com/a/1190000009817047)
>python中一切皆为对象，且python3统一了类与类型的概念，类型就是类。
基于面向对象设计一个款游戏：英雄联盟，每个玩家选一个英雄，每个英雄都有自己的特征和和技能，特征即数据属性，技能即方法属性，特征与技能的结合体就一个对象。
从一组对象中提取相似的部分就是类，类所有对象都具有的特征和技能的结合体。
在python中，用变量表示特征，用函数表示技能，因而类是变量与函数的结合体，对象是变量与方法（指向类的函数）的结合体。

[Python源码理解: '+=' 和 'xx = xx + xx'的区别](https://segmentfault.com/a/1190000009764209)
现在我们大概明白了+=实际上是干嘛了: 它应该能算是一个加强版的+, 因为它比+多了一个写回本身的功能.不过是否能够写回本身, 还是得看对象自身是否支持, 也就是说是否具备Py_NotImplemented标识, 是否支持sq_inplace_concat, 如果具备, 才能实现, 否则, 也就是和 + 效果一样而已.

[那些有趣/用的 Python 库](https://segmentfault.com/a/1190000010103386)

[Python拾遗（一）](https://segmentfault.com/a/1190000005872845)
