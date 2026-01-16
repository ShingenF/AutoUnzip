# AutoUnzip
一个能监听指定文件夹内所有压缩包并自动解压的自动化程序  
An automated program that monitors a specified folder for all compressed archives and extracts them automatically.

前言：  
作者有从各种“站”上下压缩包的需求，往往都是加密的，挨个下载再手动解压超级麻烦，怒而开发一个自动化工具。本工具使用gemini3制作，作者本人患有轻度智力障碍，文化程度属于文盲或半文盲。如果你看见程序中有奇怪的写法，那一定是我的问题。如有非常弱智的操作请务必通过issue告知。这里提前感谢大佬们的指导！

注意：使用本程序必须安装7zip，下载方式：https://www.7-zip.org/  建议安装到默认路径。如果7zip安装在特殊路径下，可在“基础设置”中修改。

功能描述：  
1.可设置一组文件夹路径，开始监听后自动解压缩内部的压缩包文件。  
2.如果你经常下载密码相同的多个压缩包，可将常用密码记入密码本，自动解压过程中会自动尝试。  
3.“智能解压”可在包内文件/文件夹数量多余一个时，自动将所有文件解压到单独文件夹中，避免零碎文件泄露。建议开启。  
4.线程一栏为调用的cpu线程，如遇解压速度慢可增加，最大不建议超过cpu物理线程。  

警告：  
1.文件发布形式是一个文件夹，不建议将exe复制出来运行，因为你的所有配置信息都会通过生成一个json来保存。  
如果将exe单独复制出来运行，非常容易误删json文件导致所有保存的文件路径、密码全部丢失。  
2.如无必要，切勿关闭“严格模式”。在你使用百度网盘/aria2等下载工具时，它们可能会创建一个带有压缩包后缀的临时文件。严格模式可以避免对临时文件进行不必要的尝试，以及在下载后漏掉。  
3.如无必要，不要关闭“开始监听后解压已有压缩包”。正如名字所讲，开启该功能后可避免监听的文件夹内有未被解压的压缩包。  
4.默认显示的日志为精简日志，完整的日志在点击“显示完整日志”后会显示出来。精简日志可避免嗅探文件导致日志产生大量重复记录。  

常见用法：  
1.你需要不时下载一些数量较多、固定来源、固定密码的压缩包。直接下载到监听的文件夹中，可以避免反复点击解压，以及“我是不是漏包了”诸如此类的疑问  
2.你希望你的下载文件夹能自己把下载的压缩包解压出来，并且希望不要残留一堆不知道内容是什么的压缩包等着自己来清理  
3.你要处理数量众多的压缩包，有时候密码还各不相同，一个个点过去再输密码很麻烦  

English Version

注：英文版本的是机翻，以中文版本为准。如有表达问题欢迎指正！  
This English README is machine-translated. Please take the Chinese version as the standard. Corrections are welcome.

Preface: The author often needs to download archives from various "sites," which are usually encrypted. Downloading them one by one and manually extracting them is incredibly troublesome, so I developed this automation tool out of sheer frustration. This tool was created using Gemini 3. The author suffers from mild intellectual disability and is essentially illiterate or semi-illiterate. If you see any strange coding styles in the program, that is definitely my problem. If there are any incredibly stupid operations, please be sure to inform me via an issue. Thanks in advance to the experts for your guidance!

Note: You must have 7-Zip installed to use this program. Download it here: https://www.7-zip.org/. It is recommended to install it to the default path. If 7-Zip is installed in a non-standard location, you can modify the path in "Basic Settings."

Features:

Folder Monitoring: You can set a group of folder paths. Once monitoring starts, it automatically extracts the archive files inside.

Password Book: If you frequently download multiple archives with the same password, you can record common passwords in the password book. The program will automatically try them during the extraction process.

Smart Extraction: When an archive contains more than one file/folder, this feature automatically extracts all files into a separate folder to avoid scattering loose files. It is recommended to keep this enabled.

Threads: This setting controls the CPU threads used. If extraction is slow, you can increase this value, but it is not recommended to exceed your CPU's physical thread count.

Warnings:

The program is distributed as a folder. Do not move the .exe file out to run it separately, as all your configuration information is saved in a generated JSON file. If you run the .exe in isolation, you risk accidentally deleting the JSON file, resulting in the loss of all saved file paths and passwords.

Unless necessary, do not turn off "Strict Mode." When you use download tools like Baidu Netdisk or Aria2, they may create temporary files with archive extensions. Strict Mode prevents unnecessary attempts on these temporary files and ensures they aren't missed after the download completes.

Unless necessary, do not turn off "Extract existing archives after starting monitoring." As the name implies, enabling this feature ensures that no unextracted archives remain in the monitored folder.

The log displayed by default is a Simplified Log. The complete log is displayed only after clicking "Show Full Log." The simplified log prevents the log from being flooded with duplicate records caused by file sniffing.

Common Use Cases:

You occasionally need to download a large number of archives from fixed sources with fixed passwords. Downloading them directly into the monitored folder saves you from repeatedly clicking to extract them and eliminates doubts like "Did I miss a package?"

You want your download folder to automatically extract downloaded archives, and you don't want to be left with a pile of archives with unknown contents waiting for you to clean up.

You have to handle a vast number of archives, sometimes with different passwords, and clicking through them one by one to enter passwords is a hassle.

You have to handle a vast number of archives, sometimes with different passwords, and clicking through them one by one to enter passwords is a hassle.
