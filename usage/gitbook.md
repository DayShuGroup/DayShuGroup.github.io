### Windows安装GitBook

1. 安装nodejs

   GitBook是基于nodejs,所以需要nodejs环境，去官网下载（https://nodejs.org/en/download/），  一般默认包含npm包管理工具。

   

2. 安装GitBook

   使用npm安装

   ```` shell
   npm install -g gitbook-cli 
   gitbook -V 
   
   ````
   
   gitbook -V 如果没有安装gitbook 则自动安装，否则显示版本信息。
   
3. 查看是否安装成功

   ````
   gitbook -V
   ````

   如果能显示版本信息，则安装成功，反之，则安装失败。

4. 安装问题

   * 如果安装报错：TypeError: cb.apply is not a function

     解决：换个nodejs版本安装，（不知道是什么问题），亲测10.14.1 本版成功。



###  GitBook使用

1. 创建存放文档的目录,需切换到新创建的目录运行命令

   ```` shell
   gitbook init
   ````

   * 会生成SUMMARY和README文件。
   * 如果存在SUMMARY会重新引用链接的其他文档，没有则创建。

