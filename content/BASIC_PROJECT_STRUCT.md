Android 工程结构
============================

## 结构

这是第一个工程目录树
```
├── app
│   ├── build.gradle
│   ├── libs
│   ├── proguard-rules.pro
│   └── src
│       ├── androidTest
│       │   └── java
│       │       └── com
│       │           └── example
│       │               └── firstproject
│       │                   └── ExampleInstrumentedTest.java
│       ├── main
│       │   ├── AndroidManifest.xml
│       │   ├── java
│       │   │   └── com
│       │   │       └── example
│       │   │           └── firstproject
│       │   │               ├── FirstFragment.java
│       │   │               ├── MainActivity.java
│       │   │               └── SecondFragment.java
│       │   └── res
│       │       ├── drawable
│       │       │   └── ic_launcher_background.xml
│       │       ├── drawable-v24
│       │       │   └── ic_launcher_foreground.xml
│       │       ├── layout
│       │       │   ├── activity_main.xml
│       │       │   ├── content_main.xml
│       │       │   ├── fragment_first.xml
│       │       │   └── fragment_second.xml
│       │       ├── menu
│       │       │   └── menu_main.xml
│       │       ├── mipmap-anydpi-v26
│       │       │   ├── ic_launcher.xml
│       │       │   └── ic_launcher_round.xml
│       │       ├── mipmap-hdpi
│       │       │   ├── ic_launcher.webp
│       │       │   └── ic_launcher_round.webp
│       │       ├── mipmap-mdpi
│       │       │   ├── ic_launcher.webp
│       │       │   └── ic_launcher_round.webp
│       │       ├── mipmap-xhdpi
│       │       │   ├── ic_launcher.webp
│       │       │   └── ic_launcher_round.webp
│       │       ├── mipmap-xxhdpi
│       │       │   ├── ic_launcher.webp
│       │       │   └── ic_launcher_round.webp
│       │       ├── mipmap-xxxhdpi
│       │       │   ├── ic_launcher.webp
│       │       │   └── ic_launcher_round.webp
│       │       ├── navigation
│       │       │   └── nav_graph.xml
│       │       ├── values
│       │       │   ├── colors.xml
│       │       │   ├── dimens.xml
│       │       │   ├── strings.xml
│       │       │   └── themes.xml
│       │       ├── values-land
│       │       │   └── dimens.xml
│       │       ├── values-night
│       │       │   └── themes.xml
│       │       ├── values-w1240dp
│       │       │   └── dimens.xml
│       │       ├── values-w600dp
│       │       │   └── dimens.xml
│       │       └── xml
│       │           ├── backup_rules.xml
│       │           └── data_extraction_rules.xml
│       └── test
│           └── java
│               └── com
│                   └── example
│                       └── firstproject
│                           └── ExampleUnitTest.java
├── build.gradle
├── gradle
│   └── wrapper
│       ├── gradle-wrapper.jar
│       └── gradle-wrapper.properties
├── gradle.properties
├── gradlew
├── gradlew.bat
├── local.properties
└── settings.gradle
```

## 重要的文件和目录说明
> 根目录
>> app
>>> build.gradle 模块 app 的构建配置
>>> libs 外部依赖 Jar 区域
>>> proguard-rules.pro 代码混淆配置，用于发布上线，保护代码
>>> src
>>>> androidTest Android 自动化测试代码区域
>>>> main 工程区域
>>>>> AndroidManifest.xml 工程配置文件
>>>>> java 工程代码区域
>>>>> res 工程资源区域
>>>>>> drawable 图像类资源，一般用于矢量图
>>>>>> mipmap-XXX 图像类资源，不同设备适配用
>>>>>> menu 菜单类资源
>>>>>> values 数据资源区域
>>>>>>> colors 颜色资源
>>>>>>> string 字符串资源
>>>> test 工程单元测试区域
> gradle Gradle封装，一般不用更改
> build.gradle 全局构建配置
> gradle.properties Gradle 构建参数
> gradlew 命令行构建命令，非Windows专用，用于自动化构建
> gradlew.bat 命令行构建命令，Windows专用，用于自动化构建
> local.properties 配置本机路径，一般用于 SDK、NDK 等路径