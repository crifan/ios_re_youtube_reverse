# iOS逆向开发：YouTube逆向

* [前言](README.md)
* [iOS逆向YouTube概览](reverse_youtube_overview/README.md)
* [逆向YouTube过程](re_yt_steps/README.md)
  * [砸壳ipa](re_yt_steps/crack_ipa/README.md)
    * [安装ipa](re_yt_steps/crack_ipa/install_ipa.md)
  * [静态分析](re_yt_steps/static_analysis/README.md)
    * [导出头文件](re_yt_steps/static_analysis/export_header.md)
    * [IDA分析代码逻辑](re_yt_steps/static_analysis/ida_f5_code.md)
  * [动态调试](re_yt_steps/dynamic_debug/README.md)
    * [分析界面元素](re_yt_steps/dynamic_debug/view_ui/README.md)
      * [Reveal](re_yt_steps/dynamic_debug/view_ui/reveal.md)
      * [Cycript](re_yt_steps/dynamic_debug/view_ui/cycript.md)
    * [调试代码逻辑](re_yt_steps/dynamic_debug/debug_logic/README.md)
      * [Xcode+MonkeyDev](re_yt_steps/dynamic_debug/debug_logic/xcode_monkeydev.md)
  * [重复上述过程](re_yt_steps/repeat_steps.md)
  * [期间涉及](re_yt_steps/invoked/README.md)
    * [恢复符号表](re_yt_steps/invoked/restore_symbol.md)
    * [Charles抓包](re_yt_steps/invoked/charles_capture.md)
* [逆向YouTube产出](re_yt_output/README.md)
  * [YouTube的app内部逻辑](re_yt_output/yt_app_internal/README.md)
    * [很多类的具体实现](re_yt_output/yt_app_internal/class_imp.md)
    * [返回数据](re_yt_output/yt_app_internal/resp_data.md)
  * [YouTube广告过滤相关](re_yt_output/yt_ads_filter/README.md)
    * [hook的类](re_yt_output/yt_ads_filter/hook_class.md)
    * [IDA伪代码](re_yt_output/yt_ads_filter/ida_code.md)
    * [函数调用逻辑](re_yt_output/yt_ads_filter/func_call.md)
    * [常见url](re_yt_output/yt_ads_filter/common_url.md)
* [逆向YouTube总结](re_yt_summary/README.md)
* [子教程](sub_book/README.md)
* [附录](appendix/README.md)
  * [参考资料](appendix/reference.md)
