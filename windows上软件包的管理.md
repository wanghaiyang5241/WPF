# windows上软件包的管理




<a name="D6f82"></a>
### 为什么要用软件包的管理?
因为软件包可以一键安装，省去去各种网站找exe安装包的过程，比如常用的rabbitmq、mysql、redis等等 配置虽然不复杂，但是过程相对比较繁琐，而且也没有一个统一的管理。
<a name="6bgIE"></a>
### 有哪些软件包的管理？
1：chocolatey 官网地址：[https://www.chocolatey.org/](https://www.chocolatey.org/)<br />2：scoop 平时用的比较少，所以不怎么关注。
<a name="Kvhvp"></a>
### choco如何使用？
参考网址：[https://blog.csdn.net/TianKongDeTangGuo/article/details/81167147](https://blog.csdn.net/TianKongDeTangGuo/article/details/81167147)，写的已经很全了。<br />设置代理：有些软件包是在墙外的，所以要通过设置代理去访问：choco config set proxy http://localhost:8888<br />（1）其中“[http://localhost:8888](http://localhost:8888)”是http代理，如果是自己本机的代理，可以用localhost或者127.0.0.1，如果其他机器的代理，那么其他机器的端口需要可以通过防火墙。<br />（2）目前官方说此代理如果是socks，可能会有问题 [https://chocolatey.org/docs/proxy-settings-for-chocolatey](https://chocolatey.org/docs/proxy-settings-for-chocolatey)<br />（3）所以如果你的代理如果是socks的，要通过privoxy来转换一下，可以参考[https://www.cnblogs.com/hongdada/p/10787924.html#2866070840](https://www.cnblogs.com/hongdada/p/10787924.html#2866070840)里面的 如何定制“SOCKS 代理转发”。
<a name="cT3HT"></a>
### 扩展资源
（1）socks是什么？<br />（2）privoxy是什么？可以参考：[https://www.cnblogs.com/hongdada/p/10787924.html](https://www.cnblogs.com/hongdada/p/10787924.html)<br />（3）代理跟vpn有什么区别？<br />以上这些都会以后有时间陆续发上去的。
