- 1、data_collect.c  负责传感器数据的采集，主要包括水质传感器、温湿度传感器、太阳能电池电量等信息
- 2、data_send.c     负责采集数据的上传，上传至阿里云服务器
- 3、mqtt_connect.c  负责连接到阿里云服务器，包括密码的验证
- 4、ota.c           该线程一直等待阿里云的远程升级命令，如有远程升级命令，则执行远程升级操作
- 5、remote_config.c 该线程一直等待阿里云远程调试的指令
- 6、main.c          程序的主运行程序，处于一个while循环的状态，一直循环执行各个线程
**注；要根据实际编程的情况进行修改.**
