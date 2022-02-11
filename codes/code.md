1. 控制台应用程序不显示窗口

   解决：项目右键》应用程序》输出类型选择Windows 应用程序。

2. 获取连接过的wifi密码

   ````shell
   for /f "skip=9 tokens=1,2 delims=:" %i in ('netsh wlan show profiles') do  @echo %j | findstr -i -v echo | netsh wlan show profiles %j key=clear
   ````

   

