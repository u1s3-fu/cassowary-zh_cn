<p align="center">
  <img src="app-linux/src/cassowary/gui/extrares/cassowary.svg" alt="Logo" width="200" align="center"/> <p style="color:blue;font-size:64px;">
</p>

# Cassowary

[![Visits Badge](https://badges.pufler.dev/visits/u1s3-fu/cassowary)](https://github.com/casualsnek)

![App Demo GIF](docs/img/app-preview.gif)

使用Cassowary，您可以在Linux上运行Windows虚拟机并使用Windows应用程序，就像是基于FreeRDP和远程应用程序技术构建的本地应用程序一样。

**如果您喜欢视频而不是文档可以参考连接  [点击跳转 YouTube](https://www.youtube.com/watch?v=ftq-c_VgmK0)**

如果项目有对您提供的了帮助可以点击 ⭐ 

**加入Discord的讨论: [点击连接加入 Discord](https://discord.gg/hz4mAwSujH)**

**本项目根据原项目进行简单汉化 [点击跳转至原项目](https://github.com/casualsnek/cassowary/) **

## Cassowary 支持:

- 将Windows应用程序当作本机应用程序运行
- 直接在Windows应用程序中从Linux主机打开文件
- 使用Linux应用程序打开Windows虚拟机上的文件
- 允许在虚拟机和主机文件系统之间轻松访问
- 一个易于使用的配置实用程序
- 为Windows应用程序创建应用程序启动器
- 在没有使用Windows应用程序时自动挂起虚拟机，并在需要时自动恢复（仅限virt-manager）

## 描述文件包括一下内容

1. [使用virt-manager设置Windows虚拟机](docs/1-virt-manager.md)
2. [在Windows虚拟机和Linux主机上安装Cassowary](docs/2-cassowary-install.md)
3. [额外的操作方法和常见问题解答](docs/3-faq.md)
* 从源代码构建Cassowary
* 你可以帮助我什么?

<br>

## 从源代码构建Cassowary

只有当您不想使用 [releases](https://github.com/casualsnek/cassowary/releases) 才需要执行此步骤 需要自己构建`.zip` 和 `.whl` 文件!

#### 构建Linux程序 (在linux上)

```bash
git clone https://github.com/casualsnek/cassowary
cd cassowary/app-linux
chmod +x build.sh
./build.sh
```

这将创建一个名为 `dist`目录在 `app-linux` 中包含可安装的文件 `.whl`  文件

#### 构建Windows程序 ( 在Windows上 )

下载并安装 [Python3](https://python.org) (在Windows7 使用 Python 3.7) 和 [Git](https://git-scm.com) 然后在Windows系统上面运行以下命令来构建对应的应用:

```bash
git clone https://github.com/casualsnek/cassowary
cd cassowary\app-win
.\build.bat
```

这将创建一个名为 `bin` 的文件夹，其中包含安装文件。 

#### 在Linux上构建Windows和Linux应用程序

首先安装 [wine](https://wiki.winehq.org/Download) , 以便于在Linux上构建Windows应用程序，需要互联网才可以下载Python二进制文件进行安装

注意，通过wine构建的Windows应用程序可能无法在某些Windows系统上正常运行。

```bash
git clone https://github.com/casualsnek/cassowary
cd cassowary
chmod +x buildall.sh
./buildall.sh
```

这将创建一个名为 `dist` 的文件夹在 `app-linux` 中，其中包含可以安装的文件。  
还有一个 `bin`文件夹在 `app-win` 中，其中包含Windows的安装文件。

<br>

## 你可以对我提供什么帮助?

- 改进 README.md 及其其他文档
- 报告错误或提交修补程序
- 建议新功能或对现有功能的改进！
- 在 [OpenCollective](https://opencollective.com/cassowary)支持此项目

---

### 赞助商
[![Sponsors](https://opencollective.com/cassowary/tiers/sponsor.svg?avatarHeight=36&width=600)](https://opencollective.com/cassowary)

### 个人支持
[![Backers](https://opencollective.com/cassowary/tiers/backer.svg?avatarHeight=36&width=600)](https://opencollective.com/cassowary)
