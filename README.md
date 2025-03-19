界面--Ionic：主要负责前端用户界面的构建和应用的样式，提供了一整套美观的预构建组件，简化了开发过程。

打包--Cordova：负责将 Ionic 应用打包为原生应用，并提供与设备硬件的交互功能，使得 Web 应用可以利用设备的原生能力。

安装：
    1、安装 Java SE 8
    2、安装 Node.js
    3、安装 Cordova 和 Ionic CLI：
       npm install -g cordova
       npm install -g @ionic/cli
    4、创建一个新的 Ionic 项目
       ionic start MyIonicApp blank
    5、添加 Cordova 平台
       cd MyIonicApp
       ionic cordova platform add android
    6、编写src，调试
    7、运行以下命令以构建 APK 文件：
       ionic cordova build android
        
