
# PRINTRUN
# PRINTRUN

![License](https://img.shields.io/github/license/kliment/Printrun)
![GitHub - Downloads](https://img.shields.io/github/downloads/kliment/Printrun/total?logo=github)
![GitHub contributors](https://img.shields.io/github/contributors/kliment/Printrun?logo=github)
![PyPI - Version](https://img.shields.io/pypi/v/Printrun?logo=pypi&label=PyPI)
![PyPI - Downloads](https://img.shields.io/pypi/dm/Printrun?logo=pypi)

Printrun consists of a suite of hosts for 3D printers and other CNC machines (printcore, pronsole and pronterface) and a small collection of helpful scripts.

Printrun 包含了一套用于 3D 打印机和其他 CNC 机器的主机程序（printcore、pronsole 和 pronterface）以及一小部分有用的脚本。

* **printcore.py** is a library that makes writing [RepRap][1] hosts easy
* **pronsole.py** is an interactive command-line host with tab-completion goodness
* **pronterface.py** is a graphical host with the same functionality as pronsole

* **printcore.py** 是一个使编写 [RepRap][1] 主机程序变得容易的库
* **pronsole.py** 是一个具有自动补全功能的交互式命令行主机
* **pronterface.py** 是一个与 pronsole 具有相同功能的图形界面主机

The contents of this document are organized in the following sections:

本文档的内容分为以下几个部分：

- [Getting Printrun](#getting-printrun)
  * [Distributed Binaries and Packages](#distributed-binaries-and-packages)
    + [Windows and macOS pre-compiled binaries](#windows-and-macos-pre-compiled-binaries)
    + [Linux packages from official repositories](#linux-packages-from-official-repositories)
    + [Printrun package from PyPI](#printrun-package-from-pypi)
  * [Running From Source](#running-from-source)

- [Using Printrun](#using-printrun)
  * [Using Pronterface](#using-pronterface)
  * [Using Pronsole](#using-pronsole)
  * [Using Printcore](#using-printcore)
  * [Platers](#platers)
  * [3D Viewer Controls](#3d-viewer-controls)
  * [RPC Server](#rpc-server)
  * [Configuration](#configuration)
  * [Using Macros And Custom Buttons](#using-macros-and-custom-buttons)
  * [Using Host Commands](#using-host-commands)

- [Testing](#testing)
- [Contributing](#contributing)
- [Contributors](#contributors)
- [License](#license)

本文档的内容分为以下几个部分：

- [获取 Printrun](#getting-printrun)
  * [分发的二进制文件和包](#distributed-binaries-and-packages)
    + [Windows 和 macOS 预编译二进制文件](#windows-and-macos-pre-compiled-binaries)
    + [来自官方仓库的 Linux 包](#linux-packages-from-official-repositories)
    + [来自 PyPI 的 Printrun 包](#printrun-package-from-pypi)
  * [从源码运行](#running-from-source)

- [使用 Printrun](#using-printrun)
  * [使用 Pronterface](#using-pronterface)
  * [使用 Pronsole](#using-pronsole)
  * [使用 Printcore](#using-printcore)
  * [Platers](#platers)
  * [3D 查看器控件](#3d-viewer-controls)
  * [RPC 服务器](#rpc-server)
  * [配置](#configuration)
  * [使用宏和自定义按钮](#using-macros-and-custom-buttons)
  * [使用主机命令](#using-host-commands)

- [测试](#testing)
- [贡献](#contributing)
- [贡献者](#contributors)
- [许可证](#license)

[1]: https://en.wikipedia.org/wiki/RepRap
