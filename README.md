# Dia-PROXY
用于Dia浏览器的小火箭规则，防止出现奇怪的错误(免得一直跳Error) 

我主要是用小火箭shadowrocket，经常更新配置导致老是需要自己重复读取日志获取规则，干脆打出来放在L站。其他代理软件通用哈！

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

![image|420x500](upload://d1wZff9pcRLM4oKZMSvGUjvft23.jpeg)
