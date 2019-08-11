使用esp8266制作极简路由器

烧录软件地址：

https://github.com/dinoGong/docs/raw/master/esp8266/route/0/flash_download_tools_v3.6.6.zip

或者

https://github.com/dinoGong/docs/raw/master/esp8266/route/0/ESP8266Flasher.exe

下载固件：

https://github.com/dinoGong/docs/raw/master/esp8266/route/0/0x00000.bin
https://github.com/dinoGong/docs/raw/master/esp8266/route/0/0x02000.bin

烧录界面：

![](https://github.com/dinoGong/docs/raw/master/esp8266/route/0/1565450457740.png)
![](https://github.com/dinoGong/docs/raw/master/esp8266/route/0/1565450433636.png)


烧录完毕后，重新插拔一下esp8266。然后用电脑连接名为MyAP的wifi，无需密码。
![](https://github.com/dinoGong/docs/raw/master/esp8266/route/0/1565450787780.png)


连接后，打开192.168.4.1进行设置：

![](https://github.com/dinoGong/docs/raw/master/esp8266/route/0/1565450770156.png)

不要勾选Automesh

否则以后无法配置了

输入wifi和密码，点击Connect按钮。

这个时候会断开连接。然后重新连接MyAP。

设置你的热点和密码。点击set。这个时候，使用你的热点登录即可

设置完毕后，需要重新插拔一下esp8266才能生效。

以上。
