## linux常用压缩命令2

先打包在压缩，可以压缩多个目录（多个目录之间以空格分隔） -c 压缩， -x 解压缩, -t 查看压缩文件


### 常用压缩格式

```
.tar.gz  .tar.bz2

先打包在压缩，可以压缩多个目录
tar -cvf 打包文件 源文件  

tar -cvf jp.tar jp


ls
gzip jp.tar

gzip -d jp.tar.gz

bzip2 jp.tar


bzip2 -d jp.tar.bz2

rm -rf jp

tar -xvf  解压缩

tar -xvf jp.tar


tar -zcvf 压缩包名.tar.gz 源文件
-z 压缩为.tar.gz

tar -zxvf 压缩包名.tar.gz

-x 解压缩.tar.gz格式


tar -jcvf 压缩包名.tar.bz2 源文件

-z: 压缩为.tar.bz2格式

tar -jxvf 压缩包名.tar.bz2
-x 解压缩.tar.bz2格式


tar -zcvf jp.tar.gz jp

rm -rf jp

tar -zxvf jp.tar.gz

tar -jcvf jp.tar.bz2 jp

tar -jxvf jp.tar.bz2 -C /tmp/ 指定解压缩位置

tar  -zcvf test.tar.gz jp abc

tar -zcvf /tmp/test.tar.gz jp abc

tar -zxvf test.tar.gz

tar -ztvf test.tar.gz 查看压缩目录
-t 查看压缩目录

```
