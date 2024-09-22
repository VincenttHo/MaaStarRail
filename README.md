# MaaStarRail

基于[MaaFramework](https://github.com/MaaXYZ/MaaFramework)实现的 崩坏星穹铁道 小助手。图像技术 + 模拟控制，解放双手！  
由 [MaaFramework](https://github.com/MaaXYZ/MaaFramework) 强力驱动！

## 功能介绍

目前已有的功能：

- 登录游戏
- 刷体力
- 委托
- 领取日常奖励

## 使用说明

下载地址：<https://github.com/VincenttHo/MaaStarRail/releases>

### Windows

- 请下载 `MaaStarRail-win-x86_64-vXXX.zip`
- 解压后运行 `MaaPiCli.exe` 即可

## 其他说明

- 提示“应用程序错误”，一般是缺少运行库，请安装一下 [vc_redist](https://aka.ms/vs/17/release/vc_redist.x64.exe)
- 添加 `-d` 参数可跳过交互直接运行任务，如 `./MaaPiCli.exe -d`
- 2.0 版本已支持 mumu 后台保活，会在 run task 时获取 mumu 最前台的 tab，并始终使用这个 tab（即使之后被切到后台了）
- 反馈问题请附上日志文件 `debug/maa.log`，谢谢！

## 图形化界面

目前暂无正式版 GUI。

## How to build

**如果你要编译源码才看这节，否则直接 [下载](https://github.com/VincenttHo/MaaStarRail/releases) 即可**

0. 完整克隆本项目及子项目

    ```bash
    git clone --recursive https://github.com/VincenttHo/MaaStarRail.git
    ```

1. 下载 MaaFramework 的 [Release 包](https://github.com/MaaXYZ/MaaFramework/releases)，解压到 `deps` 文件夹中
2. 安装

    ```python
    python ./install.py
    ```

生成的二进制及相关资源文件在 `install` 目录下

## 开发相关

- [MaaFW 开发思路](https://github.com/MaaXYZ/MaaFramework/blob/main/docs/zh_cn/0.1-%E5%BC%80%E5%8F%91%E6%80%9D%E8%B7%AF.md)  
  MaaStarRail 目前使用其中第一种方式（纯 Pipeline 低代码），后续可能会迁移到第二种方式（Pipeline + 自定义任务）
- [Pipeline 流水线协议](https://github.com/MaaXYZ/MaaFramework/blob/main/docs/zh_cn/3.1-%E4%BB%BB%E5%8A%A1%E6%B5%81%E6%B0%B4%E7%BA%BF%E5%8D%8F%E8%AE%AE.md)

更多文档请前往 [MaaFramework](https://github.com/MaaXYZ/MaaFramework) 主仓库查看