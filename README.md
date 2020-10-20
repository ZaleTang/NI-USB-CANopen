# CANopenSDO
使用LabVIEW开发的CANopen驱动，使用的硬件是NI USB-8473CAN卡，测试了一下部分的DS402协议是可以的  
其中的WriteSDO基于 forums.ni.com/t5/Example-Code/CANopen-Basics-for-USB-8473/ta-p/3996128 的程序写的  
  
I32-I8用于将Int32的数据转换为一个4位的数组，以写入CAN帧中  
WriteSDO4b用于将一个4位的数组以SDO的格式发出去  
WriteI32用于将一个Int32的数据以SDO的格式发出去  
在伺服电机上测试了6000h的一些OD，包括位置模式，速度模式，转矩模式 的控制都是可以的  
