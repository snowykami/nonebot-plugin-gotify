<div align="center">
  <img src="https://cdn.liteyuki.icu/static/img/liteyuki_icon_640.png" width="180" height="180" alt="NoneBotPluginLogo">

</div>

<div align="center">

# nonebot-plugin-gotify

_✨ 将NoneBot的通知和讯息推送到个人通知管理器 ✨_

_✨ Push NoneBot's notifications and messages to personal notification manager ✨_


<a href="./LICENSE">
    <img src="https://img.shields.io/github/license/snowykami/nonebot-plugin-gotify.svg" alt="license">
</a>
<a href="https://pypi.python.org/pypi/nonebot-plugin-gotify">
    <img src="https://img.shields.io/pypi/v/nonebot-plugin-gotify.svg" alt="pypi">
</a>
<img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">

</div>

## 📖 介绍 Introduction

将Bot生命周期，聊天讯息实时推送到Gotify，实现个人通知管理器

Push Bot lifecycle and chat messages to Gotify in real time, and achieve personal notification manager

## 💿 安装 Installation

<details open>
<summary>使用 nb-cli 安装(推荐，需先安装`nb-cli`)  Use nb-cli</summary>

    nb plugin install nonebot-plugin-liteyukibot

</details>

<details open>
<summary>使用 pip 安装 Use pip</summary>

    pip install nonebot-plugin-liteyukibot

</details>

<details>
<summary>使用包管理器安装 Use other package manager</summary>
在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令

<details>
<summary>pip</summary>

    pip install nonebot-plugin-liteyukibot

</details>
<details>
<summary>pdm</summary>

    pdm add nonebot-plugin-liteyukibot

</details>
<details>
<summary>poetry</summary>

    poetry add nonebot-plugin-liteyukibot

</details>
<details>
<summary>conda</summary>

    conda install nonebot-plugin-liteyukibot

</details>
</details>

轻雪机器人已内置该插件，无需单独安装

LiteyukiBot has built-in this plugin, no need to install separately

## 🎉 使用 Usage

本插件暂时没有和用户交互的部分

This plugin does not have an interactive part with the user for the time being

## ⚙️ 配置 Configuration

```python
# 必要字段 Required
GOTIFY_URL = "http://your-gotify-server:port"
GOTIFY_TOKEN = "your-gotify-token"
# 可选字段 Optional with default value
GOTIFY_PRIORITY = 5
GOTIFY_NICKNAME = "NoneBot" # 推送系统消息的昵称 Nickname for system messages
GOTIFY_TITLE = "{message_type}: {nickname}({user_id})" # 推送系统消息的标题模板 Title for system messages template
GOTIFY_MESSAGE = "{message}" # 推送系统消息的内容模板 Content for system messages template
GOTIFY_INCLUDES = ["message", "notice"] # 包含的消息类型 Includes message types
```

## ℹ️ 其他 Other

- 目前该插件已内置在[轻雪机器人应用](https://bot.liteyuki.icu)中，无需单独安装.
The plugin has been built into the [LiteyukiBot application](https://bot.liteyuki.icu), no need to install separately

- 该插件仍然有许多内容需要完善，欢迎各位的建议及贡献.
There are still many things to be improved in this plugin, welcome your suggestions and contributions