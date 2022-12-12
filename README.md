<img width="1176" alt="图片" src="https://user-images.githubusercontent.com/75553451/203336212-50e7bbfd-1177-426c-b4ef-be671d26f3d3.png">


# Phoenix简介

新一代目录扫描神器

Phoenix-不死鸟，探测速度不亚于dirsearch,先会去重处理，现在开始往字典加字典不用再考虑是否会重复，不死鸟将会帮你去重，不用考虑字典加的格式，无论是/a.php还是a.php,不死鸟将帮你格式字典，接口敏感度提升,-x 可以用,分开，不在单一排除

# 使用说明

## 简单使用

```
不想显示404，403 以及4xx任何状态码

Phoenix.exe -u http://www.test.com -t 25 -x 4xx

只是不想显示404 

Phoenix.exe -u http://www.test.com -t 25 -x 404,403,401

上面这个可以等于下面这个

Phoenix.exe -u http://www.test.com -t 25 -x 4xx 

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

-x  不想显示单个的状态码 404，302，500 ... (可以同时选择，分开)

    不想显示状态码 2xx/3xx/4xx/5xx/xxx (可以同时选择，分开)
    
    xxx为大于600的状态码

-p 代理,如 http://username:password@ip:port, http://ip:port

```

## 11月22日 更新

支持 -x 2xx/3xx/4xx/5xx/xxx

## 11月28日 更新

增加基础爬虫，进度条更新


## 12月1日 更新

302更新，删除自动学习，增加往字典中增加目录能够自动去重

目录增加格式 首字符去掉斜杆 如 1.php 不要写成 /1.php

## 12月7日 更新

加入代理，增加爬虫敏感度

## 12月12日 更新

更新 -x 可以选择多个 , 分开 ,去重改进，不需要再注意加入字典的格式，第一个字符有无/都能加入

[![Stargazers over time](https://starchart.cc/Pik-sec/Phoenix.svg)](https://starchart.cc/Pik-sec/Phoenix)


