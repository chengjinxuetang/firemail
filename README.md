# firemail
open sourece mail client refer to MailSpring


创建工程步骤
1.初始化工程
cd firemail
npm init

设置相关参数
调整相关配置

2.执行安装
npm install

注意：postinstall钩子在安装完node_modules中的模块后会执行
遇到的问题
request to https://registry.npmjs.org/abab failed, reason: certificate is not yet
设置
npm config set strict-ssl false

查看npm镜像源
npm config get registry 
npm config get disturl
设置npm镜像源
npm config set registry https://registry.npm.taobao.org
npm config set disturl https://npm.taobao.org/dist

3.相关下载地址
https://mailspring-builds.s3.amazonaws.com/stable.txt
内容
1.9.1-30ef802f
->
http://firemail.wang/stable.txt


https://mailspring-builds.s3.amazonaws.com/client/${head}/${distDir}/mailsync.tar.gz
->
http://firemail.wang/client/${head}/${distDir}/mailsync.tar.gz


  OS       |  ${head} |  ${distDir}  | ${process.platform} | ${process.arch}
win10 x64  | 30ef802f |   win-ia32   |   win               | ia32

所谓IA32就是“Intel32位体系结构”（Intel Architecture 32-bit），而我们常说的X86-64就是IA32的64为拓展。

下载官方的压缩包
https://mailspring-builds.s3.amazonaws.com/client/30ef802f/win-ia32/mailsync.tar.gz


应用程序目录：
%appdata%\Firemail-dev
%appdata%\Firemail

程序运行效果:
![firemail](https://github.com/chengjinxuetang/firemail/blob/main/screenshot/firemail.gif)