# Minecraft-Survival-Datapack  
为我的世界生电玩家制作的合成表数据包  
最新支持到1.19.4，可以加载实验性内容（所以也许也支持1.20）  
  
---
### 食用方法：
单人存档：  
把下载好的压缩包丢到对应世界中的datapacks文件夹中  
以新的世界为例，应该丢到\.minecraft\saves\新的世界\datapacks里面  
重进存档或者在游戏内输入指令：  
/datapack enable "file/CraftingDatapack-vx.x.zip"  
  
服务器：  
把下载好的压缩包丢到服务器根目录\world\datapacks中  
在控制台或者管理员在服务器中输入指令：  
/datapack enable "file/CraftingDatapack-v2.0.zip"  
  
  ---
## 简介
本数据包针对[SunnySlopes](https://space.bilibili.com/100377977)的数据包进行了一些逻辑的优化并添加了部分新配方。  
支持1.19.4,1.20-pre，<del>支持低版本（未测试）</del>  
由于SunnySlopes对原专栏没有再进行维护（也许？），本篇将对本数据包的内容再做一次详细介绍。
> 本数据包为游戏添加了大量合成配方，少量烧炼配方和切石配方，使得几乎所有物品都变得可再生（钻石和下界残骸可再生因为具有一定争议性将不再考虑添加到数据包中，但是矿石合成原矿不受影响），但同时因为我也是一名生电玩家，所以在数据包中我会尽量兼顾其原料的获得性使之与获得物尽量对等，以尽量减少对游戏难度的影响，所以可能会出现一些物品（如鞘翅）造价仍然很高的情况。此外，数据包也考虑到了部分建筑玩家的需求，方便所有玩家生存使用。</br>可再生的标准（防杠）：如果有主流的专门获得这种物品的农场（包括利用bug例如刷沙机），或者其他一些常见且不具有随机性的再生方式（例如流浪商人或者后期的末影龙就因为具有随机性而不算），则视为可再生。所以粘土和珊瑚块的合成仍然保留。[^引用]  

---
### 便利（conveniences）：  

![wooden_slab](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/01.png)  
切石机能切石头，那切点木头不过分吧</br>  
![wooden_stairs](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/02.png)  
同上</br>  
![bone_block](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/03.png)  
添加了骨块的无序合成</br>  
![bread](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/04.png)  
添加了面包的无序合成</br>  
![paper](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/05.png)  
添加了纸的无序合成</br>  
![shulker_box](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/06.png)  
添加了潜影盒的无序合成</br>  
![dispenser](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/07.png)  
妈妈再也不怕我手残合成一背包投掷器啦</br>  
![dispenser](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/08.png)  
再也不用慢吞吞的一把一把放弓了</br>  
![soul_soil](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/09.png)  
灵魂沙可以变成灵魂土（但是变不回来哦）</br>  

---
### 原版优化（minecrfat）：  
深板岩圆石和黑石成为圆石的替代品！  
这类配方包括：**投掷器、发射器、侦测器、活塞和拉杆**
  
![alternative](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/10.gif)  
再也不用担心废石没地方用啦</br>  

---
### 再生（renewables）：  
![ancient_debris](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/11.png)  
添加远古残骸的配方（因为有些机器会用远古残骸做爆炸室）</br>  
![coral_block](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/12.gif)  
添加珊瑚块的配方（可由珊瑚扇或珊瑚混合合成）</br>  
![bundle](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/13.png)  
添加收纳袋的配方（1.19.4需添加1.20更新数据包，不会影响其他版本）</br>  
![clay](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/14.png)  
黏土的可再生配方（无序合成）</br>  
![cobweb](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/15.png)  
蜘蛛网</br>  
![horse_armor](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/16.png)  
铁或黄金马凯同理（原版就有皮革马铠的配方故不再添加）</br>  
![dragon_head](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/17.png)  
龙首</br>  
![elytra](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/18.png)  
鞘翅  
**注意：鞘翅的附魔会被消除**[^数据包合成表]</br>  
![gilded_blackstone](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/19.png)  
镶金黑石（建筑党福音）</br>  
![heart_of_the_sea](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/20.png)  
海洋之心</br>  
![netherite_scrap](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/21.png)  
下界合金碎片（从工作台配方修改为切石机配方）</br>  
![calcite](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/22.gif)  
闪长岩烧炼为方解石（建筑党欢呼）</br>  
![dead_bush](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/23.gif)  
任意树苗烧炼为枯萎的灌木（包括杜鹃花从、盛开的杜鹃花从、红树胎生苗）</br>  
![deepslate](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/24.gif)  
平滑玄武岩烧炼为深板岩</br>  
![netherrack](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/25.gif)  
下界疣块/诡异疣块烧炼为下界岩</br>  
![notch_apple](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/26.png)  
加入了经典的附魔金苹果合成配方</br>  
![piglin_banner_pattern](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/27.png)
猪鼻旗帜图案的复制</br>  
![pigstep](https://github.com/JackHaozhu/image/blob/main/craftingdatapack/28.gif)  
用猪鼻旗帜图案将任意唱片灌录为Pigstep  
_<del>你也可以浪费一个旗帜图案来将Pigstep灌录为Pigstep</del>_



[^引用]:摘自[SunnySlopes](https://space.bilibili.com/100377977)的[专栏](https://www.bilibili.com/read/cv11805605)
[^数据包合成表]:数据包添加的合成配方无法保留物品的nbt数据
