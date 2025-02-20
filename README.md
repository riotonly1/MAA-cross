<!-- markdownlint-disable MD033 MD041 -->
<p align="center">
  <img alt="LOGO" src="https://cdn.jsdelivr.net/gh/MaaAssistantArknights/design@main/logo/maa-logo_512x512.png" width="256" height="256" />
</p>

<div align="center">

# MaaPracticeBoilerplate

</div>

本仓库为 [MaaFramework](https://github.com/MaaXYZ/MaaFramework) 所提供的项目模板，正在尝试构建 自用的交错战线收菜助手。

> **MaaFramework** 是基于图像识别技术、运用 [MAA](https://github.com/MaaAssistantArknights/MaaAssistantArknights) 开发经验去芜存菁、完全重写的新一代自动化黑盒测试框架。
> 低代码的同时仍拥有高扩展性，旨在打造一款丰富、领先、且实用的开源库，助力开发者轻松编写出更好的黑盒测试程序，并推广普及。

## 即刻开始      

- [📄 快速开始](https://github.com/MaaXYZ/MaaFramework/blob/main/docs/zh_cn/1.1-%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B.md)
- [🎞️ 视频教程](https://www.bilibili.com/video/BV1yr421E7MW)
  
## 补充部分教程-需求的软件及下载链接
1.请先行下载并安装如下软件

-VSCode 用来打开并编写json，官网链接：https://code.visualstudio.com/Download

-python 基础支持，官网链接：https://www.python.org/downloads/

-Git Bash 命令行工具，官网链接：https://git-scm.com/downloads/win

## 如何开发
补充：

1.先使用并打开cmd（win+r   输入cmd），然后按下列格式输入

git config --global user.name "Your Name"

git config --global user.email "email@***.com"

Your Nam 和 email@***.com 设置为你的用户名和邮箱
   
2.在你愿意存放项目的地址，新建一个文件夹，然后有右键点击，并选择Open Git Bash here

下面相关内容均在打开的界面进行输入（若首次本地安装MaaDebugger 地址：https://github.com/MaaXYZ/MaaDebugger 失败，可多尝试几次）

相关内容请前往 

MaaFramework 地址：https://github.com/MaaXYZ/MaaFramework 

和MaaFramework项目模板 地址：https://github.com/MaaXYZ/MaaPracticeBoilerplate 查看

3.相关json的编写请打开***\assets\resource\pipeline下的json进行编写

MaaDebugger  load失败，请检查json是否存在编写错误，打开的Git Bash窗口也会提示内容

4.相关照片请存放于***\assets\resource\image文件夹内

5.推荐使用MFATools进行截图，区域选择，坐标查看，滑动坐标的选择和查看

6.MaaDebugger本地使用代码

请使用Git Bash窗口运行如下命令

python -m MaaDebugger



**摸鱼进度：（均存在各种各样的神奇问题和bug）**

1.启动游戏并登录至主界面

请先自行登录一次游戏

建议关闭待机模式

2.基地收菜

请勿使用俯视角(未适配)

包含功能：驻员换班（红了才会进去，需设置好预设队伍）

点击矿场收菜

交易所（目前包含购买蓝图和自动合成白方块）

完成交易所任务后会直接返回主页，并停止。

3.补给站

购买免费礼包

限时贸易所购买折扣商品（慎用，所有折扣的物品都会购买，请保证自己货币充足，因为没写缺钱的情况）


    

## 鸣谢

本项目由 **[MaaFramework](https://github.com/MaaXYZ/MaaFramework)** 强力驱动！

感谢以下开发者对本项目作出的贡献（下面链接改成你自己的项目地址）:

[![Contributors](https://contrib.rocks/image?repo=MaaXYZ/MaaFramework&max=1000)](https://github.com/MaaXYZ/MaaFramework/graphs/contributors)
