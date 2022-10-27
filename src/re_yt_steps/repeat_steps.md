# 重复上述过程

对于普通的iOS逆向，就重复上述过程

对于此处，逆向YouTube来说，具体是：

* 静态分析
  * 研究和搜索头文件中的类，找出可疑的类
    * `YouTube_17.08.2_headers`
      * `header_ModuleFramework`
      * `headers_YouTube`
  * 研究导出的字符串等资源中，是否有我们要的内容
    * `staticAnalysis`
      ```bash
      └── YouTube_17.08.2
          ├── Module_Framework
          │   ├── Module_Framework_nm.txt
          │   ├── Module_Framework_otool_l.txt
          │   ├── Module_Framework_otool_oV.txt
          │   └── Module_Framework_strings.txt
          ├── YouTube
          │   ├── YouTube_nm.txt
          │   ├── YouTube_otool_l.txt
          │   ├── YouTube_otool_oV.txt
      ```
* 动态调试
  * 分析界面元素
    * 从界面元素入手，找到对应的类或父类
      * 作为后续深入研究的切入点：找类的相关头文件
  * 调试代码逻辑
    * 针对可疑的类和函数，写hook代码，加断点调试
  * 期间涉及
    * 加过滤条件
      * 比如找到了`http`的`request`和`response`的类，还要继续加**过滤条件**
        * 过滤出我们所关心的类，比如initplayback，videoplayback等url
          * https://xxx.googlevideo.com/initplayback?xxx
          * https://xxx.googlevideo.com/videoplayback?xxx
    * log太多了，如何优化减少log
      * TODO：
        * 【已解决】研究YouTube逻辑：log日志打印优化每隔几次才输出
