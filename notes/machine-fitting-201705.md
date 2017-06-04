Machine Fitting
==================

我们来聊一聊机器学习到底是什么。

识别图像中的文字，物体，语音转文字，无人驾驶，更高级一点的客服助手，如果从抽象的角度上来看，都可以看做是一种功能，
简化为完成一个特定的任务，给出特定的数据，即输入，要得到特定的结果，即输出，如果用专业的术语来讲，都可以称为一种 函数。

那什么是学习呢？学习是找到这样一个函数的过程，该函数可以最好的完成这个任务。函数不是从零找起，事先会给出一个大概的模型。

Given a specific task to solve, and a class of functions F, learning means
using a set of observations to find f* in F which solves the task in some optimal sense. cost(*f) 最低最优

However, using them is not so straightforward, and a relatively good understanding of the underlying
theory is essential.

X -> Y 是一个极其复杂的函数，专业模型极为重要。可以把这个过程称为learning，但calibrating或fitting似乎更为合适，
中文可以称为 拟合 。就像看着样本捏泥塑模型一样，第一次不像没关系，修修补补就够了。类似于傅里叶分解任何一个多项式函数。

使用nn的目的：人工实现这个复杂函数近乎不可能，希望通过计算机处理大量数据，得到足够好的拟合。给定输入，根据输出是否正确
调节函数的内部参数，可以把它理解为一个具有很多参数的黑盒，只要你找到正确的参数。因为计算量巨大，数据量巨大，只有最新的
GPU才使之成为可能。


所有计算机程序都是可拟合的吗？可以用计算机语言实现的算法，都是可拟合的。

```
  X  ->
      prepare ALGO
          prepare PL
              prepare CPU
                          -> Y
```
这被称为 https://en.wikipedia.org/wiki/Universal_approximation_theorem


Perception or Cognition
-----------------------------

视觉，听觉都是关于模型的。模式识别与认知的区别。machine fitting 可以胜任模式识别的工作，但是更重要的机器认知呢? 
识别出物体，理解物体背后的隐含，关联的意义呢

https://en.wikipedia.org/wiki/Perception
https://en.wikipedia.org/wiki/Cognition


不但要给出特定的输出，还要理解这个输出的意义，比如图中的物体是苹果，苹果是一种水果，苹果可以吃，苹果也可以拿来打人
等等，这就比图像识别更进了一层。

附:

Andrew Ng 博士课程视频 http://www.bilibili.com/video/av6949929/

阿里闵万里：有个现象，叫深度泛滥；有种AI公司，叫伪创业 https://www.huxiu.com/article/192867.html