# Systemd Web

Systemd Web 是一个 Systemd 的 Web UI 管理系统，通过直观的界面和易用的操作，让用户能够轻松地管理 Linux 系统和服务。该项目旨在简化 Systemd 的使用，使得无论是专业的系统管理员还是普通的用户，都能够方便地对系统进行操作。
## [github地址] (https://github.com/topascend/systemd-web2.0)

## 功能特性

### 基本操作功能

- **创建 service**: 通过web端创建service,简化服务器端的繁琐操作。
- **选择 service**: 通过web端选择已存在的service,简化命令行操作的复杂。
- **启动 (start)**: 通过简单的点击或命令，启动指定的服务。
- **停止 (stop)**: 停止正在运行的服务。
- **重启 (restart)**: 重启服务，以便应用最新的配置或解决临时问题。
- **查看运行状态 (status)**: 显示服务的当前状态，包括是否正在运行、运行时长等信息。
- **添加到开机启动项 (enable)**: 将服务添加到系统的开机启动项中，确保服务在系统启动时自动运行。
- **从开机启动中移除 (disable)**: 将服务从系统的开机启动项中移除，避免不必要的资源占用。

### 日志管理功能

Systemd Web 还提供了强大的日志管理功能，用户可以通过 Web 界面实时查看和管理 Systemd 的日志数据。

- **实时滚动日志(TailLog)**: 实时滚动显示最新的 Unit 日志数据**: 使用 `journalctl` 命令，用户可以在 Web 界面上实时查看最新的日志信息，了解系统和服务的运行状态。
- **查看历史日志(Log)**: 查看历史日志**: 默认显示 1 小时前的日志数据，用户还可以自由修改查看日志的时间范围，以便回顾和分析系统的历史运行情况。



## 安装步骤:
#### 1. 下载 systemd-web 文件放在linux任意目录,例如 /home/systemd-web/systemd-web
#### 2. 赋予执行权限 cd /home/systemd-web && chmod 7777 systemd-web
#### 3. 执行安装命令  ./systemd-web install
```
请输入要使用的端口号(默认9002):
请输入安全入口(默认4DPOVQF62T):
请输入登录用户名(默认admin):
请输入登录密码(默认TVC7I5JGSLMC):
2024-12-31T15:21:30 [INFO] 设置成功!
2024-12-31T15:21:30 [INFO] 命令执行成功!

[systemd-web]=================安装信息==================
[systemd-web] 端口号:9002
[systemd-web] 安全入口:4DPOVQF62T
[systemd-web] 用户名:admin
[systemd-web] 密码:TVC7I5JGSLMC
[systemd-web] 浏览器访问:
[systemd-web] http://192.168.122.132:9002/4DPOVQF62T
[systemd-web] http://127.0.0.1:9002/4DPOVQF62T
[systemd-web]=================安装信息==================
```
<img src="https://raw.githubusercontent.com/topascend/systemd-web2.0/main/a4.jpg" />
### 4. 默认自动启动,不需要此步 手动启动 ./systemd-web

### 访问 Web 界面

用户只需在浏览器中输入 `http://127.0.0.1:9002/XXXXXX` 即可访问 Systemd Web 的管理界面。界面设计简洁明了，操作便捷，用户无需深入了解 Systemd 的命令行操作即可轻松管理系统。

### 查看历史日志

用户可以通过访问特定的 URL 来查看历史日志，例如 `http://127.0.0.1:9002/log?app=systemd_web&hourAgo=-1`。通过调整 URL 中的 `hourAgo` 参数，用户可以方便地查看不同时间段的日志数据，从而更全面地了解系统的历史运行情况。

## 总结

Systemd Web 结合了 Systemd 的强大功能与 Web UI 的直观便捷，为 Linux 系统的管理带来了极大的便利。无论是专业的系统管理员还是普通的用户，都可以通过 Systemd Web 轻松地管理 Linux 系统和服务，确保系统的稳定性和功能的完整性。

<img src="https://raw.githubusercontent.com/topascend/systemd-web2.0/main/a1.jpg" />
<img src="https://raw.githubusercontent.com/topascend/systemd-web2.0/main/a2.jpg" />
<img src="https://raw.githubusercontent.com/topascend/systemd-web2.0/main/a3.jpg" />
<img src="https://raw.githubusercontent.com/topascend/systemd-web2.0/main/1.png" />
<img src="https://raw.githubusercontent.com/topascend/systemd-web2.0/main/2.png" />
<img src="https://raw.githubusercontent.com/topascend/systemd-web2.0/main/3.png" />


##  [阮一峰老师的Systemd教程](http://www.ruanyifeng.com/blog/2016/03/systemd-tutorial-commands.html)

### 感谢
#### GoFrame
GoFrame 是一款模块化、高性能、企业级的 Go Web 开发框架，它提供了丰富的功能和灵活的扩展性，使我们的后端开发变得更为高效和便捷。  
[GoFrame 官方文档](https://goframe.org/)

#### Layui
Layui 是一款非常受欢迎的前端 UI 框架，它以简单模块化的方式构建，为快速开发提供了良好的支持。Layui 的丰富组件和优美的界面设计，为我们的前端页面增色不少。  
[Layui 官方文档](https://github.com/layui/layui)  
  
