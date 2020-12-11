
  

### 带你学AI·深度学习与TensorFlow2实战开发之深度学习初探

深度学习初探

> 写这部分主要为了解决如何入门深度学习方法论的问题，小宋总结了一些大家容易疑惑的问题，包括： 1、深度学习是什么与传统算法区别，我是否需要深度学习技术。 2、该如何开始学习与选择资料 3、在学习的过程中遇到问题如何解决与寻求帮助 最后小宋一直以来学习AI开发的心得感悟分享及建议，阅读完就可以得到自己的答案

### 

是否需要深度学习

![](https://pic3.zhimg.com/v2-14d969cbd5c8661230ef2d11e9e2ff46_b.png)

可能有些朋友对深度学习感兴趣是因为这个技术最近比较流行，讨论的人多，所以才想上手这方面。小宋觉得有这样从众心理是没有问题的，但是还有一句话很重要，适合自己的才更好。先搞清楚这个问题：

我是否需要深度学习技术，我打算用深度学习技术做什么？

要想弄明白这个问题，首先我们要知道何为深度学习：

> 深度学习（英语：deep learning）是机器学习的分支，是一种以人工神经网络为架构，对资料进行表征学习的算法。 深度学习是机器学习中一种基于对数据进行表征学习的算法。观测值（例如一幅图像）可以使用多种方式来表示，如每个像素强度值的向量，或者更抽象地表示成一系列边、特定形状的区域等。而使用某些特定的表示方法更容易从实例中学习任务（例如，人脸识别或面部表情识别）。深度学习的好处是用非监督式或半监督式的特征学习和分层特征提取高效算法来替代手工获取特征。

上面是维基百科对[深度学习概念](https://bk.tw.lvfukeji.com/wiki/%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0)的介绍，更加通俗的解释为将神经网络应用到机器学习领域中替换掉繁杂的传统机器学习手工设计特征，通过神经网络的表征来自动或者半自动提取特征从而实现某一功能。

> 小白说：你这通俗的解释，怎么一点也不通俗呀？什么是特征，什么又是表征，实现某一功能又是什么意思呀？ 小宋答：那我再用一个直观的例子来说明一下：现在我们有一个需求在猫舍前面为了防止狗狗进去捣乱（当然我们也可以在狗舍前做相反功能不让猫咪进去），我们需要设计一个功能，放在猫舍门前能够分类出要进入猫咪还是狗狗（实现某一功能），然后在判断是否开门。

![](https://pic1.zhimg.com/v2-915cb9b4391171891ea4108e453bb8fc_b.png)

> 如果让一个传统机器学习算法工程师来设计算法，他会先观察猫狗的特点，然后找一下能够区分它们的特点作为特征，比如个头大小，花纹，耳朵形状等等（手工设计特征）。 如果这个算法给深度学习算法工程师，他会设计一个容器（神经网络），使用这个容器不断去过（训练）分类好带有标签的照片（训练集），这个容器在学习的过程中，不断自我优化将照片表示为一组数据（神经网络的表征）。 现在我们对比一下差异：传统机器学习需要算法工程师先研究数据，总结一些规律，设计规则。而深度学习工程师更多的是对容器（神经网络）的设计，使用这个容器（神经网络）来自动组合特征（表征）。所以说深度学习是个自动或者半自动提取特征。 其实上面例子在实际生活中有类似应用，百度相关开发人员就曾开发类似功能实现对于流浪猫的管理。后面《带你学AI》系列教程将在《手把手分类项目实战讲解》部分详细介绍如何实现。

上面部分是对于深度学习一个简单介绍，下面对于常见的几个概念进行补充。如果用一句话来概述这个图：

机器学习是实现人工智能的途径，深度学习是机器学习中一个强有力的工具。

![](https://pic4.zhimg.com/v2-8c41437008b7f223e6c25ffb15deecef_b.png)

其实深度学习并非新出现的技术，早在上世纪就被提出，经过数次起伏，最终才在2012年的ImageNet大规模视觉识别挑战赛（ILSVRC）通过AlexNet大放异彩（实现超越传统方法9个百分点的效果）。也从而推进了以卷积神经网络代表的深度学习在目标检测追踪，像素分割等任务发展与大规模应用。

> 小宋说：深度学习技术之所以受大家欢迎，原因无外乎使用简便，效果好。而这离不开三个方面，数据，算法与算力，这一点在AlexNet大放异彩体现的淋漓尽致。ImageNet大规模视觉识别数据集（数据），GPU大规模应用（算力），对LeNet的改造优化而来的AlexNet(算法)。所以如果当我们选择使用深度学习需要考虑此场景是否能满足这个条件，从而发挥出深度学习的功效。

通过上面内容，大家可以对于人工智能，机器学习，深度学习及神经网络有个初略的认识与理解。现在到了关键问题，自己是否真的需要深度学习技术？

大家可以通过以下几个简单问题测试一下：

1，是否对深度学习感兴趣打算从事相关工作？

2，所研究的领域是否可以获取相关数据？

3，工作的环境或者将要工作环境是否有相应硬件算力支持？

4，是否目前传统机器算法成为目前的局限，需要突破？

如果四个都是Yes，那么很建议你从事这方面，并坚信你将会在AI方面贡献自己的一份力。

如果满足三个条件，还是比较建议从事这方向，因为有些问题在做的过程中，不断改善。

如果仅满足一两个条件，就要好好考虑一下，是否要从事这方面工作，因为可能你遇到的阻力会有些大。

> 小白说：我通过了上述测试，但是基础一般，有些盲目，该怎么办呢？ 小宋答：其实也不难，学这个也是有规律可循的，可以持续关注一下这个系列文章，小宋将手把手来带大家上手学习。贵在坚持，小宋会持续做下去，也希望大家坚持学下去。

通过深度学习可以做很多有趣的项目，可以应用在工业上，提升检测效率；也可以应用在农业上，提升资源利用率；也可以应用在制药医疗等等。如果你也有趣的想法和创意，苦于不知道如何动手实践，那就继续往下看，下面有小宋为基础薄弱同学设计的学习方法。

### 

如何开始学习与选择资料

对深度学习有初步了解以后，就该考虑如何开始上手和资料选取。

虽然相较于几年前学习资料匮乏，目前的情况已经好了很多，资料丰富多样。这虽然降低了用户查阅资料的成本，却也增加了基础薄弱同学的选择成本。

虽说是深度学习开发，但其实覆盖的内容还是很多的，包括开发环境，编程语言，常用工具包，深度学习框架等等。小白用户还是很难掌握好步骤，如何一步步由浅入深，避免徘徊。

> 小宋说：其实小宋也不是“科班出身”的计算机相关专业学生，基础也很薄弱在刚开始转AI方面的时候也很迷茫，走了不少弯路。所以下面是小宋总结的由浅入深的学习资料，帮助大家更好更快的无痛入门。

其实学任何东西都是有途径与方法的，只要我们能理清内部关联就可以少走弯路。下面我们来一起梳理下：

1.操作系统的选取与内容学习

首先我们的算法开发要在一个系统平台上，这里就涉及到了一些与系统相关的内容。其实这对于小白用户就是一个比较麻烦的点。大部分同学都是使用Windows系统或者macOS，而好多教程都是基于Linux系统（Ubuntu）开发讲解，也都是推荐用户使用Linux开发。这其实蛮不友好的，无形中增加了学习的门槛。

> 小宋说：但其实这是很次要的一点，小宋这样认为的原因有二：一是系统只是运行的平台不是AI算法的核心；二是目前开发软件与深度学习框架对于不同平台支持差异已经很小了，区别仅仅是在多GPU调用在Windows平台支持不完备，很多新算法会首先适配Ubuntu。这些点小白用户几乎察觉不到。而macOS平台目前对GPU支持不太友好，如果需要大规模训练不太建议使用，如果只是简单试验其实和Windows差不多的。

总结一下系统部分，Windows与Ubuntu都可以用来学习与开发深度学习，如果不嫌麻烦，就装Ubuntu，支持会更好。后面《带你学AI》系列教程环境配置方面会同时包括Windows10与Ubuntu18，同学们选择自己习惯的就好。

系统方面真正要学习的技术点有Linux操作，需要掌握一些对于shell文件和目录的管理和操作。

这里推荐菜鸟教程中《Linux 教程》：[https://www.runoob.com/linux/linux-tutorial.html](https://www.runoob.com/linux/linux-tutorial.html)

建议把Linux全部看完掌握，Shell复杂的一些指令可以用到再学。

![](https://pic4.zhimg.com/v2-bf0a80c71f43c3ad8d6914c2e171484f_b.png)

> 小宋说：其实还有一些会遇到的工具，但是并非必须的，这里就不重点推荐了。比如[Shell指令](https://www.runoob.com/linux/linux-shell.html)与[Git操作](https://www.runoob.com/git/git-tutorial.html)这里仅作为补充说明，供学有余力的同学翻阅了。

2.编程语言与开发软件

编程语言其实没什么好选择的，Python可能不是最好的语言，但的确是最适合做AI开发的语言。首先目前大部分深度学习框架对于Python接口都是最丰富完善的，而且Python语言上手简单很适合小白用户。这里就直接推荐几个比较好的教程：

1.菜鸟教程的Python3教程：[https://www.runoob.com/python3/python3-tutorial.html](https://www.runoob.com/python3/python3-tutorial.html)。这个教程比较基础，适合初学者入门使用

2.廖雪峰老师的Python3教程：[https://www.liaoxuefeng.com/wiki/1016959663602400](https://www.liaoxuefeng.com/wiki/1016959663602400)。这个教程有些高阶操作，适合想要提升的同学

Python开发软件比较常用的有PyCharm与VSCode。对于PyCharm有专业版和社区版之分，专业版收费功能更加丰富；社区版是开源免费的，功能有阉割，但是用来做深度学习开发还是够用的。

> 小宋说：其实小宋最开始学Python用的就是PyCharm，给我的感触是功能丰富整体也很烦躁臃肿，当时新打开一个项目都会加载很久，后来VSCode出现了，更加轻量化也很易用，对普通用户更加友好。所以如果小伙伴们如果不是常用PyCharm，建议使用VSCode来开发。

![](https://pic4.zhimg.com/v2-8c91890ae94a53a98388da67498b0de3_b.png)

后面《带你学AI》系列教程环境配置方面会以VSCode为例，由于VSCode多平台支持的，所以会针对Ubuntu与Windows都会有使用教程说明。

3.学习框架与资料

[《带你学AI》](https://github.com/xiaosongshine/Learn2Ai4TensorFlow2)系列教程将基于TensorFlow2.3，选择TensorFlow2的原因是TensorFlow2相较于TensorFlow1.x更新为动态图，更加易用好学，同时部署性也极佳。会更加适用于大多数用户。

![](https://pic3.zhimg.com/v2-af2e7f2b31cfa5e029e7b9aa7973ef0e_b.png)

同时TensorFlow2的资料也较为丰富，易用学习与提升。下面有些总结的TensorFlow2，供小伙伴们参考：

1.官方资料：

> 中文官网： [https://tensorflow.google.cn](https://tensorflow.google.cn/) 教程： [https://tensorflow.google.cn/tutorials](https://tensorflow.google.cn/tutorials) 指南： [https://tensorflow.google.cn/guide](https://tensorflow.google.cn/guide)

2.TensorFlow2相关资料：

> Dev Summit 开发者峰会总结：[https://mp.weixin.qq.com/s/YcvIp1cpGsAfsZm2rerxmg](https://mp.weixin.qq.com/s/YcvIp1cpGsAfsZm2rerxmg) TensorFlow 2.3 新功能概览：[https://mp.weixin.qq.com/s/C_CQJrHRLrLSKk_IRUR2Pw](https://mp.weixin.qq.com/s/C_CQJrHRLrLSKk_IRUR2Pw) TensorFlow2.0 正式版官方介绍视频：[https://v.qq.com/x/page/b3003v2g8dq.html](https://v.qq.com/x/page/b3003v2g8dq.html) TensorFlow发展史：[『王霸之路』从0.1到2.0一文看尽TensorFlow奋斗史](https://xiaosongshine.blog.csdn.net/article/details/102014069)

3.上手实战资料和数据推荐

1）Keras之父作品《Python 深度学习》

> 《Python 深度学习》是由 Keras 之父、现任 Google 人工智能研究员 Francois Chollet 的作品 本书详尽介绍了用 Python 和 Keras 进行深度学习的探索实践，包括计算机视觉、自然语言处理、产生式模型等应用。

![](https://pic2.zhimg.com/v2-14401049785bdcda69d31ac528d4a58d_b.png)

书中包含30多个代码示例，步骤讲解详细透彻。由于本书立足于人工智能的可达性和大众化，读者无须具备机器学习相关背景知识即可展开阅读。

> 学习完本书后，读者将具备搭建自己的深度学习环境、建立图像识别模型、生成图像和文字等能力。

2）Xihan Li老师的《简单粗暴 TensorFlow 2》

> 此学习手册适用于以下读者： 已有一定机器学习或深度学习基础，希望将所学理论知识使用 TensorFlow 进行具体实现的学生和研究者； 曾使用或正在使用 TensorFlow 1.X 版本或其他深度学习框架（比如 PyTorch），希望了解和学习 TensorFlow 2 新特性的开发者； 希望将已有的 TensorFlow 模型应用于业界的开发者或工程师。 同时配套纸质完整版书籍，纸质版《简明的 TensorFlow 2》由人民邮电出版社（图灵社区）出版，在本在线手册的基础上进行了细致的编排校对，并增加了若干 TensorFlow 高级专题，全彩印刷，为读者带来更好的阅读体验。

![](https://pic2.zhimg.com/v2-bf9301aa8fa6c7d7b39802c752a903f9_b.png)

> 小宋说：这些推荐教材可不是广告哦，当然书籍作者大佬想给小宋打钱我也不介意哈哈~~，其实能给我邮寄个签名就很满足啦。真的是很优秀值得推荐的教材。也会是[《带你学AI》](https://github.com/xiaosongshine/Learn2Ai4TensorFlow2)系列教程主要参考资料。

最后做一下总结：

1.首先我们的算法开发要在一个系统平台上，这里就涉及到了一些与系统相关的内容。选取Windows与Ubuntu都可以，Windows与Ubuntu都可以用来学习与开发深度学习，如果不嫌麻烦，就装Ubuntu，支持会更好。

可以学习翻阅的资料有：菜鸟教程中《Linux 教程》[https://www.runoob.com/linux/linux-tutorial.html](https://www.runoob.com/linux/linux-tutorial.html)

2.学习AI开发编程无法避免的，目前大部分深度学习框架对于Python接口都是最丰富完善的，而且Python语言上手简单很适合小白用户。

必备技能点Python及学习资料推荐：菜鸟教程的《Python3教程》 [https://www.runoob.com/python3/python3-tutorial.html](https://www.runoob.com/python3/python3-tutorial.html)

编程也需要相关软件：VSCode使用

3.学习框架选择TensorFlow2，原因是TensorFlow2相较于TensorFlow1.x更新为动态图，更加易用好学，同时部署性也极佳。会更加适用于大多数用户。

主要推荐这两本书籍：

1）Keras之父作品《Python 深度学习》

2）Xihan Li老师的《[简单粗暴 TensorFlow 2](https://tf.wiki/zh_hans/)》

> 小宋说：其实上面内容略显啰嗦（官方吐槽：），其实是想通过详细的描述复现一下当想学习上手一门新技术时应该如何去选择思考。希望小伙伴们看完这个能培养出一些自己思考习惯，再学习其他新技术或者技能的时候也能找到途径与方法理清内部关联就可以少走弯路。 如果小伙伴有什么感想或者有其他好的思考方法也欢迎在评论区说出，小宋在这里替大家先谢谢啦。

### 

在学习的过程中遇到问题如何解决与寻求帮助

> 小宋说：上面一些内容主要对一些环境工具以及框架相关的介绍，下面就是针对于大家可能遇到的问题做些总结与经验分享。包括遇到问题后该如何定位问题，该如何准确详细描述问题，该在哪里搜索答案与寻求帮助。

其实在网上去找一些资料开始学习，这些并不麻烦。但遇到一些没见过的问题，确实是会让人十分头痛的。一个不起眼小问题往往会被困扰许久。其实我觉得专家与普通用户的很重要的差异就是遇到和解决问题的多少，还有就是解决问题的途径解决后的总结思考。这部分内容主要讲解的就是解决问题的思路和方法方面的经验，让小伙伴们能更好的利用出现的问题提升自己。Keep Fighting。。。

![](https://pic2.zhimg.com/v2-a7aad47224efaaf634917b17d0ed7b55_b.png)

首先是心态方面，遇到问题不用觉得害怕。因为只有在解决问题过程中我们才能不断提升自己。想起了最近在看的一本书《反脆弱》，从不确定中受益。书中讲到，人们都普遍害怕不确定情况和遇到问题，但如果可以却避免这些会导致自身变得脆弱。

![](https://pic2.zhimg.com/v2-d066603861dd572e06bbba097451a605_b.png)

就像温室里的花朵，承受不住严寒和酷暑，而真实的世界更多的是后者。不要怕遇到问题，保持一个学习成长的心态，就会从解决问题中收获很多。

下面就一些具体问题来分享一下解决方法与思路方面的经验：

![](https://pic1.zhimg.com/v2-fb8413a72696f07f72c66f918f547fc8_b.png)

以初学者大多会遇到的安装TensorFlow GPU学习框架出现问题举例，因为GPU依赖较多，这一步是很容易出问题的。首先我们先分解一下这个问题，安装TensorFlow GPU版需要哪些支持，可以看看官网上安装[TensorFlow GPU的教程](https://tensorflow.google.cn/install/gpu)：

> 硬件要求 支持以下带有 GPU 的设备： CUDA® 架构为 3.5、3.7、5.2、6.0、6.1、7.0 或更高的 NVIDIA® GPU 卡。请参阅[支持 CUDA® 的 GPU 卡](https://developer.nvidia.com/cuda-gpus)列表。 在配备 NVIDIA® Ampere GPU（CUDA 架构 8.0）或更高版本的系统上，内核已从 PTX 经过了 JIT 编译，因此 TensorFlow 的启动时间可能需要 30 多分钟。通过使用“export CUDA_CACHE_MAXSIZE=2147483648”增加默认 JIT 缓存大小，即可将此系统开销限制为仅在首次启动时发生（有关详细信息，请参阅 [JIT 缓存](https://devblogs.nvidia.com/cuda-pro-tip-understand-fat-binaries-jit-caching)）。 对于 CUDA® 架构不受支持的 GPU，或为了避免从 PTX 进行 JIT 编译，亦或是为了使用不同版本的 NVIDIA® 库，请参阅[在 Linux 下从源代码编译](https://tensorflow.google.cn/install/source)指南。 软件要求 必须在系统中安装以下 NVIDIA® 软件： [NVIDIA® GPU 驱动程序](https://www.nvidia.com/drivers)：CUDA® 10.1 需要 418.x 或更高版本。 [CUDA® 工具包](https://developer.nvidia.com/cuda-toolkit-archive)：TensorFlow 支持 CUDA® 10.1（TensorFlow 2.1.0 及更高版本） CUDA® 工具包附带的 [CUPTI](http://docs.nvidia.com/cuda/cupti/)。 [cuDNN SDK 7.6](https://developer.nvidia.com/cudnn) （可选）[TensorRT 6.0](https://docs.nvidia.com/deeplearning/sdk/tensorrt-install-guide/index.html)，可缩短用某些模型进行推断的延迟时间并提高吞吐量。

总结一下就是需要这些支持：

1.硬件要支持，需要有较新版本英伟达GPU

2.Cuda环境需要配置

3.Python开发环境配置

4.正确安装TensorFlow GPU操作

> 小宋说：这些需要一步步检查，必须确保没有问题才能保证安装的成功。经常有朋友给我私信说安装TensorFlow GPU，却无法定位到问题所在。其实这个只需要梳理一下依赖关联，有些问题就比较容易解决。直接去问别人却无法说明问题所在，有时真的是想帮也帮不了的。

小宋的建议：先自己简单检查一下可能出问题的支持和依赖，一步步由底层向上层测试，定位到问题所在：硬件是否支持，GPU驱动与Cuda是否安装好，Python版本是否正确，安装TensorFlow GPU操作步骤是否正确。

解决问题的第一步是定位问题，定位到具体问题虽在才方便解决，无论是在查找资料还是请教别人时这些都很关键。

在定位到问题后，就是要查找答案和寻求帮助了，下面列举一些寻找问题答案的网站：

-   谷歌
    
-   百度 [https://www.baidu.com/](https://www.baidu.com/)
    
-   CSDN [https://www.csdn.net/](https://www.csdn.net/)
    
-   知乎 [https://www.zhihu.com/](https://www.zhihu.com/)
    
-   GIthub [https://www.github.com/](https://www.github.com/)
    
-   Stack Overflow [如何优雅地使用 Stack Overflow？](https://www.zhihu.com/question/20824615)
    

这里多介绍一下GIthub的使用，这可不仅仅是代码开源平台，善用上面的Issues内容可以大大提升解决问题效率。Issues是开源的问题与回复汇总，开发人员常遇到的问题都在上面的，而且可以在上面提问，是个很好的工具。

![](https://pic3.zhimg.com/v2-19aca510b98b12fc67504a1678595b1e_b.png)

这里以TensorFlow 开源举例 [https://github.com/tensorflow/tensorflow/issues](https://github.com/tensorflow/tensorflow/issues)

可以在搜索框中搜索问题，推荐使用英语关键字搜索。可以搜不到可以把搜索框里的"is:issue is:open"删去代表搜索所有，如果不删搜索条件就是open的issue代表尚未解决的问题。如果没有找到相关问题，可以点击"New issue"按钮新建issue，选择一个issue类型，就可以描述自己问题了，最后提交即可，就可以等着相关人员回复：

![](https://pic2.zhimg.com/v2-0f743d571a62fe3369f0dcc9afb056c9_b.png)

其实在提交问题方面，也是有一些技巧的，大部分朋友在问小宋的时候，往往仅仅是错误信息的截图，其实错误信息的截图是很重要的信息，但是这些错误信息是和硬件系统软件版本与你的具体操作相关的。错误信息的截图配合硬件系统软件版本与你的具体操作才是良好的提问题习惯，更有助于解决问题的。

  

----------

  

### 

尾巴

这是[《带你学AI》](https://github.com/xiaosongshine/Learn2Ai4TensorFlow2)系列教程第一篇内容，主要是对于开篇的介绍以及对入门深度学习的一些经验分享，写的会比较细致，是偏理论性与经验性内容。可能会让一些大佬觉得太琐碎简单，其实文章主要面向初学者，详细复盘了小宋思考的过程。授人以鱼不如授人以渔，希望小伙伴们能通过这篇文章，培养起来一些针对问题的思考习惯。大家针对这个文章或者入门深度学习有什么想法可以在评论区欢迎发表自己看法。

下篇内容将开始实战操作，手把手环境搭建与开发环境配置（包括Ubuntu18以及Windows10），还是一样的细致入微，简单易懂。不见不散。
