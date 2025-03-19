#界面--Ionic：主要负责前端用户界面的构建和应用的样式，提供了一整套美观的预构建组件，简化了开发过程。

#打包--Cordova：负责将 Ionic 应用打包为原生应用，并提供与设备硬件的交互功能，使得 Web 应用可以利用设备的原生能力。

#安装：
    1.安装 Java SE 8
    2.安装 Node.js
    3.安装 Cordova 和 Ionic CLI：
       npm install -g cordova
       npm install -g @ionic/cli
    4.创建一个新的 Ionic 项目
       ionic start MyIonicApp blank
    5.添加 Cordova 平台
       cd MyIonicApp
       ionic cordova platform add android
    6.编写src，调试
    7.运行以下命令以构建 APK 文件：
       ionic cordova build android
        
前端
![image](https://github.com/user-attachments/assets/25a2b94d-ba2b-4b32-aada-a2155c70919a)

后端
![image](https://github.com/user-attachments/assets/690d6e5f-be50-4f91-8627-994cfbfb15f8)

Ionic和Cordova属于前端移动应用，而Java SE 8和Tomcat是后端服务

Ionic的app.component.ts是入口组件，Cordova的config.xml是配置，Android的MainActivity是启动点

Tomcat通常用于运行Servlet/JSP应用,Java Web应用。

1.Ionic应用通过HttpClient（Angular）发送请求到Tomcat后端：
2.Tomcat解析请求路径，调用对应的Servlet处理。
3.Java后端返回JSON数据，Ionic前端渲染结果。

部署流程
后端：通过Maven打包为WAR文件，部署到Tomcat的webapps/目录。
前端：运行ionic build --prod && cordova build android生成APK。
联调：确保Tomcat端口开放，Android应用配置正确的API地址。
            

