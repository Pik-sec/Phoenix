<img width="1176" alt="图片" src="https://user-images.githubusercontent.com/75553451/203336212-50e7bbfd-1177-426c-b4ef-be671d26f3d3.png">


# Phoenix简介

新一代目录扫描神器

Phoenix-不死鸟，能自动学习的目录扫描器，碰到重定向的目录会自己记录，并且滚动学习，所以不断的去使用它，可以把它越用越灵活，探测速度不亚于dirsearch

# 请继续关注！后续更新接口爬取功能！！



# 使用说明

## 简单使用

```
不想显示404，403 以及4xx任何状态码

Phoenix.exe -u http://www.test.com -t 25 -x 4xx

只是不想显示404 

Phoenix.exe -u http://www.test.com -t 25 -x 404

加入cookie 匹配状态码200

Phoenix.exe -u http://www.test.com -t 25 -c 输入cookie -mc 200

```

首先在将需要字典放在dict.txt文件中，或者在Phoenix目录下将字典改为名为dict.txt

```
-f 导入目标文件，批量扫描

-t 线程

-u 单个目标扫描，接上url 例 http://www.test.com

-c 加入cookie

-d 延迟处理

-mc 匹配状态码

-o 输出扫描日

-x 不想显示状态码 2xx/3xx/4xx/5xx/xxx 只能选择其中一个

```

## 11月22日 更新

支持 -x 2xx/3xx/4xx/5xx/xxx
