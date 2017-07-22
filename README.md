# ServerStatus： 

* ServerStatus是一个酷炫高逼格的云探针、云监控、服务器云监控、多服务器探针~，该云监控（云探针）是ServerStatus（ https://github.com/tenyue/ServerStatus ）项目的优化/修改版。
    

# 目录介绍：

* clients  客户端文件
* server   服务端文件
* web      网站文件  

# 更新说明：
* 20170722, 修复客户端安装问题
* 20170719, 优化单位进制显示
* 20170430, 优化手机显示式样
* 20170429, 去除主机名设定
* 20170427, 增加一键部署脚本

# 安装说明：     

* 注意:Centos6自带Python版本位2.6,并不能支持客户端正常运行,请自行更换系统或升级Python为2.7及以上

执行下面的代码下载并运行脚本。
``` bash
wget -N --no-check-certificate https://raw.githubusercontent.com/FeulerLoup/scripts/master/tz.sh && chmod +x tz.sh
```
下载脚本后，根据需要安装客户端或者服务端：
``` bash
# 显示客户端管理菜单
bash tz.sh c
 
# 显示服务端管理菜单
bash tz.sh s
```
然后选择你要执行的选项即可。


### 客户端：

启动：service status-client start

停止：service status-client stop

重启：service status-client restart

查看状态：service status-client status

### 服务端：

启动：service status-server start

停止：service status-server stop

重启：service status-server restart

查看状态：service status-server status

### Caddy（HTTP服务）：

启动：service caddy start

停止：service caddy stop

重启：service caddy restart

查看状态：service caddy status

Caddy配置文件：/usr/local/caddy/caddy


——————————————————————————————————————

安装目录：/usr/local/ServerStatus

网页文件：/usr/local/ServerStatus/web

配置文件：/usr/local/ServerStatus/server/config.json

客户端查看日志：tail -f tmp/serverstatus_client.log

服务端查看日志：tail -f /tmp/serverstatus_server.log


# 相关开源项目，感谢： 

* ServerStatus：https://github.com/BotoX/ServerStatus
* ServerStatus-Toyo：https://github.com/ToyoDAdoubi/ServerStatus-Toyo
* mojeda: https://github.com/mojeda 
* mojeda's ServerStatus: https://github.com/mojeda/ServerStatus
* BlueVM's project: http://www.lowendtalk.com/discussion/comment/169690#Comment_169690
