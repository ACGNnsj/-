<h1 align = "center">Final Project——Start with random walk</h1>

<div align=center>
倪世杰 2014301020001
</div>

---

**[摘要]**

**[关键词]**


###1. 引言



###2. 背景介绍

* **随机游走**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;随机游走是描述由一系列随机步骤组成的路线的数学对象。例如，一个分子在液体或气体中前进的路线，动物的觅食路线，超弦行为，一支波动的股票的价格以及一个赌徒的财务状况都可以通过随机游走模型近似,，即使事实上他们可能不是随机的。如这些例子所示，随机游走在许多科学领域都有应用，包括生态学、心理学、计算科学、物理学、化学和生物学，同时也有经济学。随机游走揭示了这些领域中许多过程中被观测到的行为，因此它作为一个已记录的随机活动的基础模型。作为一个更偏数学的应用， 在基于主体的建模环境中，π的值可以通过使用随机行走近似得出。随机行走这个术语最早被英国数学家、生物统计学家卡尔·皮尔逊于1905年提出。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在很多系统都存在不同类型的随机游走，他们都具有相似结构。单个的随机事件我们不可预测，但随机大量的群体行为，却是精确可知的，这就是概率世界的魅力，在偶然中隐含着必然。随机性造成了低尺度下的差异性，但在高尺度下又表现为共同的特征的相似性。按照概率的观点“宇宙即是所有随机事件概率的总和”。

<div align=center><img src="https://github.com/ACGNnsj/-/blob/master/Final%20Project/quantum_cloud_front_775.jpg?raw=true" /></div>

<div align=center>雕塑家安东尼·葛姆雷使用随机游走算法创作的雕塑——《量子云》</div>

* **自回避随机游走**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在数学上，自回避随机游走（SAW）是指在网格上一系列重复经过同一个点的一系列移动。自回避多边形（SAP） 则是指网格上一个封闭的自回避随机游走的路径。自回避随机游走最早被保罗·弗洛里提出用来模拟链状实体比如溶剂和聚合物的真实行为，它们拥有的体积禁止在空间同一个点上有多个物体。尽管物理学家提出了许多有数值模拟强力支持并被认为是正确的猜想，但是从数学角度来说，我们对自回避随机游走了解非常少。

<div align=center><img src="https://github.com/ACGNnsj/-/blob/master/Final%20Project/knot_3a_blog.jpg?raw=true" /></div>

<div align=center>一种自回避多边形</div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;在计算物理中，自回避随机游走是一个二维或三维欧几里得空间中有固定节点数和步长的链状路线，并且其被禁止穿过自身或其他路线。一个自回避随机游走系统满足所谓的排斥体积条件。在更高维度中，自回避随机游走被认为行为更像原本的随机游走。自回避随机游走和自回避多边形在模型化如蛋白质的线状或环状分子的拓扑和纽结理论行为时起到核心作用。自回避随机游走是分形的。例如，在二维空间中，分形维数是<a href="http://www.codecogs.com/eqnedit.php?latex=\frac{4}{3}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\frac{4}{3}" title="\frac{4}{3}" /></a>，三维空间中，分形维数接近<a href="http://www.codecogs.com/eqnedit.php?latex=\frac{5}{3}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\frac{5}{3}" title="\frac{5}{3}" /></a>，在四维和更高维空间中，分形维数为<a href="http://www.codecogs.com/eqnedit.php?latex=2" target="_blank"><img src="http://latex.codecogs.com/gif.latex?2" title="2" /></a>。这个维数被称为上临界维数，当超过这个维数时排斥体积是微不足道的。

<div align=center><img src="https://github.com/ACGNnsj/-/blob/master/Final%20Project/HK4nV.jpg?raw=true" /></div>

<div align=center>三维点阵自回避随机游走</div>

* **扩散**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;分子扩散，通常简称为扩散，是分子通过随机分子运动从高浓度（或高化学势）区域向低浓度（或低化学势）区域的网状的传播。扩散的结果是物质缓慢地混合起来。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;扩散现象是分子的内迁移现象。从微观上分析是大量分子做无规则热运动时，分子之间发生相互碰撞的结果。由于不同空间区域的分子密度分布不均匀，分子发生碰撞的情况也不同。这种碰撞迫使密度大的区域的分子向密度小的区域转移，最后达到均匀的密度分布。</font>

<div align=center><img src="https://github.com/ACGNnsj/-/blob/master/Final%20Project/Blausen_0315_Diffusion.png?raw=true" /></div>

<div align=center>颜料在水中的扩散</div>

* **扩散定律**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;扩散以一个初始分布释放大量的无规则行走，观察他们的密度就会得到分布函数。1855年法国生理学家阿道夫·菲克提出了描述扩散规律的基本公式——菲克定律。

<div align=center><img src="https://github.com/ACGNnsj/-/blob/master/Final%20Project/DiffusionMicroMacro.gif?raw=true" /></div>

<div align=center>不同尺度下观察到的扩散过程</div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;菲克第一定律假设从高浓度区域往低浓度流的通量大小与浓度梯度（空间导数）成正比，通过这个假设，菲克第一定律把扩散通量与浓度联系起来。在一维空间下的菲克第一定律如下：

<div align=center><a href="http://www.codecogs.com/eqnedit.php?latex=J=-D\frac{\partial&space;\phi&space;}{\partial&space;x}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?J=-D\frac{\partial&space;\phi&space;}{\partial&space;x}" title="J=-D\frac{\partial \phi }{\partial x}" /></a></div>

其中，<a href="http://www.codecogs.com/eqnedit.php?latex=J" target="_blank"><img src="http://latex.codecogs.com/gif.latex?J" title="J" /></a>为“扩散通量”（于某单位时间内通过某单位面积的物质量），<a href="http://www.codecogs.com/eqnedit.php?latex=J" target="_blank"><img src="http://latex.codecogs.com/gif.latex?J" title="J" /></a>为扩散系数或扩散度，<a href="http://www.codecogs.com/eqnedit.php?latex=\phi" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\phi" title="\phi" /></a>为浓度（假设为理想混合物）。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;根据斯托克斯-爱因斯坦关系，<a href="http://www.codecogs.com/eqnedit.php?latex=D" target="_blank"><img src="http://latex.codecogs.com/gif.latex?D" title="D" /></a>的大小取决于温度、流体黏度与分子大小，并与扩散分子流动的平均速度平方成正比。

在二维或以上的情况下，我们必须使用<a href="http://www.codecogs.com/eqnedit.php?latex=\nabla" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\nabla" title="\nabla" /></a>来把第一导数通用化，得

<div align=center><a href="http://www.codecogs.com/eqnedit.php?latex=J=-D\nabla\phi" target="_blank"><img src="http://latex.codecogs.com/gif.latex?J=-D\nabla\phi" title="J=-D\nabla\phi" /></a></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;菲克第二定律预测扩散会如何使得浓度随时间改变：

<div align=center><a href="http://www.codecogs.com/eqnedit.php?latex=\frac{\partial&space;\phi&space;}{\partial&space;t}=D\frac{\partial&space;^{2}\varphi&space;}{\partial&space;x^{2}}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\frac{\partial&space;\phi&space;}{\partial&space;t}=D\frac{\partial&space;^{2}\varphi&space;}{\partial&space;x^{2}}" title="\frac{\partial \phi }{\partial t}=D\frac{\partial ^{2}\varphi }{\partial x^{2}}" /></a></div>

对于二维或以上的扩散，其菲克第二定律为：

<div align=center><a href="http://www.codecogs.com/eqnedit.php?latex=\frac{\partial&space;\phi&space;}{\partial&space;t}=D\nabla^{2}\varphi" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\frac{\partial&space;\phi&space;}{\partial&space;t}=D\nabla^{2}\varphi" title="\frac{\partial \phi }{\partial t}=D\nabla^{2}\varphi" /></a></div>

其形式跟热传导方程类似。

* **熵**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;化学及热力学中所指的熵，是一种测量在动力学方面不能做功的能量总数，也就是当总体的熵增加，其做功能力也下降，熵的量度正是能量退化的指标。熵亦被用于计算一个系统中的失序现象，也就是计算该系统混乱的程度。熵是一个描述系统状态的函数，但是经常用熵的参考值和变化量进行分析比较，它在控制论、概率论、数论、天体物理、生命科学等领域都有重要应用，在不同的学科中也有引申出的更为具体的定义，是各领域十分重要的参量。

<div align=center><img src="https://github.com/ACGNnsj/-/blob/master/Final%20Project/entropy.jpg?raw=true" /></div>

<div align=center>熵增过程</div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1877年，玻尔兹曼发现单一系统中的熵跟构成热力学性质的微观状态数量相关。可以考虑情况如：一个容器内的理想气体。微观状态可以以每个组成的原子的位置及动量予以表达。为了一致性起见，我们只需考虑包含以下条件的微观状态：（i）所有粒子的位置皆在容器的体积范围内；（ii）所有原子的动能总和等于该气体的总能量值。玻尔兹曼提出一个系统的熵和所有可能微观状态的数目满足以下简单关系：

<div align=center><a href="http://www.codecogs.com/eqnedit.php?latex=S=k\ln\Omega" target="_blank"><img src="http://latex.codecogs.com/gif.latex?S=k\ln\Omega" title="S=k\ln\Omega" /></a></div>

这个公式称为“玻尔兹曼公式”，其中<a href="http://www.codecogs.com/eqnedit.php?latex=k" target="_blank"><img src="http://latex.codecogs.com/gif.latex?k" title="k" /></a>是玻尔兹曼常数，<a href="http://www.codecogs.com/eqnedit.php?latex=\Omega" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\Omega" title="\Omega" /></a>则为系统宏观状态中所包含的微观状态总数。根据玻尔兹曼的定义，熵是一则关于状态的函数。并且因为<a href="http://www.codecogs.com/eqnedit.php?latex=\Omega" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\Omega" title="\Omega" /></a>是一个自然数（1,2,3,...），熵必定是个非负数。根据这个公式，我们可以将熵看作是一个系统“混乱程度”的度量，因为一个系统越混乱，可以看作是微观状态分布越均匀。根据熵的统计学定义，热力学第二定律说明一个孤立系统的倾向于增加混乱程度。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;可以严格证明，玻尔兹曼公式的另一种等价表述形式是

<div align=center><a href="http://www.codecogs.com/eqnedit.php?latex=S=-k\sum_{s}^{&space;}P_{s}\ln&space;P_{s}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?S=-k\sum_{s}^{&space;}P_{s}\ln&space;P_{s}" title="S=-k\sum_{s}^{ }P_{s}\ln P_{s}" /></a></div>

其中<a href="http://www.codecogs.com/eqnedit.php?latex=s" target="_blank"><img src="http://latex.codecogs.com/gif.latex?s" title="s" /></a>标记所有可能的微观态， <a href="http://www.codecogs.com/eqnedit.php?latex=P_{s}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?P_{s}" title="P_{s}" /></a>表示微观态<a href="http://www.codecogs.com/eqnedit.php?latex=s" target="_blank"><img src="http://latex.codecogs.com/gif.latex?s" title="s" /></a>的出现几率。

###3. 正文

#### Ⅰ 点阵随机游走

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;一个最流形的随机游走模型就是规则点阵上的随机游走，在这个模型中，每一步对象的位置根据某种概率分布从一个阵点跳跃到另一个阵点上。这种简化使问题更易处理又不失一般性，故我们接下来主要研究该种模型。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;其中最简单的情形就是一个行人以固定步幅在一条直线上等概率地沿两个方向之一行走。为使结果更具普遍性，我们假设同时有若干人在随机游走，研究他们走完每一步后与原点之间的平均距离。

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;显然，实现该程序的关键是如何模拟行人们等几率的向两个方向行走。我们可以通过产生一个介于<a href="http://www.codecogs.com/eqnedit.php?latex=0" target="_blank"><img src="http://latex.codecogs.com/gif.latex?0" title="0" /></a>和<a href="http://www.codecogs.com/eqnedit.php?latex=1" target="_blank"><img src="http://latex.codecogs.com/gif.latex?1" title="1" /></a>之间的随机数<a href="http://www.codecogs.com/eqnedit.php?latex=r" target="_blank"><img src="http://latex.codecogs.com/gif.latex?r" title="r" /></a>来实现：若<a href="http://www.codecogs.com/eqnedit.php?latex=r<0.5" target="_blank"><img src="http://latex.codecogs.com/gif.latex?r<0.5" title="r<0.5" /></a>，则行人向右走一步，否则行人向左走一步。

#### →[查看程序](https://github.com/ACGNnsj/-/blob/master/Final%20Project/Final%20Project1-1.py)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;我们取行人人数为10000，模拟三次得如下结果

<div align=center><img src="https://github.com/ACGNnsj/-/blob/master/Final%20Project/figure_1-1.png?raw=true" /></div>

可以看出10000名行人的平均位移<a href="http://www.codecogs.com/eqnedit.php?latex=\overline{x}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\overline{x}" title="\overline{x}" /></a>在<a href="http://www.codecogs.com/eqnedit.php?latex=0" target="_blank"><img src="http://latex.codecogs.com/gif.latex?0" title="0" /></a>附近波动且波动幅度随<a href="http://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="http://latex.codecogs.com/gif.latex?n" title="n" /></a>增大，但<a href="http://www.codecogs.com/eqnedit.php?latex=\overline{x}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\overline{x}" title="\overline{x}" /></a>的期望值大致为<a href="http://www.codecogs.com/eqnedit.php?latex=0" target="_blank"><img src="http://latex.codecogs.com/gif.latex?0" title="0" /></a>，这是由于

<div align=center><a href="http://www.codecogs.com/eqnedit.php?latex=E\left&space;(&space;\overline{x}&space;\right&space;)=E\left&space;(&space;\&space;\frac{1}{N}\sum_{i=1}^{N}x_{i}\right&space;)" target="_blank"><img src="http://latex.codecogs.com/gif.latex?E\left&space;(&space;\overline{x}&space;\right&space;)=E\left&space;(&space;\&space;\frac{1}{N}\sum_{i=1}^{N}x_{i}\right&space;)" title="E\left ( \overline{x} \right )=E\left ( \ \frac{1}{N}\sum_{i=1}^{N}x_{i}\right )" /></a><a href="http://www.codecogs.com/eqnedit.php?latex==E\left&space;(&space;\&space;\frac{1}{N}\sum_{i=1}^{N}\sum_{j=1}^{n}s_{ij}\right&space;)=\frac{1}{N}NnE\left&space;(&space;s&space;\right&space;)=n\left&space;[&space;\frac{1}{2}\times&space;1&plus;\frac{1}{2}\times&space;\left&space;(&space;-1&space;\right&space;)&space;\right&space;]=0" target="_blank"><img src="http://latex.codecogs.com/gif.latex?=E\left&space;(&space;\&space;\frac{1}{N}\sum_{i=1}^{N}\sum_{j=1}^{n}s_{ij}\right&space;)=\frac{1}{N}NnE\left&space;(&space;s&space;\right&space;)=n\left&space;[&space;\frac{1}{2}\times&space;1&plus;\frac{1}{2}\times&space;\left&space;(&space;-1&space;\right&space;)&space;\right&space;]=0" title="=E\left ( \ \frac{1}{N}\sum_{i=1}^{N}\sum_{j=1}^{n}s_{ij}\right )=\frac{1}{N}NnE\left ( s \right )=n\left [ \frac{1}{2}\times 1+\frac{1}{2}\times \left ( -1 \right ) \right ]=0" /></a></div>

下面我们具体研究<a href="http://www.codecogs.com/eqnedit.php?latex=\overline{x}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\overline{x}" title="\overline{x}" /></a>的波动幅度与步数<a href="http://www.codecogs.com/eqnedit.php?latex=n" target="_blank"><img src="http://latex.codecogs.com/gif.latex?n" title="n" /></a>的关系，下图是一次模拟中<a href="http://www.codecogs.com/eqnedit.php?latex=\overline{x^{2}}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\overline{x^{2}}" title="\overline{x^{2}}" /></a>随步数的变化

<div align=center><img src="https://github.com/ACGNnsj/-/blob/master/Final%20Project/figure_1-2.png?raw=true" /></div>

可以看出，<a href="http://www.codecogs.com/eqnedit.php?latex=\overline{x^{2}}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\overline{x^{2}}" title="\overline{x^{2}}" /></a>的值大致等于步数，这是因为

<div align=center><a href="http://www.codecogs.com/eqnedit.php?latex=E\left&space;(&space;\overline{x^{2}}&space;\right&space;)=E\left&space;(&space;\&space;\frac{1}{N}\sum_{i=1}^{N}x_{i}^{2}\right&space;)=\frac{1}{N}\sum_{i=1}^{N}E\left&space;(&space;\&space;x_{i}^{2}\right&space;)=E\left&space;(&space;\&space;x_{i}^{2}\right&space;)=E\left&space;[\left&space;(&space;\sum_{j=1}^{n}s_{ij}&space;\right&space;)^{2}&space;\right&space;]" target="_blank"><img src="http://latex.codecogs.com/gif.latex?E\left&space;(&space;\overline{x^{2}}&space;\right&space;)=E\left&space;(&space;\&space;\frac{1}{N}\sum_{i=1}^{N}x_{i}^{2}\right&space;)=\frac{1}{N}\sum_{i=1}^{N}E\left&space;(&space;\&space;x_{i}^{2}\right&space;)=E\left&space;(&space;\&space;x_{i}^{2}\right&space;)=E\left&space;[\left&space;(&space;\sum_{j=1}^{n}s_{ij}&space;\right&space;)^{2}&space;\right&space;]" title="E\left ( \overline{x^{2}} \right )=E\left ( \ \frac{1}{N}\sum_{i=1}^{N}x_{i}^{2}\right )=\frac{1}{N}\sum_{i=1}^{N}E\left ( \ x_{i}^{2}\right )=E\left ( \ x_{i}^{2}\right )=E\left [\left ( \sum_{j=1}^{n}s_{ij} \right )^{2} \right ]" /></a></div>

而<a href="http://www.codecogs.com/eqnedit.php?latex=s_{ij_{1}}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?s_{ij_{1}}" title="s_{ij_{1}}" /></a>与<a href="http://www.codecogs.com/eqnedit.php?latex=s_{ij_{2}}" target="_blank"><img src="http://latex.codecogs.com/gif.latex?s_{ij_{2}}" title="s_{ij_{2}}" /></a>是相互独立的随机变量，故有

<div align=center><a href="http://www.codecogs.com/eqnedit.php?latex=E\left&space;(s_{ij_{1}}s_{ij_{2}}&space;\right&space;)=E\left&space;(&space;s_{ij_{1}}&space;\right&space;)E\left&space;(&space;s_{ij_{2}}&space;\right&space;)=\left&space;[&space;\frac{1}{2}\times&space;1&plus;\frac{1}{2}\times&space;\left&space;(&space;-1&space;\right&space;)&space;\right&space;]^{2}=0" target="_blank"><img src="http://latex.codecogs.com/gif.latex?E\left&space;(s_{ij_{1}}s_{ij_{2}}&space;\right&space;)=E\left&space;(&space;s_{ij_{1}}&space;\right&space;)E\left&space;(&space;s_{ij_{2}}&space;\right&space;)=\left&space;[&space;\frac{1}{2}\times&space;1&plus;\frac{1}{2}\times&space;\left&space;(&space;-1&space;\right&space;)&space;\right&space;]^{2}=0" title="E\left (s_{ij_{1}}s_{ij_{2}} \right )=E\left ( s_{ij_{1}} \right )E\left ( s_{ij_{2}} \right )=\left [ \frac{1}{2}\times 1+\frac{1}{2}\times \left ( -1 \right ) \right ]^{2}=0" /></a></div>

从而有

<div align=center><a href="http://www.codecogs.com/eqnedit.php?latex=E\left&space;[\left&space;(&space;\sum_{j=1}^{n}s_{ij}&space;\right&space;)^{2}&space;\right&space;]=\sum_{j=1}^{n}E\left&space;(&space;s_{ij}^{2}&space;\right&space;)=nE\left&space;(&space;s_{ij}^{2}&space;\right&space;)=n\left&space;[&space;\frac{1}{2}\times&space;1^{2}&plus;&space;\frac{1}{2}\times&space;\left&space;(-1&space;\right&space;)^{2}&space;\right&space;]=n" target="_blank"><img src="http://latex.codecogs.com/gif.latex?E\left&space;[\left&space;(&space;\sum_{j=1}^{n}s_{ij}&space;\right&space;)^{2}&space;\right&space;]=\sum_{j=1}^{n}E\left&space;(&space;s_{ij}^{2}&space;\right&space;)=nE\left&space;(&space;s_{ij}^{2}&space;\right&space;)=n\left&space;[&space;\frac{1}{2}\times&space;1^{2}&plus;&space;\frac{1}{2}\times&space;\left&space;(-1&space;\right&space;)^{2}&space;\right&space;]=n" title="E\left [\left ( \sum_{j=1}^{n}s_{ij} \right )^{2} \right ]=\sum_{j=1}^{n}E\left ( s_{ij}^{2} \right )=nE\left ( s_{ij}^{2} \right )=n\left [ \frac{1}{2}\times 1^{2}+ \frac{1}{2}\times \left (-1 \right )^{2} \right ]=n" /></a></div>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;接下来，我们取消步长为固定值的限制，使每步的位移在<a href="http://www.codecogs.com/eqnedit.php?latex=\left&space;[&space;-1,1&space;\right&space;]" target="_blank"><img src="http://latex.codecogs.com/gif.latex?\left&space;[&space;-1,1&space;\right&space;]" title="\left [ -1,1 \right ]" /></a>间等概率随机取值。

#### →[查看程序](https://github.com/ACGNnsj/-/blob/master/Final%20Project/Final%20Project1-2.py)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;我们同样取行人人数为10000，模拟三次得如下结果

<div align=center><img src="https://github.com/ACGNnsj/-/blob/master/Final%20Project/figure_2-1.png?raw=true" /></div>



###4. 结果讨论

---

<h4 align="center">参考文献</h4>
