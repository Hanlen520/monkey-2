# monkey

* 一个monkey压力测试框架.
* 从以前所写的automation_demo里面分离出来.(https://github.com/afantishui/python_automation_demo)
* 加入adb二次封装方法与图像识别.

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

* -img (把项目截图删除后不显示，可自行建文件夹)
*     -queryImg  匹配图片存放
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

* 1.部分adb命令封装（已实现）
* 2.移动端性能数据收集（已实现）
* 3.图像识别功能（已实现）
* 4.用例编写时要把每步的截图放入queryImg目录

* 5.在匹配到目标图片的地方做标记，截图保存（挖坑）
* 6.加入操作步骤日志输出（挖坑）
* 7.写一个冒烟模块demo（挖坑）
* 8.输出报告（挖坑）

