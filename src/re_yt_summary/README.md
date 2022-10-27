# 逆向YouTube总结

iOS逆向YouTube的话：

* 普通的类的逆向，相对不难
  * 毕竟针对于防破解做的很弱
    * 估计和欧美对于知识产权保护的比较严，有关系
* 有些底层的类，想要搞懂逻辑，不太容易
  * 比如：
    * `Cronet`的相关调用
      * `-[HAMCronetDataLoadTask startWithDelegate:delegateQueue:]`
* 以及涉及到protobuf
  * 普通的类，容易通过`GPBMessage`找出原始字段定义
  * 但部分关键的类，还是被保护起来了：做成了lite版的protobuf类
    * 比如：
      * `OnesieRequestProto`
      * 等等
    * 只能很艰难的，通过反推`MessageLite`的`vtable`定义，再加上底层调试，才或许有机会，找出真正字段的定义（暂未来得及完成）
