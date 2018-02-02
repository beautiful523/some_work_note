### 安装python3
安装python3的时候不要将/usr/bin/python这个软连接从python2指向python3,这样会带来一些麻烦。比如说pip安装不上。
如果已经这样做了，可能会报如下的错：
ImportError: No module named 'ConfigParser'
解决办法：
先将软连接改回去
rm /usr/bin/python
 ln -s /usr/bin/python2 /usr/bin/python
 再重新装python-configparser
sudo apt-get purge --auto-remove python-configparser
sudo aptitude install python-configparser
### ipython和python的区别
ipython有tab键提示
### 安装pip
https://www.cnblogs.com/twtp/p/5325649.html
sudo apt-get install python-pip
sudo apt-get install python3-pip

### ubuntu下markdown编辑神器haroopad安装与配置
https://www.jianshu.com/p/064aec7a5164
然后命令行输入haroopad运行
### 装git
http://blog.csdn.net/qq_33052539/article/details/52820032
### 安装subl
https://jingyan.baidu.com/article/64d05a023cd849de55f73be4.html
http://blog.csdn.net/flyfish111222/article/details/51886787
### Ubuntu下MongoDB的安装和使用
http://blog.csdn.net/flyfish111222/article/details/51886787
### 安装selenium
官网下载安装包https://pypi.python.org/pypi/selenium
进入安装包所在目录 cd ~/Downloads
解压缩tar zxvf selenium-3.8.1.tar.gz
进入解压缩后目录 cd selenium-3.8.1/
安装 sudo python setup.py install

报错unable to start phantomjs with ghostdriver
解决 apt-get方式安装phantomjs


