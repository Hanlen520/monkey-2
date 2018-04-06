# monkey

一个monkey的测试框架.放假有空把这个从automation_demo中分离出来,加入adb二次封装方法与图像识别。

## 所需环境
* Python3
* monkey
* adb
* opencv模块

## 目录结构

*  -Base
*     -analysis.py    分析monkey日志
*     -imgProcess.py  图像识别
*     -init.py        初始化配置
*     --monkeyBase.py  封装monkey命令
*     -readconfig.py  读取配置

*  -config
*     -config.yml    ui自动化配置
*     -monkey.yml    跑monkey命令配置

* -Base
*     -queryImg  匹配图片存放
*     -sceneImg  截图目录

* -lib
*     -Excel_report.py  输出monkey报告
*     -logger.py        日志函数

 * -logs 日志文件

 * -RunTest 执行脚本文件夹

 * -test_report 报告文件夹

 * -testsuites  用例脚本
## monkey压力测试部分
* monkey跑冒烟 命令配置-执行-日志分析-输出报告
* 参数配置在config\.yml,根据需要进行设置
* 输出的是excel报告
* 跑10W次,每次延时300ms,耗时2.5H（供参考）

## 图像识别部分方法说明：

* 已实现：
*     1.部分adb命令封装
*     2.移动端性能数据收集
*     3.图像识别功能
*     4.用例编写时要把每步的截图放入queryImg目录

* 挖个小坑
*     1.在匹配到目标图片的地方做标记，截图保存
*     2.加入操作步骤日志输出
*     3.写一个冒烟模块demo
*     4.输出报告

