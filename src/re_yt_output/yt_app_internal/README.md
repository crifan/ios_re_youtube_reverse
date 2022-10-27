# YouTube的app内部逻辑

TODO：

* 网络请求
  * 【整理】YouTube广告拦截从头播放视频：相关的网络请求和大概逻辑
* 网络协议
  * Cronet
    * 【整理】Cronet相关源码和定义和具体实现
    * 【已解决】YouTube中struct Cronet_UrlRequestCallback的具体定义实现
    * 【已解决】iOS的YouTube中Cronet_UrlRequestCallback的OnFailed中cronet=10和quic协议关系
  * QUIC
    * 【整理】YouTube相关：QUIC协议和源码
  * 【整理】YouTube涉及到的Network、quic等Chromium相关源码
  * 【整理】YouTube涉及到Chromium中Cronet相关源码和文档
* YouTube视频格式
  * 【整理】YouTube中视频相关信息：ISO Media file produced by Google Inc
  * 【未解决】YouTube的response的data视频格式：ftyp=dash
  * 【整理】YouTube逻辑：视频流格式代码
* HTTP协议
  * 【已解决】研究YouTube视频内容请求：Transfer-Encoding chunked
* 【整理】YouTube中Module_Framework函数对应关系 20220804
* YouTube广告过滤规则
  * 圈X
    * 【记录】研究YouTube逻辑：验证最新圈X的规则能否拦截广告
    * 【记录】pico中使用圈X最新规则的YouTube广告拦截效果
  * 【记录】测试最新版过滤规则的iOS的YouTube的app中广告过滤效果
* 调试相关
  * 【记录】Xcode+MonkeyDev动态调试YouTube：广告页面相关类
  * 【记录】调试YouTube广告页面：调试相关数据
