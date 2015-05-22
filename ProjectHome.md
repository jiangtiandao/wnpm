# WNPM 3.5（Nginx + PHP + MySQL + Zend + eAccelerator + Memcached） #


```
WNPM目录结构：
\wnpm\
│ Readme.txt			说明文件
│ memcached.cmd			memcached服务安装启动脚本
│ WNPM.cmd			WNPM主程序
│ WNPM.conf			PHP&MySQL版本配置
│
├─ Cmds				WNPM启动控制脚本
│
├─ webserver			各种服务软件包
│  │ Process.exe		
│  │ RunHiddenConsole.exe	
│  ├─ eAccelerator		php加速器
│  ├─ mysql			mysql-5.1.60-winx64/mysql-5.5.19-winx64
│  ├─ php			php-5.2.17-Win32-VC6-x86/php-5.3.8-nts-Win32-VC9-x86
│  ├─ zend			Zend Optimizer-3.3.0
│  ├─ memcached			memcached-1.2.6-win32-bin
│  └─ nginx			nginx-1.1.12
│
└─ www
   │ index.php
   └─ phpMyAdmin		phpMyAdmin 3.4.0-rc1
```

```
新增：
Memcached Server
PHP支持Memcache和Redis模块

更新：
修复Windows下php-cgi自动关闭退出的问题
```

```
使用方法：
解压后请放于磁盘根目录，如E:\wnpm\
\wnpm\WNPM.cmd			WNPM启动、重启、停止、切换版本
\wnpm\webserver\nginx\vhost\	nginx虚拟主机配置文件存放目录
MySQL root密码：123456
```

```
说明：
php-5.2.17为线程安全版
支持Zend Optimizer

php-5.3.8为非线程安全版
支持eAccelerator
```

```
2013-9-11
作者：Zmor
E-mail：lure21@163.com
http://code.google.com/p/wnpm/

本软件仅限学习使用，未经许可禁止一切商业用途。
```


## http://pan.baidu.com/share/link?shareid=2363388511&uk=2013586172 ##
