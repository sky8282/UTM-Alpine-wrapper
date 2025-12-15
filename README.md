# UTM-Alpine-wrapper
## 基于 UTM (ARM)虚拟机的 Alpine3.20 系统镜像,自带 wrapper 与管理器
* **UTM项目**：https://github.com/utmapp/UTM  (镜像使用4.7.4 版本生成)
* **wrapper项目**：https://github.com/zhaarey/wrapper  或 https://github.com/WorldObservationLog/wrapper
* **wrapper管理器v1版**：https://github.com/sky8282/wrapper-manager-v1
* **apple-music-downloader 原版**：https://github.com/zhaarey/apple-music-downloader
* **apple-music-downloader 多线程多区域版本分支**：https://github.com/sky8282/apple-music-downloader

## 🚀 MacOS 安装 Go 下载器所需依赖:
```text
# 安装 MP4Box
brew install gpac
# 验证安装
MP4Box -version

# 安装 mp4decrypt
brew install bento4
# 验证安装
mp4decrypt
—————————————————————————————————————————————
如提示未装或者需要升级 Go 版本，请自行问 ai 操作步骤
—————————————————————————————————————————————
```
## ✨ 首次开机自动启动 wrapper 管理器，如未启动请执行:
```text
# 前台启动：
cd /root/wrapper && ./wrapper-manager

# 后台启动：
cd /root/wrapper && nohup ./wrapper-manager > /dev/null 2>&1 &

# 停止后台运行：
pkill -f wrapper-manager && pkill -9 -f wrapper && ps aux | grep wrapper
```
## 🛠️ 建议在 MacOS 本体上进行 Go 下载
* 如真的需要在虚拟机里下载的话，请自行安装 Go 程序
* MP4Box / mp4decrypt 已经编译，请执行安装:
```text
cd /root/MP4Box-mp4decrypt-Alpine && ./install.sh
```
## 🛠️ 加载 UTM 镜像文件步骤：
* 新建虚拟机
* 打开解压好的压缩包
* 使用 ssh 工具如 finalshell 链接 192.168.64.16:22
* 账号 root 密码 root

![1](https://github.com/user-attachments/assets/c1ab5d7d-d787-41a8-811c-c7954f816cd8)


![2](https://github.com/user-attachments/assets/08a74e44-363f-450f-b571-599ad0b2e808)


