# google-cloud-shell1

# 启动地址： https://ssh.cloud.google.com/

Google Cloud Shell 让您可以直接在浏览器中通过命令行访问云端资源。您可以轻松管理项目和资源，而无需在系统上安装 Google Cloud SDK 或其他工具。Cloud Shell 让您可以根据自己的需要，随时使用最新且经过全面身份验证的 Cloud SDK gcloud 命令行以及其他必要的实用工具。

# 官方文档： https://cloud.google.com/shell/docs

# Cloud Shell 预装了许多您喜爱的命令行工具
包括 bash 和 sh，以及 emacs 和 vim，并且均为最新版本。MySQL 客户端、Docker 和 Kubernetes 等管理工具已配置完毕并准备就绪

# 方案
下载安装官方SDK： https://cloud.google.com/sdk/docs/downloads-versioned-archives

FinalShell：点击下载

命令
初始化： gcloud init

启动：gcloud alpha cloud-shell ssh

选择区域：gcloud config set compute/region us-east1

目前 可用计划任务，防止掉线。配额还在测试！


# 防掉线
可以用Shell 或 PHP 做个计划任务，30分钟主动连接一下SSH，目前稳定，不重置不关机！
1.最直接的方法。让你的电脑一直连着Cloud Shell 就可以。
2.可以利用软路由，或者其他的VPS，去连接远程的Cloud Shell，定时任务10分钟一次。
3.也可以利用网站也就是php去远程连接cloud shell ，为了保证可用，也是定时任务10分钟一次即可。
4.当然你不会写程序，也可以借助宝塔面板，添加计划任务！


# 翻墙
目前还没有 好方法，但是可以用ssh隧道代理
