# qGroundControl开发环境搭建

​		本文介绍qgc3.4.4版本代码在windows环境下开发环境的搭建。由于qgc必须使用MSVC2015 32bit编译器编译，所以在搭建qt环境前首先需要安装vs2015的C++编译器，由于qt5.12及以上版本不包含MSVC2015 32bit的qt库，所以本文使用qt5.11.3版本。  

## 1. VS2015下载及安装

		### 1.1 vs2015下载

​		在https://msdn.itellyou.cn/中下载vs2015如下图所示

 <img src="C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200201211132434.png" alt="image-20200201211132434" style="zoom: 67%;" />

​		这个网站的下载速度特别快。

​		我下载的文件名是：cn_visual_studio_community_2015_with_update_3_x86_x64_dvd_8923246.iso

### 2.2 VS2015安装

​		只需要选择C++选项，若下图所示。

​		![image-20200201211737760](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200201211737760.png)  

## 2 qt5.11.3下载及安装

### 2.1 qt5.11.3下载

​		高速下载地址为:http://download.qt.io/archive/qt/5.11/5.11.3/ 

​		在windows下的开发环境下载项是:

![image-20200201212446840](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200201212446840.png)

## 2.2 qt5.11.3的安装选项

​		必须选择MSVC 2015 32-bit与Qt Charts等组建，我选择的组建如下所示:

![image-20200201212917025](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20200201212917025.png)

## 3. qGroundControl编译

​		用Qt Creator打开qgroundcontrol.pro文件，构建套件选择“MSVC2015 32bit”。

​		编译过程中如果遇到错误"user_config.pri: No such file or directory"，右键点击工程名，选择“重新构建”。
