MIUI_patchrom_Find5
===================
1.安装Java SDK和Android SDK 附：AOSP编译环境搭建 一键搭建编译环境脚本

2.安装Git and Repo

$ mkdir ~/bin

$ PATH=~/bin:$PATH

$ curl http://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/bin/repo

$ chmod a+x ~/bin/repo

3.同步代码

$ mkdir MIUI && cd MIUI

$ repo init -u git://github.com/MiCode/patchrom.git -b kitkat

$ repo sync -j4

$ git clone https://github.com/lilinxin9712/MIUI_patchrom_Find5

4.编译MIUI

$ source build/envsetup.sh && cd Find 5

$ make fullota

5.输出目录out下的fullota.zip即为所得MIUI ROM

感谢

感谢MIUI官方开源patchrom

感谢github上无私奉献代码的朋友
All the stuff related to the miui porting device OPPO Find 5
