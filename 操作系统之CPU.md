# 操作系统之CPU

<!--Note-->
## 应试要点：


### 死锁：
- 判断是否有死锁（结合图论中的环）
- 安全状态安全序列的判断
- 银行家算法
<!--/Note-->

## 进程

### 程序实例化

### 线程

#### 共享数据

### fork

## CPU调度

### 调度算法

#### 轮转法

#### 先来先服务

#### 最短作业优先

#### 优先级调度

#### 反馈队列

## 临界区问题

### 原子化操作

## 同步问题

## 死锁

### 死锁的解决

#### 死锁预防

<!--Note-->
###### 破坏死锁产生的四个条件：
####### ~~互斥mutual exclusion~~
- 共享访问
- 虚拟化技术/spooling
####### ~~保持和等待hold and wait~~
- 一次性申请，一次性分配
####### ~~不可抢占no~~
- 剥夺等待资源的进程所持有的资源
####### ~~循环等待circular waiting~~
- 给文件、设备等资源编号，进程需要递增式地申请，从而不会产生环

<!--/Note-->

#### 死锁避免

<!--Note-->
###### 安全序列与安全状态
###### 安全检测算法
###### 银行家算法
<!--/Note-->

#### 死锁检测和恢复

<!--Note-->
###### 死锁检测和恢复属于容错计算机
###### 死锁检测算法
- 检测环O（n^2）
- 安全检测算法
###### 死锁恢复策略
- kill进程（abort）-代价最小化、可能饥饿
	- 运行时间
    - 占用资源多少
    - 优先级
- 恢复到没有死锁的状态（rollback）
- watchdog（常用）
<!--/Note-->

#### 鸵鸟算法

UNIX、WINDOWS、LINUX

### 死锁产生的条件

#### 互斥

#### 保持和等待

#### 不可抢占

#### 循环等待

### 环与死锁

#### 有环不一定有死锁

#### 有环且等待的资源唯一，产生死锁

#### 有死锁一定有环，无环一定无死锁

## CPU状态

### 内核态

### 用户态
