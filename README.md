# Server_projects
Server High Concurrency Communication Framework with Business Logic Framework

linux环境下实现服务器高并发通讯框架 + 业务逻辑框架

项目包括：

(1)项目是完整的多线程高并发服务器程序

(2)按照包头 + 包体格式 收，完美的解决了数据粘包的问题

(3)根据收到的数据包 来执行不同的业务逻辑

(4)把业务处理产生的结果数据包正确的返回给客户端

(5)心跳包的实现、虚假唤醒、flood攻击应对

(6)控制客户端连入数，以及防范黑客-畸形包以及恶意用户的应对

(7)专门处理数据发送的一整套数据发送逻辑以及发送线程；

用到的主要开发技术：

(1)epoll高并发通讯技术，用的是水平触发模式【LT】

(2)通过线程池技术处理业务逻辑

(3)多线程，线程之间的同步技术包括互斥量、信号量、条件变量等等

(4)次要技术：单例模式，信号，日志打印，更改标题、fork()创建子进程，守护进程

(5)连接池中的连接的延迟回收。
