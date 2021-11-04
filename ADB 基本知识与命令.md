#### ADT（_Android Development Tools_ —— 安卓开发工具）

> 在搭建 Android 开发环境的时候，开发人员需要为 `Eclipse` 安装 `ADT` 插件，该插件可以提供一个强大的 Android 集成开发环境。通过给 `Eclipse` 安装 `ADT` 插件，开发人员才能够完成快速新建 Android 项目、创建界面、调试程序、导出 `.apk` 等一系列的开发任务。

#### SDK （_Software Development Kit_ —— 软件开发部件）

> 通常是为辅助开发某类软件而编写的特定软件包，框架集合等，`SDK` 一般包含相关文档，范例和工具。

#### ADB（_Android Debug Bridge_ —— 安卓调试桥梁）

> 用来连接安卓手机与 PC 端的桥梁，通过 `ADB` 服务，在 PC 端通过输入命令，通过命令行界面对手机进行全面的操作。

### **ADB 命令**

```shell
连接 Android 手机的方式：USB 或者通过 Wi-Fi
# 方式一：USB
> 前置准备：
1.电脑安装好 ADB,并配置好环境变量
2.下载ADB驱动
3.一台安卓手机,一根USB线
4.手机开启开发者模式,并勾选 USB 调试

>> 步骤:
1.通过 USB 线将安卓手机连接电脑
2.通过电脑给安卓手机安装 ADB 驱动
3.运行cmd,输入命令 adb devices 检查手机与电脑是否连接成功


# 方式二：Wi-Fi
> 前置准备：
1.电脑安装好 ADB,并配置好环境变量
2.一台安卓手机,一根USB线
3.手机开启开发者模式，并勾选 USB 调试

>> 步骤：
1.通过 USB 线将安卓手机连接电脑
2.运行 cmd,输入命令 adb tcpip 5555 可重启 adb 监听的端口 5555
3.断开 USB 连接
4.进入手机设置中的 WLAN,查看手机 IP 地址
5.运行 cmd,输入命令 adb connect [手机 IP 地址]:[端口号 5555]
PS：第五步的端口号 5555 可以省略
```



```shell
adb connect ip 地址 ————— 连接设备
adb disconnect ip 地址 —————— 断开连接
adb devices —————— 查看设备连接状态
```

