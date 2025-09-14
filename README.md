# Dia-PROXY
用于Dia浏览器的小火箭规则，防止出现奇怪的错误(免得一直跳Error) 

我主要是用小火箭shadowrocket，经常更新配置导致老是需要自己重复读取日志获取规则，干脆打出来放出来。其他代理软件通用哈！

以下规则去美国节点🇺🇸

```
[Rule]
DOMAIN-SUFFIX,account.diabrowser.engineering
DOMAIN-SUFFIX,ai-service.diabrowser.engineering
DOMAIN-SUFFIX,clientstream.launchdarkly.com
DOMAIN-SUFFIX,releases.diabrowser.com
```

测试过加了这几条，一般就不会在启动台用户登录时及dia对话失败。

不知道怎么添加的看下图，在配置-（你正在使用的配置边上的！）-右上角加号添加

<img width="627" height="746" alt="image" src="https://github.com/user-attachments/assets/3419bfe2-1254-4e56-b3d5-dc17b756c08a" />

添加完 完整 纯文本 显示如下：
“IEPL|US 美国03 MITM”替换成你自己的美国节点
```
[Rule]
DOMAIN-SUFFIX,account.diabrowser.engineering,IEPL|US 美国03 MITM
DOMAIN-SUFFIX,ai-service.diabrowser.engineering,IEPL|US 美国03 MITM
DOMAIN-SUFFIX,clientstream.launchdarkly.com,IEPL|US 美国03 MITM
DOMAIN-SUFFIX,releases.diabrowser.com,IEPL|US 美国03 MITM
```

[***dia.conf***](https://raw.githubusercontent.com/QIAO1520/Dia-PROXY/refs/heads/main/dia.conf) 
