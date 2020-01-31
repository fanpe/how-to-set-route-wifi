# how-to-set-route-wifi
如何设置从路由成AP模式
## 以下以openwrt为例：
* 进入管理后台后->无线->移除所有的无线网络（最好是线连接从路由器的任意一个LAN口）->扫描
![1](https://github.com/fanpe/how-to-set-route-wifi/blob/master/1.jpg)
* 找到主路由的WIFI名，加入网络，如下：
![2](https://github.com/fanpe/how-to-set-route-wifi/blob/master/2.jpg)
* 设置主路由WIFI一样的密码及加密方式
* 上图有radio0及radio1,因为从路由器是双频，故有两个随便选一个，找到那个主路由的WIFI加入网络即可
* 成功加入后，在另一个频率，这里因为radio1已经加入到主路由了，故我们只能在radio1设置你要连上从路由wifi密码及名称，**注意：这里WIFI名字及密码和主路由可以相同也可以不同，为了考虑自动切换问题，可以设置相同**
* 为了测试成功与否，你可以在无线界面最下面可以看到你的设备是否已连接并是否可上网
## PS：主路由器不用做任何设置，只需记住密码，具体要达到自动切换网络等功能还在摸索中，此方式即可实现双路由无需网线连接达到信号扩大WIFI信号的方案
