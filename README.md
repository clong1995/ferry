# ferry 消息摆渡程序
## 原生golang开发，无第三方依赖。可实现公网访问内网，或网络中电脑的消息传递。
在内网电脑上执行:
``` bash
mian -server quickex.com.cn:20080 -client 127.0.0.1:80
```
在公网服务器上执行:
``` bash
mian -server :20080 -public :18080
```  
## 链路实现  
进入 192.168.20.134:18080 -> 192.168.20.134:28080 -> 127.0.0.1:8009  
流出 192.168.20.134:18080 <- 192.168.20.134:28080 <- 127.0.0.1:8009
