This is a Matrix Calculator program in Java


本程序能够自定义矩阵，并且能对矩阵进行基本的四则运算以及复杂的混合运算，可以为你省去无聊、繁琐的计算过程，非常适合正在学习线性代数的同学
（想老子大一那年就非常讨厌计算矩阵，这也是我想写这个程序的原因）。本程序参考matlab实现，一些交互逻辑是和matlab是一样的，比如命令行模式，
个人认为在这里这种输入模式的效率是最高同时也是最简单的，定义矩阵的方式完全参考matlab。本程序同样能够识别一些其他基本命令，能够对输入错误进行一些提示。



整个界面分成了三部份，左边的输入和输出区，也就是所谓的command区，右上角记录你当前定义的矩阵，右下角记录你运算的历史记录，你在左边输入定义矩阵的命令，若这个矩阵没有被定义过，则会在右上角加入这个矩阵，若之前被定义过，则会更新它的值。你在左边输入表达式，运算结果会紧接着在左边显示，同时会添加到右下角的历史记录区。菜单栏设置里的重置是在左边区域出问题时能帮你回到最开始的状态用的。自动换行是设置左边的command区域用的，当命令过长时，勾选这个看起来比较美观。



有几个注意点:


-- 目前，最多只支持定义10个矩阵，再多了就会出问题，当然你也可以修改程序来达到更多的目的，不过我认为10个就够用了。


-- 目前把矩阵内的数据统一当作double型数据处理，并且运算结果统一保留两位，为的是打印出来比较整齐。


--目前支持的命令有：


  cls(清屏)
  
  help(帮助) 
  
  about(关于) 
  
  del all(删除所有已经定义过的矩阵) 
  
  inv(name)(求某个矩阵的逆矩阵)
  
  定义矩阵  
  
  计算表达式   
  
  (注意前面的命令都不区分大小写)


-- 这里给一下输入矩阵的格式


  A = [2 2;2 2]


  A = [2,2;2,2]


  A = [2 2;2,2]



和matlab输入一样的格式，任意位置都允许任意多个空格


--矩阵的名字必须以字母开头，任意多个数字或者字母结束
