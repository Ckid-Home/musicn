<div align="center">

# Musicn

🎵 一个下载高品质音乐的命令行工具

![](https://miqilin-blog.oss-cn-shenzhen.aliyuncs.com/musicn-demo.gif)

</div>

## 全局安装

```bash
$ npm install musicn -g
```

## 使用

```bash
$ musicn 晴天
# or
$ msc 晴天
```

网易云服务下载(默认是咪咕的服务):

```bash
$ msc 晴天 --service netease
# or
$ msc 晴天 -s netease
# or
$ msc -s netease 晴天
```

附带歌词下载(默认是不附带):

```bash
$ msc 晴天 --lyric
# or
$ msc 晴天 -l
# or
$ msc -l 晴天
```

指定文件夹路径下载(默认是当前文件夹路径):

```bash
$ msc 晴天 --path ../music
# or
$ msc 晴天 -p ../music
# or
$ msc -p ../music 晴天
```

## 资源

- 音乐来源: 咪咕和网易云（API 是从公开的网络中获得）

## 说明

1. 部分歌曲支持无损音乐（目前只有咪咕服务支持无损flac音乐的下载，网易云服务暂时只支持mp3），支持格式：flac、mp3
2. 优先搜索下载高品质音乐（无损 -> 320K -> 128K）
3. 暂时只支持下载咪咕及网易云平台上已有的音乐（因一些特殊原因，腾讯旗下的平台都是不支持的，同时网易云平台上VIP尊享音乐也是不支持下载的）
4. 在 `windows` 桌面端的 `git Bash` 中不支持上下切换选歌，问题是 `inquirer` 不兼容，建议使用其它终端工具
5. node version > 14