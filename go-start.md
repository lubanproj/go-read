@[TOC](Let`s go start)

# go入门

大家好！欢迎大家一起学习go语言。下面主要分享一些go语言入门的资料。我们知道学习一门语言方式可能有很多，但是都离不开基本语法的了解和学习，并不断练习使用基本语法写出一些稍微复杂的程序，再就是慢慢了解这门语言的一些高级特性，并在工作和生活中不断运用，并不断复习总结，在使用过程中不断复盘，同时将自己所理解的和大家一份分享和学习交流，可能也许这就是费曼学习法吧。坚持下去我们就会慢慢掌握甚至精通这门语言。

## go 语言历史



  
 1.go语言是一门新的语言，Go 语言起源 2007 年，并于 2009 年正式对外发布。它从 2009 年 9 月 21 日开始作为谷歌公司 20% 兼职项目，即相关员工利用 20% 的空余时间来参与 Go 语言的研发工作。<br>
 2. 大事件 <br>
2007 年 ：雏形设计 <br>
2009 年 ：首次公开发布 <br>
2010 年 ：当选 2009 年年度语言，谷歌投入使用 <br>
2011 年 ：Google App Engine 支持 Go 语言<br>
 3. 使用Go的项目<br>
Docker, a set of tools for deploying Linux containers<br>
Doozer, a lock service by managed hosting provider Heroku<br>
Gogs, self-hosted Git Service.<br>
Drone, Drone is a self-service Continuous Delivery platform for busy development teams.<br>
InfluxDB, an open source database specifically to handle time series data with high availability and high performance requirements.<br>
Juju, a service orchestration tool by Canonical, packagers of Ubuntu Linux<br>
Packer, a tool for creating identical machine images for multiple platforms from a single source configuration<br>
Snappy, a package manager for Ubuntu phone developed by Canonical.<br>
Syncthing, an open-source file synchronization client/server application<br>
 4. 创始人 
该项目的三位领导者均是著名的 IT 工程师：<br>
罗伯特·格瑞史莫(Robert Griesemer)     Google V8引擎 & JVM HotSpot 开发者<br>
罗勃特·派克(Rob Pike)    Unix早期开发者 & UTF-8创始人<br>
肯尼斯·汤普逊(Ken Thompson)    Unix & C 创始人  1983图灵奖获得者 <br>
 5. 国内使用go公司：七牛，阿里，百度，腾讯，头条，京东、、、


## go入门网站链接

官网地址: [https://golang.google.cn  文档](https://golang.google.cn)<br>
菜鸟教程：[https://www.runoob.com/go/go-tutorial.html 文档](https://www.runoob.com/go/go-tutorial.html)<br>
慕课网教程：[https://www.imooc.com/learn/968 视频](https://www.imooc.com/learn/968)<br>
b站教程：[https://www.bilibili.com/video/av57512936?t=122 视频](https://www.bilibili.com/video/av57512936?t=122)<br>


##  go有什么优势呢，那为什么我们要学习go? 
 1.   学习曲线容易:Go语言语法简单，包含了类C语法。因为Go语言容易学习，所以一个普通的大学生花几个星期就能写出来可以上手的、高性能的应用。在国内大家都追求快，这也是为什么国内Go流行的原因之一。<br>   
 ![Alt](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9hdmF0YXIuY3Nkbi5uZXQvNy83L0IvMV9yYWxmX2h4MTYzY29tLmpwZw==#pic_center) 
 2. 效率：快速的编译时间，开发效率和运行效率高，开发过程中相较于 Java 和 C++呆滞的编译速度，Go 的快速编译时间是一个主要的效率优势。Go拥有接近C的运行效率和接近PHP的开发效率。<br>
 ![Alt](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9hdmF0YXIuY3Nkbi5uZXQvNy83L0IvMV9yYWxmX2h4MTYzY29tLmpwZw==#pic_center)
 <br>
 C 语言的理念是信任程序员，保持语言的小巧，不屏蔽底层且底层友好，关注语言的执行效率和性能。而 Python 的姿态是用尽量少的代码完成尽量多的事。于是我能够感觉到，Go 语言想要把 C 和 Python 统一起来，这是多棒的一件事啊<br>
 ![Alt](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9hdmF0YXIuY3Nkbi5uZXQvNy83L0IvMV9yYWxmX2h4MTYzY29tLmpwZw==#pic_center)
 3. 出身名门、血统纯正：之所以说Go出身名门，从Go语言的创造者就可见端倪，Go语言绝对血统纯正。其次Go语言出自Google公司，Google在业界的知名度和实力自然不用多说。Google公司聚集了一批牛人，在各种编程语言称雄争霸的局面下推出新的编程语言，自然有它的战略考虑。而且从Go语言的发展态势来看，Google对它这个新的宠儿还是很看重的，Go自然有一个良好的发展前途。<br>
 ![Alt](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9hdmF0YXIuY3Nkbi5uZXQvNy83L0IvMV9yYWxmX2h4MTYzY29tLmpwZw==#pic_center)
 4. 自由高效：组合的思想、无侵入式的接口：Go语言可以说是开发效率和运行效率二者的完美融合，天生的并发编程支持。Go语言支持当前所有的编程范式，包括过程式编程、面向对象编程、面向接口编程、函数式编程。程序员们可以各取所需、自由组合、想怎么玩就怎么玩。
 5. 强大的标准库：这包括互联网应用、系统编程和网络编程。Go里面的标准库基本上已经是非常稳定了，特别是我这里提到的三个，网络层、系统层的库非常实用。Go 语言的 lib 库麻雀虽小五脏俱全。Go 语言的 lib 库中基本上有绝大多数常用的库，虽然有些库还不是很好，但我觉得不是问题，因为我相信在未来的发展中会把这些问题解决掉。
 6. 部署方便：二进制文件，Copy部署：这一点是很多人选择Go的最大理由，因为部署太方便了，所以现在也有很多人用Go开发运维程序。
 7. 简单的并发：并行和异步编程几乎无痛点。Go 语言的 Goroutine 和 Channel 这两个神器简直就是并发和异步编程的巨大福音。像 C、C++、Java、Python 和 JavaScript 这些语言的并发和异步方式太控制就比较复杂了，而且容易出错，而 Go 解决这个问题非常地优雅和流畅。这对于编程多年受尽并发和异步折磨的编程者来说，完全就是让人眼前一亮的感觉。Go 是一种非常高效的语言，高度支持并发性。Go是为大数据、微服务、并发而生的一种编程语言。
Go 作为一门语言致力于使事情简单化。它并未引入很多新概念，而是聚焦于打造一门简单的语言，它使用起来异常快速并且简单。其唯一的创新之处是 goroutines 和通道。Goroutines 是 Go 面向线程的轻量级方法，而通道是 goroutines 之间通信的优先方式。
创建 Goroutines 的成本很低，只需几千个字节的额外内存，正由于此，才使得同时运行数百个甚至数千个 goroutines 成为可能。可以借助通道实现 goroutines 之间的通信。Goroutines 以及基于通道的并发性方法使其非常容易使用所有可用的 CPU 内核，并处理并发的 IO。相较于 Python/Java，在一个 goroutine 上运行一个函数需要最小的代码。<br>
![Alt](https://imgconvert.csdnimg.cn/aHR0cHM6Ly9hdmF0YXIuY3Nkbi5uZXQvNy83L0IvMV9yYWxmX2h4MTYzY29tLmpwZw==#pic_center)
 8. 稳定性：Go拥有强大的编译检查、严格的编码规范和完整的软件生命周期工具，具有很强的稳定性，稳定压倒一切。那么为什么Go相比于其他程序会更稳定呢？这是因为Go提供了软件生命周期（开发、测试、部署、维护等等）的各个环节的工具，如go tool、gofmt、go test。<br>
# go进阶 （待补充..TODO）
大家好！欢迎大家一起学习go语言。下面主要分享一些go语言进阶的资料。我们知道学习一门语言方式可能有很多，但是都离不开基本语法的了解和学习，并不断练习使用基本语法写出一些稍微复杂的程序，再就是慢慢了解这门语言的一些高级特性，并在工作和生活中不断运用，并不断复习总结，在使用过程中不断复盘，同时将自己所理解的和大家一份分享和学习交流，可能也许这就是费曼学习法吧。坚持下去我们就会慢慢掌握甚至精通这门语言。

## go进阶网站链接
b站教程：[https://www.bilibili.com/video/av57512936?t=122 视频](https://www.bilibili.com/video/av57512936?t=122)





