# Project 1----Hog
- [x] ## 问题0

  熟悉骰子怎么实现的

- [x] ## 问题1

  实现了掷骰子的分数统计和`pig out`的特例

  ```python
  	# BEGIN PROBLEM 1
      "*** YOUR CODE HERE ***"
      lst = []
      for i in range(num_rolls):
          lst.append(dice())
      flag = True
      for i in lst:
          if i == 1:
              flag = False
              break
      if flag:
          return sum(lst)
      else:
          return 1
      # END PROBLEM 1
  ```

  

  <img src="C:\Users\阿漆\AppData\Roaming\Typora\typora-user-images\image-20220620162047458.png" alt="image-20220620162047458" style="zoom:33%;" />

- [x] ## 问题2

  实现free bacon。（一个游戏规则）。

  感觉这是出牌者主动选择的一个技能，就是这轮不掷骰子，然后根据对手的分数直接计算得到本轮分数。
  
  下面是具体的规则：
  
  ![image-20220620163156376](C:\Users\阿漆\AppData\Roaming\Typora\typora-user-images\image-20220620163156376.png)

<img src="C:\Users\阿漆\AppData\Roaming\Typora\typora-user-images\image-20220620163208074.png" alt="image-20220620163208074" style="zoom:50%;" />

​		比如说最后一个例子，pi小数点后第42位是9，故此轮可以得到12分。

```python
	# Trim pi to only (score + 1) digit(s)
    # BEGIN PROBLEM 2
    # 官方给的Hint是修剪(Trim)Pi到(score+1)位,然后把最后一位加3返回
    "*** YOUR CODE HERE ***"
    pi = pi//(10**(100-score))
    # END PROBLEM 2

    return pi % 10 + 3
```

<center>过啦！</center>

<img src="C:\Users\阿漆\AppData\Roaming\Typora\typora-user-images\image-20220620165842024.png" alt="image-20220620165842024" style="zoom:45%;" />

- [x] ## 问题3

​	<img src="C:\Users\阿漆\AppData\Roaming\Typora\typora-user-images\image-20220621150939355.png" alt="image-20220621150939355" style="zoom:33%;" />

- [x] ## 问题4A

  如果自己和对手分数的最大公约数 >=10，则可以额外获得一轮

  不过有点忘记gcd怎么写了，可恶！

  <img src="C:\Users\阿漆\AppData\Roaming\Typora\typora-user-images\image-20220621194625399.png" alt="image-20220621194625399" style="zoom: 33%;" />

- [x] ## 问题4B

- [ ] <img src="C:\Users\阿漆\AppData\Roaming\Typora\typora-user-images\image-20220621195701468.png" alt="image-20220621195701468" style="zoom:33%;" />

- [ ] 

- [x] ## 问题5

感觉是目前为之最难的一个了。

思路一开始就有点小问题，然后细节上也有很多坑。

<img src="C:\Users\阿漆\AppData\Roaming\Typora\typora-user-images\image-20220621222414604.png" alt="image-20220621222414604" style="zoom:33%;" />