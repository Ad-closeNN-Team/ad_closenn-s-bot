![GitHub Issues or Pull Requests](https://img.shields.io/github/issues/Ad-closeNN-Team/ad_closenn-s-bot)
![GitHub Issues or Pull Requests](https://img.shields.io/github/issues-pr/Ad-closeNN-Team/ad_closenn-s-bot)
![GitHub Release](https://img.shields.io/github/v/release/Ad-closeNN-Team/ad_closenn-s-bot)

![GitHub last commit (branch)](https://img.shields.io/github/last-commit/Ad-closeNN-Team/ad_closenn-s-bot/main?label=main%20last%20commit)
![GitHub last commit (branch)](https://img.shields.io/github/last-commit/Ad-closeNN-Team/ad_closenn-s-bot/beta?label=beta%20last%20commit)

# 如何使用
> [!IMPORTANT]
> 使用之前请确保你的网络环境可以连接到 Discord 的服务！本地开发的且使用代理的如果能打开Tun模式最好要打开！

> [!CAUTION]
> 填写API的时候请勿使用本repo自带的API，请去申请一个API填入（包括Discord机器人的Token、SparkAI的API key。如果只是临时想用的话可以“借用”一下SparkAI的API Key（Discord机器人的Token不能借，毕竟[申请个机器人](https://www.freecodecamp.org/chinese/news/create-a-discord-bot-with-python)也没什么难的吧？），如果“借”的多的话，请考虑自己申请API key

## 本地开发

| 依赖库 | Python 版本  |
|-------|------
| spark_ai_python | 3.8+ |  
| discord.py   | *3.10+ |  
| sparkdesk-api | *3.10+ |

*未经准确测试，GitHub Codespaces提供的Python版本为`3.10.13`(2024/8/7记录)

[讯飞星火官方开发文档](https://www.xfyun.cn/doc/spark/Web.html)  | 
[非官方星火api开发文档](https://github.com/HildaM/sparkdesk-api)
### 下载
有两种方法：
- 点击右边 Relases 的 最新版本(标有latest的)，往下找，找到 Assets ，在列表选择合适自己的操作系统的 Source code（Windows用户建议优选选择zip版本），将其下载到本地，然后解压这个文件。在这个解压后的文件夹里，打开终端（命令提示符）

- 点击上方的 Code, 如果列表为 Codespaces ，请切换到 Local 列表，点击 `Download ZIP` 将源代码下载下来。下载完后，解压这个文件。
---
### 安装
解压完成后，你需要进入到全是文件的文件夹里面，此时目录树应为如下所示：
```
ad_closenn-s-bot-main
        .env
        main.py
        README.md
        requirements.txt
```
**一切就绪后：**
### Windows 用户请依次输入：
```bash
python -m pip install --upgrade pip
```
```bash
pip install -r requirements.txt
```
```bash
python main.py
```
### Linux 用户请依次输入：
```bash
python3 -m pip install --upgrade
```
```bash
pip3 install -r requirements.txt
```
```bash
python3 main.py
```
---
## 网上开发
### 安装
- 如果是临时想看看代码能不能跑得起来，那么可以fork本项目，然后在自己fork后的页面点击 Code ，然后切换到 Codespaces ，添加一个新的Codespace，按照[上面](#安装)描述的安装方法进行安装即可。

- 如果你是有自己的云主机什么的（要能运行Python和连接到[互联网]），那么建议使用云主机，GitHub Codespaces不能持续运行代码（bug不说），需要自己的云服务器。