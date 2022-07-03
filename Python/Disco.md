# AI 艺术家

What can AI do? 今天就来介绍一个AI画图的程序“**Disco Diffusion**".

### 用法&原理

简单来说，只要你输入一句英文，Disco 就会根据你的描述来生成一张图片。

**原理**：Disco 根据描述寻找大量的相关图片通过GAN等DL算法渲染出图片。

### 部署问题

Disco 目前有Google Colab的版本，即完全部署在云端，不受本地显卡质量限制，也不需要繁琐的cuda配置。~~（但需要跨过那个不存在的墙）~~

为了运行程序，还需要Google账号，但自从Google大部分退出中国后也ban了中国用户注册Google账号，需要某些玄学方法or万能tb。

Google colab 提供了免费的显卡，大部分时间我分配到的都是Tesla V100 or K80（最近在跑的MNIST也是部署在colab上的）

### 一起来欣赏一些AI画出来的图片吧~

![TimeToDisco(0)_0](C:\Users\阿漆\Desktop\disco\TimeToDisco(0)_0.png)

（a beautiful painting of Chinese Shanshui landscape, clouds, ink style, trending on artstation）

![TimeToDisco(3)_0](C:\Users\阿漆\Desktop\disco\TimeToDisco(3)_0.png)

A beautiful painting of a **starry night**, shining its light across a **sunflower sea** by **James Gurney**, Trending on artstation

![TimeToDisco(3)_2](C:\Users\阿漆\Desktop\disco\TimeToDisco(3)_2.png)

同上

![TimeToDisco(2)_1](C:\Users\阿漆\Desktop\disco\TimeToDisco(2)_1.png)

![TimeToDisco(2)_3](C:\Users\阿漆\Desktop\disco\TimeToDisco(2)_3.png)

A beautiful painting of a singular lighthouse

### 更上一层楼

AI画图的一个特点就是会产生一些人类想不到的地方（就像当年Alphago对阵李世石的那摸不着头脑的一手棋），一些画师开始尝试在AI画出来的图上进行修改，来产出新的作品。在我看来，AI要做的，不是代替，而是协助。

**PS**：如果你有好的idea，欢迎联系我跑一跑，说不定就是下一张壁纸了呢。

