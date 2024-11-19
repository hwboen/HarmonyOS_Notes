## 熟悉 DevEco-Studio

DevEco-Studio 它的全称是 Developer Eco Studio，Eco 是 Ecosystem 生态的简写。

DevEco-Studio 创建的项目类型有 Application 和 Atomic Service 两种。Application 是最原始的 App 形式，需要用户主动安装，而 Atomic Service 的主体是服务，无需进行安装，通过 HarmonyOS 系统的 OneHop（手机碰一碰）或者扫码调用。

## 创建一个 Empty Application Project

创建的时候需要填写：

- Project name
  项目名，应用名称默认和项目名相同
- Bundle name
  应用的唯一标识符，通常采用反域名的形式，例如 com.boen.beagle，其中第一级为域名后缀 com，第二级为厂商或者个人名，这里就是 boen，
  第三极为应用名 beagle。bundle 的中文意思是捆绑，应用最终会将各类资源打包到一起，形成一个 bundle 供应用市场进行分发。因此这里的 bundle 可以理解为 App 在应用市场上的表现形式。
- Save Location 项目存储地址
- Compatible SDK
  最低兼容的 SDK 版本
- Module name
  主包名称，鸿蒙项目采用模块化的结构设计，可以划分不同的功能模块，一个应用只有一个主包。
- Device type
  用户标识当前 Module，这里是主包，可以运行在哪些设备类型上，目前的类型有 phone,tablet 平板，2in1 设备（电脑的屏幕和键盘可拆卸触摸），tv 智慧屏，wearable 智能手表，car 车机。

## 熟悉 Application Project 的目录结构

创建好项目之后，让我们熟悉一下项目结构。

首先项目文件有配置、资源、源码三大类型，并且按项目 Project 和模块 Module 进行划分。

我们先从项目 Project 这一层说起：

- `.hvigor`
