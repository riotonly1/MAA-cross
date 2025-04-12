<!-- markdownlint-disable MD033 MD041 -->
<p align="center">
  <img alt="LOGO" src="https://cdn.jsdelivr.net/gh/MaaAssistantArknights/design@main/logo/maa-logo_512x512.png" width="256" height="256" />
</p>

<div align="center">

# MaaPracticeBoilerplate

</div>

本仓库为 [MaaFramework](https://github.com/MaaXYZ/MaaFramework) 所提供的项目模板，开发者可基于此模板直接创建自己的 MaaXXX 项目。

> **MaaFramework** 是基于图像识别技术、运用 [MAA](https://github.com/MaaAssistantArknights/MaaAssistantArknights) 开发经验去芜存菁、完全重写的新一代自动化黑盒测试框架。
> 低代码的同时仍拥有高扩展性，旨在打造一款丰富、领先、且实用的开源库，助力开发者轻松编写出更好的黑盒测试程序，并推广普及。

## 功能介绍（自用摆烂板）
注意事项

使用MFA任务管理器时若任务列表无任务，请手动点击+号图标添加任务

仅在雷电模拟器上进行过测试，本人使用时未发现严重bug

本人为代码小白，未防止避免误点击造成损失，请诸位使用时，最好看着屏幕运行

本人雷电模拟器，分辨率为：平板版 1920*1080（dpi 280），少部分功能为识色，可能存在不准确的情况。

1.启动app并登录至主界面

2.基建收菜
 
    包含内容
    1. 矿场收菜

    2. 更换干员
    更换疲惫干员，请先设置好预设1和预设2

    由于游戏特性，干员不在设施中便可自动恢复心情，所以未写更换干员宿舍人员内容

    3.订单
    浏览并交易蓝图，无蓝图材料会自行合成，请确保自己材料充足

    均设置了开关，

    好友界面向左滑动功能：在订单界面选择好友时，向左滑动几次，确保从第一个好友开始浏览，如果没有手动向右滑动选择好友，建议不开。

3.免费礼包+限时贸易所购买折扣物品
  
   根据建议，设置了不同的开关

   购买所有折扣物品（默认关闭 ）：会购买所有打折物品，包括芯片、材料等

   剩余材料开关，打开则会购买对应的材料（无论是否打折），关闭则不购买
   材料清单在完善中，目前只有少数材料（未来补充）

4.模拟军演
   请先设置好自己的整容

   增加战力刷新选择（大于对应战力则会刷新），只会对第一个对手进行识别。

5.周本（第一关）
   只会使用队伍1，请先编好队伍后进入周本一次。

   顺便刷刷好感度，建议一两个高练度角色带一群低好感角色。

6.每日探索
除芯片关卡外均已支持，默认扫荡不使用燃料的最高次数（判定过程可能较慢），

开启手动选择后，也讲开启燃料使用，下方手动次数才会生效。


7.日常任务领取和通行证领取

仅领取日常，周常需自行领取，建议周末再领，
通行证仅领取任务，请自行领取通行证奖励

8.活动（云端行迹 困难第八关 扫荡）

## 小白从零开始补充内容
请先下载
[Git bash]（https://gitforwindows.org/?spm=a2c6h.12873639.article-detail.4.75dd4775UWa3Ar）               
基础支持

安装之后，先在你想存放项目的地点新建文件夹，后右键点击文件夹并点击 Open Git Bash here 后续克隆，启用MAAdebager等均在代开的窗口进行

MaaDebugger调试json文件，加载失败时，可在打开的窗口查看红色内容，确认报错内容

[vs code](https://code.visualstudio.com/)
编写json

[MFATools](https://github.com/SweetSmellFox/MFATools)
裁剪图片、获取区间、确定点击坐标、获取颜色的upper和lower等功能

python
基础需要

## 即刻开始

- [📄 快速开始](https://github.com/MaaXYZ/MaaFramework/blob/main/docs/zh_cn/1.1-%E5%BF%AB%E9%80%9F%E5%BC%80%E5%A7%8B.md)
- [🎞️ 视频教程](https://www.bilibili.com/video/BV1yr421E7MW)


## 如何开发

0. 使用右上角 `Use this template` - `Create a new repository` 来基于本模板创建您自己的项目。

1. 完整克隆本项目及子项目

    ```bash
    git clone --recursive https://github.com/riotonly1/MAA-cross
    ```

    **请注意，一定要完整克隆子项目，不要漏了 `--recursive`，也不要下载 zip 包！**  
    这步未正确操作会导致所有 OCR（文字识别）失败！

2. 下载 MaaFramework 的 [Release 包](https://github.com/MaaXYZ/MaaFramework/releases)，解压到 `deps` 文件夹中。

3. 配置资源文件。

    ```bash
    python ./configure.py
    ```

4. 按需求修改 `assets` 中的资源文件，请参考 MaaFramework 相关文档。

    - 可使用 [MaaDebugger](https://github.com/MaaXYZ/MaaDebugger) 进行调试；
    - 也可以在本地安装后测试： python -m MaaDebugger

        1. 执行安装脚本

            ```bash
            python ./install.py
            ```

        2. 执行`MaaPiCli`

            - **Windows**

                运行 `install/MaaPiCli.exe`

            - **Linux/macOS**

                > 如果提示缺少启动权限，可通过 `chmod a+x install/MaaPiCli` 命令添加

                运行 `install/MaaPiCli`

5. 完成开发工作后，上传您的代码并发布版本。

    ```bash
    # 配置 git 信息（仅第一次需要，后续不用再配置）
    git config user.name "您的 GitHub 昵称"
    git config user.email "您的 GitHub 邮箱"
    
    # 提交修改
    git add .
    git commit -m "XX 新功能"
    git push origin HEAD -u
    ```

6. 发布您的版本

    需要**先**修改仓库设置 `Settings` - `Actions` - `General` - `Read and write permissions` - `Save`

    ```bash
    # CI 检测到 tag 会自动进行发版
    git tag v1.0.0
    git push origin v1.0.0
    ```

7. 更多操作，请参考[个性化配置](./docs/zh_cn/个性化配置.md)（可选）




## 鸣谢

本项目由 **[MaaFramework](https://github.com/MaaXYZ/MaaFramework)** 强力驱动！

感谢以下开发者对本项目作出的贡献（下面链接改成你自己的项目地址）:

[![Contributors](https://contrib.rocks/image?repo=MaaXYZ/MaaFramework&max=1000)](https://github.com/MaaXYZ/MaaFramework/graphs/contributors)
