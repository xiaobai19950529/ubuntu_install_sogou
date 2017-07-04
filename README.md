# ubuntu_install_sogou

ubuntu16.04 搜狗输入法的安装

1，添加fcitx的键盘输入法系统，因为sogou是基于fcitx的，而系统默认的是iBus；
2，安装sogou输入法；

第一步、添加fcitx键盘输入法系统
先添加以下源
sudo add-apt-repository ppa:fcitx-team/nightly

然后更新下系统

sudo apt-get update

开始安装fcitx
sudo apt-get install fcitx

sudo apt-get install fcitx-config-gtk

sudo apt-get install fcitx-table-all

sudo apt-get install im-switch

第二步，安装搜狗输入法，去官网下载对应版本的资源包

http://pinyin.sogou.com/linux/?r=pinyin

去到~/Downloads下
cd ~/Downloads 
sudo dpkg -i xxx.deb 

第三步 设置语言选项
1。到系统设置->语言支持，将键盘输入法系统由默认的iBus设置为fcitx
2.然后注销一次
3.搜索出fcitx配置，将sogou输入法设为默认即可
