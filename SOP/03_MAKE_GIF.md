---
STATUS: 使用中
---

# 如何制作 gif 放到readme中作为演示说明

步骤如下。

## 一、人工手动录频

在macos上，人工使用cmd+shift+5,录制多个mov格式视频，每个3-10秒，修改命令为内容录制内容。
用户会手动把这些mov文件，存放到 docs/assets目录下。

## 二、使用命令压缩成gif

命令为：

```
ffmpeg -i demo.mov -vf "fps=10,scale=800:-1:flags=lanczos,split[s0][s1];[s0]palettegen[p];[s
1][p]paletteuse" demo.gif
```

AI 需要使用这个命令，将docs/assets下的mov全部转换成同名的gif。
生成完毕后，AI需要在.gitignore中，将docs/assets下的mov列入不提交部分。

## 三、添加到readme

AI 需要将这些gif，添加到readme中。如果根目录有readme_zh中文版本，也同时需要添加进去。
