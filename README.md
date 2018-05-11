# DDNS

针对 Ubuntu 操作系统的动态域名解析（Dynamic DNS）的解决方案
 
## 准备工作

### 快速安装

* 克隆代码 
    
```
  git clone https://github.com/LaoLuMian/DDNS.git

```


* 填写配置信息
  * 选择本地网卡
  * 填写 noip 账号
  * 填写 noip 账号密码
  * 填写域名解析更新周期(分钟),比如 5

```
  ./DDNS-control config test-config

```
* 启动客户端

```
  ./DDNS-control start test-config
```

* 查看运行状态

```
  ./DDNS-control status test-config
```

### 卸载

* 停止运行

```
  ./DDNS-control stop <config-file>
```

* 删除配置文件

```
  ./DDNS-control clean <config-file>
```   
    
### 查看现有配置 

```
  ./DDNS-control list
```

### 更改 DDNS 更新周期

```
  ./DDNS-control update <config-file> <min>
```