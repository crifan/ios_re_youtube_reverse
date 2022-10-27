# IDA分析代码逻辑

主要涉及，分别用IDA加载和分析，YouTube的2个二进制的文件：

* `YouTube`
* `Module_Framework`

然后分析其代码逻辑。

其中最核心用法是，找到可以的要研究的类的函数后，去`Functions`窗口中，通过函数名搜索函数，找到对应汇编代码，再`F5`查看反编译后的伪代码，尝试搞懂代码的具体逻辑。

## 特殊：导出IDA全部伪代码

为了更好的，全局去搜一些类、变量、字符串等，用于iOS逆向研究YouTube的逻辑

所以考虑去导出全部的IDA伪代码：

TODO：

* 【未解决】IDA图形界面GUI模式使用ida-batch_decompile批量导出全部YouTube的Module_Framework全部伪代码
* 【未解决】用IDA的命令行文本模式使用ida-batch_decompile批量导出全部YouTube的Module_Framework全部伪代码
* 【未解决】用插件导出IDA的YouTube的Module_Framework的全部反汇编的源码伪代码
* 【记录】IDA中用idat64的Batch Mode尝试反编译导出全部源代码：试试二进制小点的
* 【已解决】IDA中用idat64的Batch Mode尝试反编译导出YouTube的Module_Framework全部代码伪代码
