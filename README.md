# Padavan-build说明
现在不需要新建Release了，已经更改了脚本，直接fork，修改好之后，点击右上角的 Star 星星按钮即可开始自动编译（自己点击才会编译）。

### 遇见的问题 ###
* Error：Process completed with exit code 2 
* 即（https://github.com/chongshengB/Padavan-build/issues/295）

 —————————————————————————————————————————————————————————————

* 解决方法： 
* 到h大那下载新库—— rt-n56u/trunk/user/htop/Makefile 
*  （https://github.com/hanwckf/rt-n56u/blob/master/trunk/user/htop/htop-3.0.2.tar.gz） 
* 把rt-n56u库fork一下，然后再自己的库中上传新库，并修改一下同一目录下的Makefile第二行
* 再修改一下自编译代码中的workflows/build-padavan.yml第36行，如下
*   git clone --depth=1 https://github.com/pKm8/rt-n56u.git /opt/rt-n56u
*   指向自己的库
 
 ———————————————————————————————————————————————————————————————
