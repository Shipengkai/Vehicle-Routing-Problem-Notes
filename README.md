# Vehicle-Routing-Problem-Notes 
**Key difficulties and solutions in learning VRP problems**

## 1 最速VRP问题学习路线
&emsp;&emsp;以在**最短时间内获得基础VRP科研能力**为目标，给出一份**学习难度梯度上升**的简要学习路线，零基础也可以**轻松上手**。  
### 1.1 文献搜索、管理与阅读
&emsp;&emsp;1）文献搜索：[谷粉学术](https://gfsoso.99lb.net/scholar.html)和Scihub可以免科学上网搜索英文文献  
&emsp;&emsp;2）文献管理与阅读：推荐使用文献管理工具。我使用的是Zotero+若干插件，插件可以在github上搜索“zotero”找到，比较好用的有pdf翻译插件、文章颜色标签插件、自动下载插件、以及浏览器关联插件（浏览器商店中搜索zotero）。
    
### 1.2 VRP问题的建模与求解
#### 1.2.1 建模（1-3天）
&emsp;&emsp;各视频博客网站上能找到海量VRP建模教程，诸如“xxx-VRP问题建模实战”。然而这些教程良莠不齐，或重点讲解算法实现，或注重建模工具使用，甚至错误频出，未能讲清楚VRP问题的来龙去脉、问题描述与模型之间的对应关系。初学者在这类晦涩难懂却急功近利的教程中仿佛学了很多，但是到了知识应用的时候却无法写出正确合理的问题描述，更不必说建模了。  
&emsp;&emsp;基础知识的获取需要准确无误的知识来源，推荐精读Vehicle Routing Problems, Methods, and Applications, Second Edition by Paolo Toth, Daniele Vigo一书的**绪论与前两个模型**，该书在网络上可搜到免费电子版（https://librarygenesis.pro/）。  
&emsp;&emsp;完全吃透本书前两个CVRP的问题描述与模型，学会根据问题一条一条公式搭建模型（请勿A文章的模型+B文章的一条约束+C文章的一条约束+...），可以建立牢固的基础。  
&emsp;&emsp;**避坑**：xx实战教程、CSDN上的模型、未验证模型的论文  
#### 1.2.2 求解器求解（1-2周）
&emsp;&emsp;以Gurobi+Python为例，可以跟着bilibili“[大规模优化求解器-Gurobi-教程”的课程一](https://www.bilibili.com/video/BV1jt411b73m)完成下载安装，同时搭建conda+python环境，申请gurobi资格，并加入官网qq群,视频是19年的，有出现疑问的地方qq群文件可以找到答案。Gurobi求解器的中国团队非常nice，邮件申请个人学术资格仅需几小时，qq群中的老师回答提问很迅速。
&emsp;&emsp;这一部分需要学会：1）Python最简单的基础语法；2）编程学习中遇到疑问请学会查阅python、gurobi、matplotlib的官网帮助文档或向chatgpt提问（请避免百度搜索或CSDN）,另外请学会使用chatgpt写代码和修改代码，让chatgpt当码农，自己当老板负责指指点点。3）复现[Gurobi解决VRP问题（Python接口）](https://www.bilibili.com/video/BV1wU4y1W7jD)bilibili若失效请前往https://youtu.be/7_-Xuq2xKdc
#### 1.2.3 启发式算法（1-2月）
&emsp;&emsp;实现一个VRP问题的启发式算法并不简单，尤其在需要求解的问题与他人研究差别较大时更加困难，下载一份现成代码并简单修改最多得到晕乎乎的大脑和很差的求解结果。  
&emsp;&emsp;1）首先必学数据结构与算法课程（可以跟着任意“数据结构与算法python”视频学习、勤动手），达到：能够解答LeetCode上的简单题，看到一个计算过程能知道它的时间复杂度。  
&emsp;&emsp;2）然后学习[墨尔本大学discrete optimization线上课程](https://www.bilibili.com/video/BV1z84y1h7M1)的TSP与VRP部分，其余部分按需学习有助于了解经典算法的设计方式从而获得算法设计灵感。  
&emsp;&emsp;当你需要某个算法时，使用github搜索，找到高star仓库，远比CSDN、微信公众号等渠道靠谱。很多经典算法pipy上有现成的包（俗称“轮子”）提供支持，可以避免重复造轮子，学习时可以阅读该包的帮助文档。
