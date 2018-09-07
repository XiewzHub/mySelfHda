



# 修改DSDT步骤

> 要修改dsdt需要知道的网址
>
> - [https://bitbucket.org/RehabMan/，资源丰富，长期维护](https://bitbucket.org/RehabMan/)
> - [https://www.tonymacx86.com，集合大量关于黑苹果安装以及问题的解决方案，可能需要梯子](https://www.tonymacx86.com)

本文参考的文章

- [对笔记本的 DSDT／SSDT 打补丁](https://blog.csdn.net/wr132/article/details/54798754)
- [各种教程，很强大](http://enjoycc.f3322.net:8558/黑苹果安装教程/)

## 1 提取系统的ACPI的表

![](http://ww1.sinaimg.cn/large/e8450fe4gy1fv0pgul5izj20q90pcn0q.jpg)

## 2 反编译文件成为asl文件

### 反编译

mac下使用命令反编译，反编译命令[下载](https://bitbucket.org/RehabMan/acpica/downloads/)后可以通过命令

```
cd ~/Downloads
unzip iasl.zip
sudo cp iasl /usr/local/bin
```

将该命令放置到可执行的终端，然后可以通过`iasl -da -dl *.aml`命令来进行反编译DSDT表。

参考文章https://blog.csdn.net/wr132/article/details/54798754

### 修改源码

修改源码需要有个比较合适的源码编辑器，mac系统使用的软件为[MaciASL](https://bitbucket.org/RehabMan/os-x-maciasl-patchmatic/downloads/)，是一个在GitHub上的开源项目，此软件用于编辑aml代码，提供了代码高亮显示，和一些插件等。




