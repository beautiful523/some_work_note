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
### ubuntu下markdown编辑神器haroopad安装与配置
https://www.jianshu.com/p/064aec7a5164
然后命令行输入haroopad运行
