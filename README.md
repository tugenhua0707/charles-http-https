## charles工具进行http/https抓包

#### 1. 首先下载charles，可以去charles官网下载，下载完成后记住下载一个charles.jar破解版包覆盖，如果不覆盖
试用期就是30天了；
## 安卓手机端对http及https进行抓包
### 一：手机端抓取http请求
#### 1. 设置代理(手机和电脑使用的是需要同一个网络)
#### 2. 查看我们的电脑的IP地址，及我们的charles的默认端口，打开 charles --> Proxy --> Proxy Settings 会看到HTTP Proxy的默认端口是8888；因此我们需要在手机端的网络改成 手动代理，然后把IP地址和端口号输进去即可抓
取到http请求的数据了；
### 二：手机端抓取https协议的包
#### 1. 设置charles ssl代理
#### Proxy --> SSL Proxy Settings 会弹出一个SSL代理设置界面；进行如下设置：
#### 1：Enable SSL Proxying 复选框勾上；
#### 2：添加我们想要的设置代理的域名，我们可以填写一个*号，对所有的https进行抓取；设置默认端口443；
如下图所示：
#### <img src="http://images2015.cnblogs.com/blog/561794/201607/561794-20160728003208825-162242806.png"/>
#### 3. 手机下载SSL证书；help--> SSL Proxying -> 选择下拉框列表第四项，这里就不写英文了；会弹出一个提示框
如下所示：
#### <img src="http://images2015.cnblogs.com/blog/561794/201607/561794-20160728003234153-806873645.png"/>
#### 4. 注意：使用安卓自带的浏览器在地址栏中访问 http://charlesproxy.com/getssl 即可下载证书；
选择WLAN（这里android，一定要选WLAN而不是VPNxxx），确定，完成！
#### 5. 完成后，我们现在可以使用手机访问网页，然后在电脑上使用charles抓取https请求了；

