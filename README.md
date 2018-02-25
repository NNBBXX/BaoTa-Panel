# 宝塔面板 linux版本 5.6.0
![image](https://www.bt.cn/bbs/newsimg/5.6.jpg)


# 前言

我只是大自然的搬运工，这里分享的是宝塔面板安装所用到的所有文件（我能找到的文件）。

有环境文件，有宝塔的面板代码源文件。

bt文件夹里的文件在宝塔安装过程中会自动下载

bt_code文件夹里的文件是宝塔面板的源码也会在安装过程中自动下载。

bt.init 宝塔面板PyWeb配置文件

install.sh Centos/Fedora安装文件 

install-ubuntu.sh Ubuntu/Deepin/Debian安装文件

宝塔安装需要的程序chardet-2.3.0、MySQL-python-1.2.5、psutil-5.2.2、Pillow-3.2.0、setuptools-33.1.1、web.py-0.38

panel是宝塔的面板源码。update.sh面板更新文件。uninstall.sh面板卸载软件

## 安装要求：

Python版本： 2.6/2.7（安装宝塔时会自动安装）
内存：128M以上，推荐512M以上（纯面板约占系统10M内存）

硬盘：100M以上可用硬盘空间（纯面板约占20M磁盘空间）

系统：CentOS 6.x / 7.x (Ubuntu、Debian、Fedora 请点这里)，确保是干净的操作系统，没有安装过其它环境带的Apache/Nginx/php/MySQL

#### 以下主机商必看（开端口教程，不开不能用）：
腾讯云：[https://www.bt.cn/bbs/thread-1229-1-1.html](https://www.bt.cn/bbs/thread-1229-1-1.html)

阿里云：[https://www.bt.cn/bbs/thread-2897-1-1.html](https://www.bt.cn/bbs/thread-2897-1-1.html)

华为云：[https://www.bt.cn/bbs/thread-3923-1-1.html](https://www.bt.cn/bbs/thread-3923-1-1.html)

## Linux面板5.6.0安装命令：

**Centos/Fedora安装命令：**

```
sh install.sh
```

**Ubuntu/Deepin/Debian安装命令：**

```
bash install-ubuntu.sh
```

## 更新命令（仅限3.x以上版本使用！不支持2.X面板！）：

```
sh /www/server/panel/update.sh
```

**若点击更新后没生效，请尝试重启面板服务：**

```
service bt restart
```


## 面板特色功能：

1. 一键配置服务器环境（LAMP/LNMP）
1. 一键安全重启
1. 一键创建管理网站、ftp、数据库
1. 一键配置（定期备份、数据导入、伪静态、301、SSL、子目录、反向代理、切换PHP版本）
1. 一键安装常用PHP扩展(fileinfo、intl、opcache、imap、memcache、apc、redis、ioncube、imagick)
1. 数据库一键导入导出
1. 系统监控（CPU、内存、磁盘IO、网络IO）
1. 防火墙端口放行
1. SSH开启与关闭及SSH端口更改
1. 禁PING开启或关闭
1. 方便高效的文件管理器（上传、下载、压缩、解压、查看、编辑等等）
1. 计划任务（定期备份、日志切割、shell脚本）
1. 软件管理（一键安装、卸载、版本切换）

#### 5.6.0更新内容：
1. 增强php的安装稳定性
2. 提高apache2.4/mysql高并发下的负载能力(仅新安装的)
3. 增加mysql慢日志(仅新安装的)
4. 更新mysql源码包
5. 添加数据库时允许自定义用户名
6. 设置数据库权限时允许多个许可IP
7. 优化nginx反向代理配置
8. 修正redis/memcached状态中的命中率算法错误
9. 增加内存盘工具(在Linux工具箱插件)
10. 增加PHP-FPM日志显示
11. 增加PHP慢日志显示
12. 优化PHP安装扩展页面的交互逻辑
13. 增加DNS云解析插件(感谢dns.com提供技术支持)
14. 优化面板系统资源调度程序，提升面板稳定性
15. 重做代码安全审计，修复所有已知安全隐患
16. 重新优化下载节点检测程序，减少部分地区安装软件时可能出现的卡顿
17. 其它细节调整

#### 以下为部分功能预览图：
软件管理
![image](https://www.bt.cn/bbs/newsimg/rjgl.jpg)

面板设置

![image](https://www.bt.cn/bbs/newsimg/mbsz.jpg)


SSL

![image](https://www.bt.cn/bbs/newsimg/ssl.jpg)


文件管理

![image](https://www.bt.cn/bbs/newsimg/pic5.png)


监控

![image](https://www.bt.cn/bbs/newsimg/control.jpg)


计划任务

![image](https://www.bt.cn/bbs/newsimg/beifen.jpg)


网络管理

![image](https://www.bt.cn/bbs/newsimg/pic8.png)


进程管理

![image](https://www.bt.cn/bbs/newsimg/pic9.png)


PHP扩展

![image](https://www.bt.cn/bbs/newsimg/pic10.png)


服务器跑分

![image](https://www.bt.cn/bbs/newsimg/fwqpf.jpg)


一键部署源码

![https://www.bt.cn/bbs/data/attachment/forum/201707/31/083934mbvv42m3dwwwtjwm.jpg](https://www.bt.cn/bbs/data/attachment/forum/201707/31/083934mbvv42m3dwwwtjwm.jpg)


以上为部分功能界面截图，如需了解更多，敬请安装体验，一行代码，2分钟能装好，完全免费。