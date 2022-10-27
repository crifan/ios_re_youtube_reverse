# Xcode+MonkeyDev

MonkeyDev调试YouTube的代码逻辑：

TODO：

* 【记录】恢复自己Mac的iOS逆向开发环境
* 【已解决】Xcode调试越狱iPhone6中的YouTube
* 【已解决】XCode+MonkeyDev动态调试YouTube的ipa
* 【记录】研究YouTube广告拦截导致视频从头播放的原因：XCode+MonkeyDev动态调试
* 【记录】恢复iOS逆向Xcode调试YouTube的开发环境

期间涉及：写hook代码，加断点调试：

找到一些可疑的，需要调试确认是否被调用到的类，则就是：去写hook代码，加断点，去调试看看是否触发：

* 如果触发：说明推测和判断是对的
* 如果没触发：说明推测出错
  * 再去找其他可疑的类，再继续去写hook加断点去调试

涉及的过程大概是：

* 【未解决】研究iPhone中YouTube的app播放视频中间广告导致从头播放
* 【已解决】iOS的Theos的Logos的hook代码中获取当前YouTube类YTWatchController的属性值activeVideoID
* 【记录】XCode的lldb调试YouTube的类：YTWatchController
* 【已解决】XCode+MonkeyDev动态调试YouTube：让程序停止在出现广告的页面
* 【基本解决】XCode的lldb中输出YouTube类MDXSession实例的属性值currentVideoID
* 【记录】给MonkeyDev的YouTube的hook中加上通用log代码
* 【已解决】XCode的lldb调试输出YouTube类YTWatchController实例的属性值和调用函数
* 【记录】XCode+MonkeyDev动态调试YouTube：寻找和广告相关的类和逻辑
* 【记录】XCode中Pause暂停去找YouTube的广告相关的类
* 【记录】研究YouTube广告逻辑：MDXPlaybackController的didPressSkipAd
* 【记录】研究YouTube广告逻辑：IDA中搜skipAd
* 【未解决】YouTube动态调试：写hook代码监控视频播放时间被重置变成0
* 以及后续换其他思路
  * 【记录】从.googlevideo.com入手找YouTube广告视频相关逻辑
  * 【记录】研究YouTube函数：resetWatchTime
  * 【记录】XCode+MonkeyDev动态调试YouTube：寻找和广告相关的类和逻辑
  * 【未解决】研究YouTube逻辑：找到最初的广告视频请求
  * 【未解决】研究YouTube逻辑：找到最初广告视频请求的响应
  * 【已解决】研究YouTube逻辑：找到带ctier=A的response和error出错的地方
  * 【已解决】研究YouTube逻辑：ctier=A时的 request和response的函数调用顺序
  * 【未解决】研究YouTube逻辑：寻找搞懂广告视频ID获取的大流程
  * 【已解决】研究YouTube逻辑：抓包iOS版YouTube的广告视频ID产生的大流程
