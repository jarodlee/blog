# 扫雷的入门教学

扫雷是大多数电脑中自带安装的一个小游戏，在windows电脑中可通过“开始”菜单-&gt;“游戏”找到它。

它是一种对记忆和推理能力进行练习的简单测试，在游戏中练习并熟练鼠标的操作，重点区分鼠标左键与右键的使用方法。

## 游戏目标：

找出空方块并避免触雷。

![&#x9AD8;&#x7EA7;&#x626B;&#x96F7;&#x6210;&#x529F;&#x753B;&#x9762;](../.gitbook/assets/411525803-hd-32.png)

看起来很容易，不是吗？

## 规则和基本要求

### 游戏目标

找出空方块，同时避免触雷。清除扫雷区的速度越快，得分就越高。

### 玩法

扫雷的规则非常简单：

挖开地雷，游戏即告结束（失败）。

挖开空方块，可以继续玩。

挖开数字，则表示在其周围的八个方块中共有多少个雷，可以使用该信息推断能够安全单击附近的哪些方块。

### 扫雷等级

扫雷有三个标准扫雷区可供选择，各扫雷区的扫雷难度依次递增。

初级： 81 个方块、10 个雷

中级： 256 个方块、40 个雷

高级： 480 个方块、99 个雷

还可以创建自定义扫雷区。扫雷游戏支持最多有 720 个方块和 668 个雷的扫雷区。

### 提示与技巧

标记地雷。 如果您认为某个方块可能藏有地雷，请右键单击它。这会在该方块上做一个旗标。

研究图案。 如果一行中有三个方块显示为 2-3-2，您就会知道该行旁边可能排列着三个雷。如果一个方块显示为 8，则它周围的每个方块下面都有一个雷。

浏览未探测的。 如果不确定下一个单击位置，可以尝试清除某些未探测的区域。在未标记方块的中间单击比在可能有雷的区域单击要好一些。

## 全球的扫雷比赛网站

在全世界各个国家都有很多人热爱扫雷，我们可以通过《扫雷世界》这个网站与所有人竞赛：[https://minesweeper.online/zh/](https://minesweeper.online/zh/)

### 成就系统：[https://minesweeper.online/zh/achievements](https://minesweeper.online/zh/achievements)

![&#x626B;&#x96F7;&#x4E16;&#x754C;&#x7684;&#x6210;&#x5C31;&#x7CFB;&#x7EDF;](../.gitbook/assets/achievement.png)

### 网站中的一些参数定义：

ZiNi 點擊最小値

H.ZiNi Human ZiNi ZiNi仿人類算灋

IoE Index of Efficiency 效率指數 3BV / Cl

ThrP 破空率 IoE / Corr

Corr Correctness 準確率 ECl / Cl

ZNE ZiNi Efficiency 點擊效率 ZiNi / Cl

ZNT 有效點擊效率 ZiNi / ECl

RQP Rapport Qualité Prix​​ \(RTime+1\) / 3BV/s

IoS Index of Speed 速率指數 log \(3BV\) / log \(Time - 1\)

感谢[一位玩家](https://minesweeper.online/zh/player/2731349)在聊天室中提供的回复

## 网络资料

参考1：[http://www.minesweeper.info/wiki/Strategy](http://www.minesweeper.info/wiki/Strategy)

