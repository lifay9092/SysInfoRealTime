# SysInfoRealTime
实时监控服务器信息：OS、内存、CPU等信息，并生成JSON格式的日志文件

##### 学习一下Golang，语法不过关还在慢慢摸索

基于[gopsutil](https://github.com/shirou/gopsutil)写了一个可以在不同os环境定时运行的监控程序，可以定期记录该服务器配置、实时CPU、实时内存等信息。后期本人应用主要是通过Web方式采集并可视化多个服务器的性能信息，结合服务请求数据、提供服务器性能瓶颈和扩展的基础数据支撑，以下为生成的JSON格式文件样例（按日期生成Log文件）
![image.png](https://upload-images.jianshu.io/upload_images/17879100-3b6b37f040fd2ae2.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![image.png](https://upload-images.jianshu.io/upload_images/17879100-243be2ea1915071a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

目前程序默认间隔时间为15秒，空置时间为每天21点-次日8点，需要调整的可以自行修改
