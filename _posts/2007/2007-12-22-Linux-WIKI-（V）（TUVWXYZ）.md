---
layout: post
title: Linux WIKI （V）（TUVWXYZ）
categories:
- Diandian
tags:
- Linux

---
T
<br />
<br />Tarballs
<br />
<br />Many pieces of software for Linux don't come in precompiled form, but rather as a bundle of
<br />
<br />source code files. These files are appended one to another (with the tar utility) and zipped
<br />
<br />(compressed) with gzip. Their names are often &quot;hop.tar.gz&quot; or &quot;hop.tgz&quot;
<br />许多Linux软件都没有以预编译的形式出现，而是以源代码文件包的形式。这些文件打包
<br />
<br />到一个文件中（通过tar工具）并用gzip打包（压缩）。它们的名字通常
<br />
<br />是&quot;hop.tar.gz&quot;或&quot;hop.tgz&quot;。
<br />
<br />In order to install these programs one needs to unpack them (unzipping and un-tarring) and often to
<br />
<br />compile them. GNU compliant software is usually easy to compile.
<br />为了安装这些程序，一是需要解包（unzipping and un-tarring）同时通常还需要编译它们。
<br />
<br />GNU相关软件通常可以很容易进行编译。
<br />
<br />Always read the README file before doing anything other than unpacking!
<br />在解包后最好做其他任何事之前，读一下README文件。
<br />
<br />U
<br />
<br />UID, SetUID
<br />
<br />A number representating a user. The root user's UID is 0. A program is usually run under the UID
<br />
<br />of the person who executes it (emacs, gcc, vi) except those that need to do special things (passwd,
<br />
<br />chsh) that are run as setUID root. These are the programs that are allowed to do things that only
<br />
<br />root is allowed to do, such as changing a password, or writing things to the screen of everyone on
<br />
<br />the system. These programs must be kept to a few because of the security risk that they represent.
<br />代替一个用户的数字。根用户的UID是0。程序通常在执行该程序（emacs, gcc, vi)的用户
<br />
<br />UID下运行，除非该程序需要通过设置根用户UID（即SetUID）来运行一些特定的任务
<br />
<br />（passwd, chsh）。也有些程序被允许做一些只有根用户才能被允许做的事，如改变密码或
<br />
<br />将系统上每个人的屏幕上写东西。正如它所描述的那样，出于安全考虑这些程序必须只能
<br />
<br />保留少量。
<br />
<br />Owner
<br />
<br />The user with individual permissions to a file or directory. By default, the owner is the user who
<br />
<br />originally created the file, but it can be changed to someone else with the chown command.
<br />对一个文件或目录拥有独立权限的用户。一般来说所有者是始建文件的用户，但它也可以
<br />
<br />通过chown命令改成其它人。
<br />
<br />See Also access permissions, chown.
<br />参见access permissions, chown
<br />
<br />Unicode
<br />
<br />It's quite obvious that 8-bit ASCII can't be used to represent all the possible characters in the world
<br />
<br />(think of the chinese ideograms !). So a new encoding has been devised, called Unicode, with
<br />
<br />enough room for all possible characters of all existing languages (sort of).
<br />8位ASCII字符并不能表示世界上所有可能的符号（如中国的表意文字），这是十分明显的
<br />
<br />。所以一个新的编码被设计同来，叫Unicode。它有足够的位置来表示所有存在语言的全
<br />
<br />部可能的字符。
<br />
<br />W
<br />
<br />Wildcard
<br />
<br />A special regular expression, noted * , the wildcard is expanded to any and all possible values.
<br />特点的规则表达式，如著名的*，通配符可以表示任意或全部可能的值。
<br />
<br />* means all possible values, hop* means all values that start by &quot;hop&quot;, and so on...
<br />* 可以表示所有可能的值，hop*表示以hop开始的所有值，诸如此类...
<br />
<br />Window Manager
<br />
<br />see X
<br />参见X
<br />
<br />X
<br />
<br />Extensible Markup Language
<br />
<br />A widely-used data representation format.
<br />一种被广泛使用的数据表示形式。
<br />
<br />See Also Standard Generalized Markup Language.
<br />参见Standard Generalized Markup Language
<br />
<br />X
<br />
<br />aka &quot;The X Window System&quot;
<br />也称为“X窗口系统”
<br />
<br />and many other (more or less correct) names (but don't just say 'Windows', argh...)
<br />还有许多其他（基本上都算正确）的叫法（但不会被叫成“Windows”，argh...）
<br />
<br />It is the system that is used to display graphical things on the screen.
<br />这是一种被用来在屏幕上显示图形事物的系统。
<br />
<br />An X server waits for &quot;events&quot; such as motion from the mouse, keypresses... It can then send this
<br />
<br />information to X clients such as Xterm, xv, that may run on different computers.
<br />X服务器等待“事件”的发生，如监视鼠标，击键...等。然后它将该事件的信息发送给X客
<br />
<br />户端，如Xterm，xv等，这些客户端也可以运行在其他计算机上。
<br />
<br />The way an X display looks like is set by a window manager whose job is to, ahem, manage your
<br />
<br />windows and their look. Smile (Borders, background image...)
<br />X显示的方式看上去象是被窗口管理器所设置，该管理器的任务就是管理你的窗口和它们
<br />
<br />的外观。Smile（边界，背景图片...）
<br />
<br />Y
<br />
<br />YMMV
<br />
<br />Your Mileage May Vary
<br />此法对你可能不灵
<br />
<br />Z
<br />
<br />Zip
<br />
<br />Usually, large files (or group of files) are compressed in order to save disk space. The most widely
<br />
<br />found standard is &quot;zip&quot;.(winzip in Windows(r), gzip in Unix), these standards are two versions of an
<br />
<br />old algorithm called Lempel-Ziv (LZ)(1977).
<br />通常压缩大文件（或一组文件）是为了节省磁盘空间，大多数人广泛使用的创建标准是“
<br />
<br />zip”（Windows下是winzip，Unix下是gzip）。这些标准其实是一个叫Lempel-Ziv(LZ)(1997)
<br />
<br />老算法的两个版本。
<br />
<br />In Unix, zipped files usually bear the extension .gz (sometimes .tgz see Tar), use gzip file to zip
<br />
<br />(compress) and gunzip file to unzip (decompress).
<br />在Unix下，zipped文件通常后缀名是.gz（有时是.tgz，参见Tar），使用gzip文件去zip（压缩
<br />
<br />）并用gunzip文件去unzip（解压）。