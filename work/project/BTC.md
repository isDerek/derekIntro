# 基于 MK64 的大树云

---

**项目概述：**

1. 该项目采集数据上传至云端，通过手机监控设备
2. 通过后台管控系统将设备采集的数据导出 Excel
3. 通过手机 APP 监控设备

**人员安排：**

设备端软件 1 人、后台管控系统 1 人、Android APP 1 人、IOS APP 1 人

**个人职责：**

设备端软件设计

**具体内容：**

1. 实现设备以太网联网并通过 Socket 连接云端，以 JSON 格式的私有协议打通与云端的链路层通讯(设备注册、设备控制等)
2. 编写 Bootloader，实现大树云主控板的 OTA 升级，检验采用 CRC 和 MD5
3. I2C 调通紫外线传感器、RGB 灯、温湿度传感器、压力传感器、光强传感器、OLED 屏
4. PWM 控制电机
5. 基于 FreeRTOS 多线程编程（异常模块、事件模块、定时器模块、网络模块）
6. LWIP 协议栈实现 DHCP
