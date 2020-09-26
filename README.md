# bt580-demo
Android BLE Source code for IRXON BT580 Serial Bluetooth adapter application.





下载到的是bt580-demo-master.zip压缩文件，解压缩后，得到一个名为bt580-demo-master的项目文件夹。
这个项目是在Android Studio上开发的，在Android Studio启动界面，选择Import Project。如下图：




导入解压缩后的bt580-demo-master项目文件夹，如下图：




导入后，Android Studio编程开发界面如下图所示：
java目录下面共有三个java文件，与BT580用户二次开发密切相关的是MainActivity和Ble_Activity这两个java文件。

MainActivity的主要功能是搜索手机周围的蓝牙设备，目的是找到BT580从机。

Ble_Activity是蓝牙BT580应用开发的主要代码。它的主要功能包括：与BT580从机建立蓝牙连接、查找BT580串口透传的特征值、 在屏幕下方发送文本对BT580特征值进行写操作、开启特征值的Notify通知功能、监听Notify通知的数据并在屏幕上方显示。
通过对特征值的写和监听，实现与BT580的蓝牙BLE通讯，进而与BT580所连接的串口设备实现无线串口通讯。

BT580用户的个性化应用二次开发，只需要改变Ble_Activity文件里的数据处理方式即可。
本例程将收到的数据直接在手机屏幕上方显示，用户可根据自己串口设备的特点，修改一下界面，处理一下数据，然后再显示出来。
本例程将发送的文本直接写入特征值了，用户可根据自己串口设备的特点，修改一下界面，比如设置多个按钮发送特定数据，实现对串口设备的远程控制或设置。




点击Build，选择Build APK，即可生成可以在安卓手机上直接安装的apk文件。如下图：



