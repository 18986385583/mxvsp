# 美渲虚拟串口

“MX虚拟串口”具有虚拟串口对、串口分身、串口聚合、串口群组、串口转tcp客户端、串口转tcp服务端等功能，应用只需面向串口开发，就可以完成几乎所有的通信能力。

# 工具/原料

MX虚拟串口
 [点击从官网下载]( http://www.meixuannet.cn/)
&nbsp;
&nbsp;

# 功能点
功能点说明如下：
&nbsp;
&nbsp;

## 虚拟串口对

在计算机中虚拟出两个配对串口，从其中一个发送数据，另一个能够即可收到，反之依
然。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190423085819777.png)
&nbsp;

## 串口分身

将一个真实串口（物理串口）拆分成多个虚拟串口，每个虚拟串口都直接映射这个真实串口，如，多个应用程序访问同一个硬件设备。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190423085927683.png)
&nbsp;

## 串口聚合

多个真实串口（物理串口）合成一个虚拟串口，能够接收到所有真实串口的数据，聚合串口发出的数据能够转发给全部真实串口。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190423085957560.png)
&nbsp;

## 串口群组

串口群组内可以有真实串口（物理串口）和虚拟串口，任何一个串口发送的数据都可以在其它串口输出。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190423090023653.png)
&nbsp;
## 串口转TCP客户端

串口数据透过TCP网络连接到远程服务器上，同时接收远程服务器数据，通过串口输出过来。

![在这里插入图片描述](https://img-blog.csdnimg.cn/2019042309004897.png)
&nbsp;
##  串口转TCP服务端

将TCP服务器端接收到的数据通过串口输出给应用程序，通常和串口客户端配合使用，建立两台远程主机之间的之间串口通信。


![在这里插入图片描述](https://img-blog.csdnimg.cn/20190423090111914.png)
&nbsp;
# 使用方法/步骤
&nbsp;
> 下载安装“MX虚拟串口”

到官网下载  http://www.meixuannet.cn/

&nbsp;
>  创建“虚拟串口对”，虚拟出两个串口，实现相互通信

说明：虚拟串口不需要设置波特率，任意波特率均可

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190423090212883.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2NpY296aGFuZw==,size_16,color_FFFFFF,t_70)

&nbsp;
> 创建“串口分身”，将真实串口分成多个虚拟串口，可让多个软件访问同一台设备

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190423090230600.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2NpY296aGFuZw==,size_16,color_FFFFFF,t_70)
&nbsp;
> 创建“串口聚合”，将多个真实串口合成一个虚拟串口，一个软件可访问多台设备。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190423090251703.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2NpY296aGFuZw==,size_16,color_FFFFFF,t_70)

&nbsp;
> 创建“串口群组”，向群组中任何串口发送数据，其它串口都能接收到。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190423090308855.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2NpY296aGFuZw==,size_16,color_FFFFFF,t_70)
&nbsp;
> 创建“串口TCP客户端”，实现串口转tcp网络，写入串口的数据会发给远程tcp服务器，方便实现远程串口应用。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190423090326702.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2NpY296aGFuZw==,size_16,color_FFFFFF,t_70)
&nbsp;
> 创建“串口TCP服务端”，实现tcp服务端网络转串口，如果安装在云服务器上，可将DTU的数据通过串口发送给应用软件。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190423090343840.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2NpY296aGFuZw==,size_16,color_FFFFFF,t_70)
&nbsp;
&nbsp;
# 注意事项
1. 虚拟串口不需要设置波特率
2. 在云服务器上使用“串口服务端”时，需要服务器开通端口访问权限
3. 如果真实串口没有识别出来，重新插拔或检查是否有虚拟串口名称冲突

&nbsp;

![在这里插入图片描述](https://img-blog.csdnimg.cn/20190423090744316.png)
美渲网络，精美出品
http://www.meixuannet.cn
