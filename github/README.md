# 优化GitHub加载太慢问题
- 在浏览器中打开DNS查询网站http://tool.chinaz.com/dns
- 分别输入github.com、github.global.ssl.fastly.net对应的IP，查找反应时间最少的IP地址
- 在hosts文件中增加映射
~~~
192.30.xx.xx github.com
151.101.xx.xx github.global.ssl.fastly.net
~~~
- 最后刷新DNS：ipconfig /flushdns
