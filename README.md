# Vehicle-Routing-Problem-Notes 
> **Key difficulties and solutions in learning VRP problems**  
> 很高兴能帮助到你，别忘了点击右上角的⭐   
> 如果你有任何建议，欢迎发送至shipengkai1@gmail.com

## 1 VRP问题-最速学习路线:running:(经验之谈仅供参考)   
一份**学习难度梯度上升**的简要学习路线，旨在帮助初学者**在短时间内获得基础VRP科研能力**，零基础也可以**轻松上手**。     
  
### 1.1 文献搜索、管理与阅读
- 文献搜索：[谷粉学术](https://gfsoso.99lb.net/scholar.html)和Scihub可以免科学上网搜索英文文献。  
- 文献管理与阅读：推荐使用文献管理工具。如：[Zotero](https://www.zotero.org)+若干插件，插件可以在github上搜索“zotero”获取，推荐[zotero-pdf翻译](https://github.com/windingwind/zotero-pdf-translate)、[zotero-sichub自动下载](https://github.com/ethanwillis/zotero-scihub)、以及浏览器关联插件（浏览器商店中搜索zotero）。   

### 1.2 VRP问题的建模与求解
#### 1.2.1 建模（1-3天）
- 各种视频、博客网站上能找到海量VRP建模教程，诸如“xxx-VRP问题建模实战”。然而这些教程良莠不齐，或重点讲解算法实现，或注重建模工具使用，甚至错误频出，未能讲清楚VRP问题的来龙去脉、**问题描述与模型之间的推导过程**。初学者在这类晦涩难懂却急功近利的教程中仿佛学了很多，等到知识应用的时候却无法写出正确合理的问题描述，更不必说建模。    
- 基础知识的学习需要准确无误的来源，推荐精读[Vehicle Routing Problems, Methods, and Applications, Second Edition by Paolo Toth, Daniele Vigo](https://librarygenesis.pro)的**绪论与前两个模型**。完全吃透书中前两个CVRP的问题描述与模型，以此学会根据问题描述逐条写出公式，最终建立模型（请勿A文章的模型+B文章的一条约束+C文章的一条约束+...）。    
>避坑：xxx实战教程、CSDN上的模型、未验证模型的论文    
#### 1.2.2 求解器求解（1-2周，以Gurobi+Python为例）
- 参照视频“[大规模优化求解器-Gurobi-教程”的课程一](https://www.bilibili.com/video/BV1jt411b73m)搭建conda+python环境并[申请Gurobi资格](http://www.gurobi.cn/NewsView1.Asp?id=4)。另外推荐加入官方q群,答疑老师超级负责。   
- 需要学会：  
 1）Python最基础的语法；   
 2）解决疑难时~百度或CSDN~查阅[python](https://docs.python.org/zh-cn/3/)、Gurobi、matplotlib的**官网帮助文档**或**向Chatgpt提问**，Chatgpt亦可成为你的码农；    
 3）独立复现[Gurobi解决VRP问题（Python接口）](https://www.bilibili.com/video/BV1wU4y1W7jD)。  
#### 1.2.3 启发式算法（1-2月）
- 实现VRP启发式算法并非易事，尤其在研究的问题比较新颖时。初学者下载一份现成代码并简单修改会导致很差的结果和混乱的头脑。  
1）必学**数据结构与算法**（可以跟着任意“数据结构与算法python”视频勤动手），务必达到：a、能独立完成[LeetCode简单题](https://leetcode.cn/problemset/all/?difficulty=EASY&page=1)；b、能轻松看出计算过程的时间复杂度。    
2）必学[墨尔本大学discrete optimization线上课程](https://www.bilibili.com/video/BV1z84y1h7M1)的TSP与VRP部分，其余部分按需学习可获得算法设计灵感。   
> 当你需要某个算法时，使用~CSDN、微信公众号~github搜索,例如
> 经典算法pipy一般有现成包和帮助文档（俗称“轮子”），善用以避免重复劳动.例如：
> - [多目标优化算法包pymoo](https://www.pymoo.org/),
> - [自适应大领域搜索包alns](https://alns.readthedocs.io/en/latest/index.html),
> - [个人笔记py-ga-VRPTW](https://github.com/iRB-Lab/py-ga-VRPTW)

      
******
- 作者：Ezreal S
- github地址：https://github.com/Shipengkai/Vehicle-Routing-Problem-Notes
- 仅供参考-转载请注明出处
