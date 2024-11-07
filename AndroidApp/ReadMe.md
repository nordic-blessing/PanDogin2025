2024/11/05 16:45
written by Icol Lee

1.将本文件位置添加到系统环境变量中
2.win+r，输入cmd，进入终端，输入adb version查看版本号
3.手机进入开发者模式，并打开USB调试，允许USB安装应用，将手机通过USB数据线连接电脑
4.在电脑终端输入adb get-serialno，获取手机序列号（需要在手机端点击允许）
5.在电脑终端输入adb install .apk文件的地址（如果地址中包含空格，需要用引号套起）
6.如果安装失败，电脑终端输入 adb install --bypass-low-target-sdk-block .apk文件的地址
7.终端显示“Success”,且手机端出现PanDogin的应用图标，则安装成功