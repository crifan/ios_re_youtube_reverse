# iOS逆向开发：YouTube逆向

* 最新版本：`v0.8`
* 更新时间：`20221104`

## 简介

以YouTube逆向介绍典型的iOS逆向的流程。先是YouTube逆向概述，再是详细介绍iOS的YouTube逆向的详细过程，包括砸壳ipa以及安装ipa、静态分析的导出头文件、IDA分析代码逻辑、动态调试的分析界面元素和MonkeyDev调试，其中界面分析用Reveal、Cycript；MonkeyDev调试典型逻辑是，猜测类和函数、写hook代码、加断点调试；期间涉及到恢复符号表、Charles抓包；然后介绍逆向的产出和相关总结；产出包括app内部逻辑和广告过滤相关内容；以及相关子教程。

## 源码+浏览+下载

本书的各种源码、在线浏览地址、多种格式文件下载如下：

### HonKit源码

* [crifan/ios_re_youtube_reverse: iOS逆向开发：YouTube逆向](https://github.com/crifan/ios_re_youtube_reverse)

#### 如何使用此HonKit源码去生成发布为电子书

详见：[crifan/honkit_template: demo how to use crifan honkit template and demo](https://github.com/crifan/honkit_template)

### 在线浏览

* [iOS逆向开发：YouTube逆向 book.crifan.org](https://book.crifan.org/books/ios_re_youtube_reverse/website)
* [iOS逆向开发：YouTube逆向 crifan.github.io](https://crifan.github.io/ios_re_youtube_reverse/website)

### 离线下载阅读

* [iOS逆向开发：YouTube逆向 PDF](https://book.crifan.org/books/ios_re_youtube_reverse/pdf/ios_re_youtube_reverse.pdf)
* [iOS逆向开发：YouTube逆向 ePub](https://book.crifan.org/books/ios_re_youtube_reverse/epub/ios_re_youtube_reverse.epub)
* [iOS逆向开发：YouTube逆向 Mobi](https://book.crifan.org/books/ios_re_youtube_reverse/mobi/ios_re_youtube_reverse.mobi)

## 版权和用途说明

此电子书教程的全部内容，如无特别说明，均为本人原创。其中部分内容参考自网络，均已备注了出处。如发现有侵权，请通过邮箱联系我 `admin 艾特 crifan.com`，我会尽快删除。谢谢合作。

各种技术类教程，仅作为学习和研究使用。请勿用于任何非法用途。如有非法用途，均与本人无关。

## 鸣谢

感谢我的老婆**陈雪**的包容理解和悉心照料，才使得我`crifan`有更多精力去专注技术专研和整理归纳出这些电子书和技术教程，特此鸣谢。

## 更多其他电子书

本人`crifan`还写了其他`150+`本电子书教程，感兴趣可移步至：

[crifan/crifan_ebook_readme: Crifan的电子书的使用说明](https://github.com/crifan/crifan_ebook_readme)
