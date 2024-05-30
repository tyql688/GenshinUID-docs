# 插件开发指南 <Badge type="tip" text="普通" />

::: tip

- 🎉 该文档将从最基础的创建项目结构开始，直至创建一个**能正常使用功能**的GsCore插件。

- 🤗 该文档适用于**任何人**，哪怕*你没有最基本的Python知识*，也能通过该文档进行**学习**。
  - 但是你需要拥有一颗善于学习的心、以及最基本的互联网查找技能

:::

## 0、在开始前

::: info

在编写代码开始前，请先确保你安装了最基本的环境。

注意：以下说的是你的本地开发环境，而非Bot部署环境（服务器）

:::

- 🛠 你已经通过[该文档](/Started/EnvCheck)安装并检查了如下工具：

  - Python 3.8及以上（建议3.11）
  - git
  - poetry/pdm

  

- 🚀 你已经通过[该教程](/Started/InstallCore)安装并成功[运行](/Started/StartCore)本项目，即GsCore正常运行

  

- 🤖 你已经成功运行任何一个Bot端和服务端，并能使用IM软件与你的Bot进行对话

  - Bot端：NoneBot2、HoshinoBot、Koishi、Yunzai、等等.....
  - 协议端：Go-CQHTTP、NapCat、或者某些Bot自带的协议适配器、等等.....
  - IM软件：QQ、QQ频道、Discord、Telegram、KOOK、DODO、微信、等等.....
  - 和Bot对话：发送命令`core状态`，Bot能够正确进行回复

  

- ⌨ 安装任意一个代码编辑器，这里推荐VSC，也就是[Visual Studio Code](https://code.visualstudio.com/)

  - 当然你也可以选择使用PyCharm，但以下内容将以VSC为范例。

  

## 1、明确项目需求

