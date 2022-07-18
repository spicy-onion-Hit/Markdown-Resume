 <center>
     <h1>王仕林</h1>
     <div>
         <span>
             <img src="assets/phone-solid.svg" width="18px">
             15813710887
         </span>
         ·
         <span>
             <img src="assets/envelope-solid.svg" width="18px">
             570024873@qq.com
         </span>
         ·
         <span>
             <img src="assets/rss-solid.svg" width="18px">
             <a href="https://www.cnblogs.com/wsl-hitsz/">My Blog</a>
         </span>
     </div>
 </center>

 ## <img src="assets/info-circle-solid.svg" width="30px"> 个人信息 

 - 男，1996 年出生
 - 求职意向：C++  研发工程师


## <img src="assets/graduation-cap-solid.svg" width="30px"> 教育经历

- 硕士，哈尔滨工业大学，机械工程，2019.9~2022.1
- 学士，燕山大学，机械工程，2014.9~2018.7

## <img src="assets/briefcase-solid.svg" width="30px"> 工作经历

- **字节跳动 系统平台 ，后端研发 工程师，2022.2~2022.8**

   对接系统部门的各个资源，例如云主机、物理服务器、带宽、机柜等的管理、成本及收入账单生成，并通过财经分析平台接口推送相应的账单，提供hive表给下游数据分析，提供项目的api 接口完成关于财务相关的线上化流程。
   - 基于django web 框架，基于restful 风格，提供后端接口，以支持关于财务相关的线上化流程。
   - python bin 脚本通过http/mysql/hive 获取ods层面的数据，获取每日全量数据快照，生成相应的计算链路，注册相应的psm,在dorado 大数据平台进行相应的每日调度，推送日月账单
   - 基于hive拉去每日全量实例表，构造数据模型，基于ods->dwd->dwa模型的层级关系,生成日月账单，将hive表数据 迁移至 mysql，推送日月账单
   -  对python数据链路迁移至hive,完成数据链路优化，通过大数据平台实现对数据集成以及计算调度的闭环，完成对链路的管理和监控，便于后续的数仓统一建设和管理

## <img src="assets/project-diagram-solid.svg" width="30px"> 项目经历

- **基于reactor 模型的多并发web服务器**

  *项目技术： epoll I/O复用 线程池 HTTP*
  
    - 使用EPOLL 边沿触发监听I/O事件，设置非阻塞I/O，项目整体架构采用主从Reactor 模型，主 Reactor 只负责对I/O事件的的链路创建，subReactor 负责dispatch已经连接的 socket事件
    - 采用线程池避免了多线程创建销毁开销，对I/O信号进行解码编码处理
    - 使用状态机对HTTP协议进行解析，支持GET请求，支持长/短连接
    - 使用share_ptr 对项目内存进行管理，防止内存泄漏
- **高并发内存池(参考TC Malloc)**

  *项目技术： 内存碎片， TLS， 多线程*
  
    - 项目池使用三层结构，Thread Cache, Central Cache, Page Cache
    - 每一个线程具有独立的 Thread Cache, 小内存申请无需加锁，提高速度
    - Central Cache 通过全局锁机制，控制每一个线程内存的申请以及释放
    - Page Cache 回收Central Cache 的内存，并通过合并避免内存碎片，分配内存给Central Cache
      基于三层缓存结构，线程缓存、内存缓存、页缓存实现高效的内存分配方式，解决 内存碎片以及申请效率问题

## <img src="assets/tools-solid.svg" width="30px"> 技能

- 熟悉C++ 基础知识(指针，引用，内存管理)对C++ 面向对象思想封装、继承、多态 有较为深入了解
- 对python 语言有一定的了解
- 熟悉STL 库的基本容器的使用方法，掌握常见的数据结构
- 熟悉进程、线程的基本思想，对互斥锁、条件锁
- 熟悉TCP/IP 协议，对计算机的五层数据模型了解
- 了解 mysql 以及redis 的 基本使用方式
- 了解网络编程的基本API，了解epoll select IO 复用的基本特性
- 了解Linux操作系统，掌握常见的开发工具git