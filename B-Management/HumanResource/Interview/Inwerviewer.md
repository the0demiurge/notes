# 面试总结

## 编程随想：招聘系列

苏格拉底式面试法，刨根问题一直问到本源。

[招聘的误区](https://program-think.blogspot.com/2009/04/defect-of-hire.html)

[俺的招聘经验](https://program-think.blogspot.com/2011/03/hiring-experience-0.html#index)

1. [面试 vs 笔试](https://program-think.blogspot.com/2011/03/hiring-experience-1.html)
2. [考察技术 vs 考察非技术](https://program-think.blogspot.com/2011/03/hiring-experience-2.html)：综合素质：智力因素（思维，沟通，创造）、非智力因素（性格、意志、兴趣）
3. [开放性问题 vs 封闭性问题](https://program-think.blogspot.com/2011/05/hiring-experience-3.html)：实践型问题，理解型问题（WHY），个性化问题，主观性问题（THINK）
4. [通过笔试答题能看出啥？](https://program-think.blogspot.com/2011/11/hiring-experience-4.html)：思路，规范性（排版，命名，注释），细心（审题），严密（边界条件），条理
5. [面试前的准备工作](https://program-think.blogspot.com/2012/12/hiring-experience-5.html)
6. 面谈的技巧
7. (未完待续)

## 问题总结

1. 常规问题：
   - 能来这干多久
   - 每周来几天
   - 什么时候能来
   - base 哪里

2. 强化学习
   1. 算法理解
      - 使用什么算法，算法细节，输入输出，网络设计
      - Model-based, model-free
      - On-policy, off-policy, 优劣
      - AC, Value-based, PG, 优劣
      - tricks, tricks有效的原因
      - nstep dqn为什么可以work，理论上和公式不相符(by gxy)
      - 为什么强化学习中batchnorm和dropout很少见(by gxy)
      - 收敛性的理论分析，各种因素对收敛性的影响，reward scale/正负对算法的理论影响(merged from gxy)
      - gae与td lambda的关系 为什么用gae(by gxy)
      - Over-estimated Q values
      - POMDP 有哪些类型和常见解决方法
      - RL 有哪些弱点和局限
   2. 工程经验
      - 状态/动作/回报怎么设计
      5. 如何判断训练是否正常(by gxy)
      - 使用什么指标评估效果，有baseline算法吗
      - 样本不平衡，reward稀疏
      - 过拟合
      - 调过哪些参数，哪些参数分别有什么影响
      - 不收敛的原因有哪些，如何解决
   
3. Linux
   - Bash里面 字符串单双引号区别
   - 权限，用户(chmod, chown), 比如644的权限，文件夹的 x 权限
   - 环境变量，写到各种地方的区别和原理
   - apt
   - 文本处理：grep, sed, awk, wc, uniq, history
   - 文件处理：find, du, df, lsblk
   - 进程：ps, top, fg, bg
   - 外置存储：mount, umount
   - 系统管理组件：systemctl, rc, init, crontab
   - 启动项：grub/systemd-boot
   
4. 操作系统
   - 进程/线程区别
   - 进程/线程通信
   - python进程/线程（GIL）
   - python进程启动方式区别
   - 堆区和栈区
5. 软件工程
   - git, git workflow
   - 如何设计整个代码架构（比如边写边改边抽象；提前设计好接口-自顶向下法或自底向上法等）
   - 设计模式
   - 代码量，文件量，分模块，各个模块功能
   - 代码规范化
   - 单元测试
   - 开源协议知道哪些
6. python/shell
   - python 优缺点
   - GIL
   - mutable
   - ==, is
   - 上下文管理器：with 的实现；装饰器的功能和实现
   - functools, logging, collections
   - yield, nonlocal, break
   - re
   - sort
   - Asyncio
   - 一切都是对象的理解
   - inspect, dir
   - 垃圾回收
7. C++开发
   - 开发规范：头文件写接口，cc 文件写实现
   - 用什么编译器编译命令
   - 库函数
   - Autopointer
   - segfault
- 内存/资源泄漏
   - 安全（内存/线程，以及不安全的函数）
   - makefile
8. 数据结构与算法
   - 矩阵运算（行列式，正定，逆，转置，特征值，解方程等等）
   - 递归（树，斐波那契数列）
   - 排序，稳定性，时空复杂度，复杂度推导
   - DFS, BFS
   - 链表（反转，找环，Y形链表）
   - 动态规划（求一下最长公共字符串），回溯（八皇后）
   - [qsort/mergesort](../1-Computer_Science/sort.py.md)/bubblesort/[二分查找](https://github.com/python/cpython/blob/master/Lib/bisect.py)/找中位数/topK/第K大数
   - 筛法

9. 非技术类：
   - （解决问题能力）遇到过过哪些很难的问题，如何解决
   - （学习能力）如何学习一个从没接触过的学科或者编程语言，有过哪些快速学习的经历
   - （学习能力）读过哪些强化学习方面资料/书籍/论文，资料中有哪些令人印象深刻的内容
   - （兴趣）生活中用编程做了哪些有趣的事情
   - （团队协作）在团队中怎么分工和合作

10. 有哪些想问我的问题