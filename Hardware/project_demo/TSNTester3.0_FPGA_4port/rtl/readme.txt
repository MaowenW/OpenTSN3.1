﻿本目录下的rtl文件是TSNSwitch3.0的网络接口数目相关文件和器件相关文件，此示例工程是实例化4个网络接口的TSN交换机工程。本目录中各个文件说明如下：
1.网络接口数目相关文件
um.v：                                    每个接口映射逻辑，在TSN测试仪3.0示例工程中，0号接口用于处理时间同步相关逻辑，1号接口用于发送测试报文，2号接口用于接收测试报文，3号接口用于接收TSN测试仪配置报文、发送TSN测试仪状态上报报文和测试封装报文
tester_3_0_top.v:                      网络接口输入处理逻辑和网络接口输出处理逻辑实例化数目相关代码，根据网络接口数目实例化对应数量的gmii_adapter，以及调用um.v
2.器件相关文件
除um.v，tester_3_0_top.v外，其他文件均为器件相关文件。