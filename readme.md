# txthinking/brook [![translate-svg]][translate-list]

[translate-svg]: http://llever.com/translate.svg
[translate-list]: https://github.com/chinanf-boy/chinese-translate-list

「 Linux / MacOS / Windows 上的 VPN，也许你可以将它用于游戏」

[中文](./readme.md) | [english](https://github.com/txthinking/brook)

---

## 校对 🀄️

<!-- doc-templite START generated -->
<!-- repo = 'txthinking/brook' -->
<!-- commit = 'b6c9fbfe90f9c4132b78f4b7913db8d4566ab1f4' -->
<!-- time = '2018-09-04' -->

| 翻译的原文 | 与日期        | 最新更新 | 更多                       |
| ---------- | ------------- | -------- | -------------------------- |
| [commit]   | ⏰ 2018-09-04 | ![last]  | [中文翻译][translate-list] |

[last]: https://img.shields.io/github/last-commit/txthinking/brook.svg
[commit]: https://github.com/txthinking/brook/tree/b6c9fbfe90f9c4132b78f4b7913db8d4566ab1f4

<!-- doc-templite END generated -->

- [x] readme
- [ ] [wiki](https://github.com/chinanf-boy/brook-zh/wiki)

### 贡献

欢迎 👏 勘误/校对/更新贡献 😊 [具体贡献请看](https://github.com/chinanf-boy/chinese-translate-list#贡献)

## 生活

[help me live , live need money 💰](https://github.com/chinanf-boy/live-need-money)

---

# brook

[![Build Status](https://travis-ci.org/txthinking/brook.svg?branch=master)](https://travis-ci.org/txthinking/brook) [![Go Report Card](https://goreportcard.com/badge/github.com/txthinking/brook)](https://goreportcard.com/report/github.com/txthinking/brook) [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0) [![Wiki](https://img.shields.io/badge/docs-wiki-blue.svg)](https://github.com/chinanf-boy/brook-zh/wiki)

<p align="center">
    <img style="float: right;" src="https://storage.googleapis.com/txthinking-file/_/brook_200x200.png" alt="Brook"/>
</p>

---

### v20180909

- Linux / MacOS / Windows 上的 VPN,也许你可以将它用于游戏，[维基](https://github.com/chinanf-boy/brook-zh/wiki/How-to-run-VPN-on-Linux,-MacOS-and-Windows%3F)

---

### 目录

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [什么是 brook](#%E4%BB%80%E4%B9%88%E6%98%AF-brook)
- [下载](#%E4%B8%8B%E8%BD%BD)
- [包获取](#%E5%8C%85%E8%8E%B7%E5%8F%96)
  - [Arch Linux](#arch-linux)
  - [MacOS (GUI)](#macos-gui)
- [brook](#brook)
  - [服务器](#%E6%9C%8D%E5%8A%A1%E5%99%A8)
  - [客户端(CLI)](#%E5%AE%A2%E6%88%B7%E7%AB%AFcli)
  - [客户端(GUI)](#%E5%AE%A2%E6%88%B7%E7%AB%AFgui)
    - [隧道](#%E9%9A%A7%E9%81%93)
    - [Tproxy(通常在 Linux 路由器盒上使用)](#tproxy%E9%80%9A%E5%B8%B8%E5%9C%A8-linux-%E8%B7%AF%E7%94%B1%E5%99%A8%E7%9B%92%E4%B8%8A%E4%BD%BF%E7%94%A8)
    - [VPN](#vpn)
    - [relay](#relay)
    - [Socks5](#socks5)
    - [Socks5 到 HTTP](#socks5-%E5%88%B0-http)
    - [2.6.8](#268)
- [贡献](#%E8%B4%A1%E7%8C%AE)
- [执照](#%E6%89%A7%E7%85%A7)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## 什么是 brook

Brook 是一个跨平台的 proxy/VPN 软件.<br/>brook 的目标是保持简单,傻瓜式和潜藏.

## 下载

| 下载                                                                                                               | 服务器/客户端  | OS         | Arch 架构 | 备注 |
| ------------------------------------------------------------------------------------------------------------------ | -------------- | ---------- | --------- | ---- |
| [brook](https://github.com/txthinking/brook/releases/download/v20180909/brook)                                     | 服务器和客户端 | Linux      | amd64     | CLI  |
| [brook_linux_386](https://github.com/txthinking/brook/releases/download/v20180909/brook_linux_386)                 | 服务器和客户端 | Linux      | 386       | CLI  |
| [brook_linux_arm64](https://github.com/txthinking/brook/releases/download/v20180909/brook_linux_arm64)             | 服务器和客户端 | Linux      | arm64     | CLI  |
| [brook_linux_arm5](https://github.com/txthinking/brook/releases/download/v20180909/brook_linux_arm5)               | 服务器和客户端 | Linux      | arm5      | CLI  |
| [brook_linux_arm6](https://github.com/txthinking/brook/releases/download/v20180909/brook_linux_arm6)               | 服务器和客户端 | Linux      | arm6      | CLI  |
| [brook_linux_arm7](https://github.com/txthinking/brook/releases/download/v20180909/brook_linux_arm7)               | 服务器和客户端 | Linux      | arm7      | CLI  |
| [brook_linux_mips](https://github.com/txthinking/brook/releases/download/v20180909/brook_linux_mips)               | 服务器和客户端 | Linux      | mips      | CLI  |
| [brook_linux_mipsle](https://github.com/txthinking/brook/releases/download/v20180909/brook_linux_mipsle)           | 服务器和客户端 | Linux      | mipsle    | CLI  |
| [brook_linux_mips64](https://github.com/txthinking/brook/releases/download/v20180909/brook_linux_mips64)           | 服务器和客户端 | Linux      | mips64    | CLI  |
| [brook_linux_mips64le](https://github.com/txthinking/brook/releases/download/v20180909/brook_linux_mips64le)       | 服务器和客户端 | Linux      | mips64le  | CLI  |
| [brook_linux_ppc64](https://github.com/txthinking/brook/releases/download/v20180909/brook_linux_ppc64)             | 服务器和客户端 | Linux      | ppc64     | CLI  |
| [brook_linux_ppc64le](https://github.com/txthinking/brook/releases/download/v20180909/brook_linux_ppc64le)         | 服务器和客户端 | Linux      | ppc64le   | CLI  |
| [brook_darwin_amd64](https://github.com/txthinking/brook/releases/download/v20180909/brook_darwin_amd64)           | 服务器和客户端 | MacOS      | amd64     | CLI  |
| [brook_windows_amd64.exe](https://github.com/txthinking/brook/releases/download/v20180909/brook_windows_amd64.exe) | 服务器和客户端 | Window     | amd64     | CLI  |
| [brook_windows_386.exe](https://github.com/txthinking/brook/releases/download/v20180909/brook_windows_386.exe)     | 服务器和客户端 | Window     | 386       | CLI  |
| [Brook.dmg](https://github.com/txthinking/brook/releases/download/v20180909/Brook.dmg)                             | 客户端         | MacOS      | amd64     | GUI  |
| [Brook.Setup.exe](https://github.com/txthinking/brook/releases/download/v20180909/Brook.Setup.exe)                 | 客户端         | Window     | amd64     | GUI  |
| [应用商店](https://itunes.apple.com/us/app/brook-brook-shadowsocks-vpn-proxy/id1216002642)                         | 客户端         | iOS 版     | -         | GUI  |
| [Brook.apk](https://github.com/txthinking/brook/releases/download/v20180909/Brook.apk)(没有 Google Play)           | 客户端         | Android 版 | -         | GUI  |

**看[维基](https://github.com/chinanf-boy/brook-zh/wiki)了解更多教程**

## 包获取

### Arch Linux

```
sudo pacman -S brook
```

### MacOS (GUI)

```
brew cask install brook
```

## brook

```
NAME:
   Brook - 跨平台 Proxy/VPN 软件

USAGE:
   brook [global options] command [command options] [arguments...]

VERSION:
   20180909

AUTHOR:
   Cloud <cloud@txthinking.com>

COMMANDS:
     server         以 服务器模式运行
     servers        以 多服务器模式运行
     client         以客户端模式运行
     tunnel         以隧道模式运行
     tproxy         运行为tproxy模式，透明代理，仅适用于Linux
     vpn            以VPN模式运行
     streamserver   以 服务器模式运行
     streamservers  以 多服务器模式运行
     streamclient   以客户端模式运行
     ssserver       以 shadowsocks服务器模式运行，默认方法是aes-256-cfb
     ssservers      以 shadowsocks运行多个服务器模式，默认方法是aes-256-cfb
     ssclient       以 shadowsocks客户端模式运行，默认方法是aes-256-cfb
     socks5         以 原始socks5服务器运行
     relay          以 中继模式运行
     relays         以 多中继器模式运行
     qr             打印brook服务器的二维码
     socks5tohttp   将socks5转换为http代理
     systemproxy    使用 pac url设置系统代理，或删除，仅适用于 MacOS /Windows
     help, h        显示一个命令的命令列表或帮助

GLOBAL OPTIONS:
   --debug, -d               Enable debug
   --listen value, -l value  Listen address for debug (default: ":6060")
   --help, -h                show help
   --version, -v             print the version
```

### 服务器

```
# Run as a brook server
$ brook server -l :9999 -p password
```

```
# Run as multiple brook servers
$ brook servers -l ":9999 password" -l ":8888 password"
```

> 如果您运行公共/共享服务器,请不要忘记此`--tcpDeadline`参数

### 客户端(CLI)

```
# 运行 brook client, 执行 socks5 proxy socks5://127.0.0.1:1080
$ brook client -l 127.0.0.1:1080 -i 127.0.0.1 -s server_address:port -p password
```

```
# 运行 brook client, 启动  http(s) proxy http(s)://127.0.0.1:8080
$ brook client -l 127.0.0.1:8080 -i 127.0.0.1 -s server_address:port -p password --http
```

### 客户端(GUI)

看[维基](https://github.com/chinanf-boy/brook-zh/wiki)

#### 隧道

```
# Run as tunnel 127.0.0.1:5 to 1.2.3.4:5
$ brook tunnel -l 127.0.0.1:5 -t 1.2.3.4:5 -s server_address:port -p password
```

#### Tproxy(通常在 Linux 路由器盒上使用)

看[维基](https://github.com/chinanf-boy/brook-zh/wiki/How-to-run-transparent-proxy-on-Linux%3F)

#### VPN

```
# Run as VPN to proxy all TCP/UDP. [需要 ROOT 权限].
$ sudo brook vpn -l 127.0.0.1:1080 -s server_address:port -p password
```

**看[维基](https://github.com/chinanf-boy/brook-zh/wiki/How-to-run-VPN-on-Linux,-MacOS-and-Windows%3F)了解更多教程**

#### relay

```
# Run as relay to 1.2.3.4:5
$ brook relay -l :5 -r 1.2.3.4:5
```

#### Socks5

```
# Run as a raw socks5 server 1.2.3.4:1080
$ brook socks5 -l :1080 -i 1.2.3.4
```

#### Socks5 到 HTTP

```
# Convert socks5://127.0.0.1:1080 to http(s)://127.0.0.1:8080 proxy
$ brook socks5tohttp -l 127.0.0.1:8080 -s 127.0.0.1:1080
```

#### 2.6.8

```
# Run as a shadowsocks server
$ brook ssserver -l :9999 -p password
```

```
# Run as multiple shadowsocks servers
$ brook ssservers -l ":9999 password" -l ":8888 password"
```

> 如果您运行公共/共享服务器,请不要忘记此`--tcpDeadline`参数

```
# Run as shadowsocks client, start a socks5 proxy socks5://127.0.0.1:1080
$ brook ssclient -l 127.0.0.1:1080 -i 127.0.0.1 -s server_address:port -p password
```

```
# Run as shadowsocks client, start a http(s) proxy http(s)://127.0.0.1:8080
$ brook ssclient -l 127.0.0.1:8080 -i 127.0.0.1 -s server_address:port -p password --http
```

> 默认方法是 aes-256-cfb

**看[维基](https://github.com/chinanf-boy/brook-zh/wiki)了解更多教程**

## 贡献

请阅读[CONTRIBUTING.md](.github/CONTRIBUTING.md)先

## 执照

根据 GPLv3 许可证获得许可
