![lightning!](./imgs/lightning.png)



# 闪电

## 项目介绍

**lightning-web**

项目的 `WEB` 前端， 采用 主流的 Vue + Eelement-ui 来实现。

[lightning-web 仓库](https://github.com/zhengyansheng/lightning-web)



**lightning-ops**

以 `Python` 语言为主，采用 `django-restframework` 框架实现后端 *API* 模块开发。

- 服务树
- 作业平台
- CMDB
- API 权限系统

[lightning-ops 仓库](https://github.com/zhengyansheng/lightning-ops)



**lightning-go**

以 `Go` 语言为主，采用 **斗鱼** 微服务框架`Jupiter` 实现后端 *API* 模块开发。

- 多云管理
- 消息中心
- 定时任务
- 任务系统

[lightning-go 仓库](https://github.com/zhengyansheng/lightning-go)



## 模块架构

![ops-2021-arch](./imgs/ops-2021-arch.png)

## 项目地址



[项目Demo](http://www.aiops724.com/)



## 部署

### lightning-ops

克隆代码

```bash
$ git clone https://github.com/zhengyansheng/lightning-ops
$ cd lightning-ops
```

创建虚拟环境

```bash
$ python3.6 -m venv .venv
$ source .venv/bin/active
```

同步表结构到数据库

```bash
$ make migrate
```

启动*开发环境*服务

```bash
$ make run
```

启动*生产环境*服务

```bash
$ ./start.sh
```



### lightning-go

克隆代码

```bash
$ git clone https://github.com/zhengyansheng/lightning-go
$ cd lightning-go
```

下载项目依赖包

```bash
$ go get .
```

同步表结构到数据库

```bash
$ make migrate
```

启动*开发环境*服务

```bash
$ make run
```

启动*生产环境*服务

```bash
$ ./start.sh
```



### lightning-fe

克隆代码

```bash
$ git clone https://github.com/zhengyansheng/lightning-fe
$ cd lightning-fe
```

下载项目依赖包

```bash
$ npm install
```

同步表结构到数据库

```bash
$ make migrate
```

启动*开发环境*服务

```bash
$ npm run serve
```

启动*生产环境*服务

```bash
$ npm run build
```

