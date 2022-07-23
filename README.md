<div align="center">

# Musicn

🎵 一个下载音乐的命令行工具

![](https://miqilin-blog.oss-cn-shenzhen.aliyuncs.com/musicn-demo.gif)

</div>

## 全局安装

```bash
$ npm i musicn -g
```

## 使用

```bash
$ musicn 陈奕迅
# or
$ msc 陈奕迅
```

搜索的页码数(默认是第1页):

```bash
$ msc 陈奕迅 --number 2
# or
$ msc 陈奕迅 -n 2
# or
$ msc -n 2 陈奕迅
```

咪咕服务下载(默认是网易云的服务):

```bash
$ msc 陈奕迅 --service migu
# or
$ msc 陈奕迅 -s migu
# or
$ msc -s migu 陈奕迅
```

附带歌词下载(默认是不附带):

```bash
$ msc 陈奕迅 --lyric
# or
$ msc 陈奕迅 -l
# or
$ msc -l 陈奕迅
```

自定义下载路径(默认是当前路径):

```bash
$ msc 陈奕迅 --path ../music
# or
$ msc 陈奕迅 -p ../music
# or
$ msc -p ../music 陈奕迅
```

帮助信息:

```bash
$ msc --help
# or
$ msc -h
```

版本信息:

```bash
$ msc --version
# or
$ msc -V
```

## 资源

- 音乐来源: 咪咕和网易云（API 是从公开的网络中获得）

## 说明

1. 暂时只支持网易云和咪咕的服务（因一些特殊原因，腾讯旗下的平台都是不支持的，之前支持的咪咕无损音乐下载因为接口的改变也不支持了，现在暂时都只支持格式：mp3，后期会继续探索其余平台可用的无损音乐下载）
2. 在 `windows` 桌面端的 `git Bash` 中不支持上下切换选歌，问题是 `inquirer` 不兼容，建议使用其它终端工具
3. node version > 14
