# simple-java-projs
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;这个仓库用于汇集学习过程中的一些java基础语法和进阶语法，然后由团队合作写项目，balabala，其实我也不会说什么，但大致就是这样的。

## 具体要做些什么呢？
1. 大佬们可以将想要实现的项目push到本仓库，具体方式如下：<br>
    第一步：fork本仓库
    ![fork教程](img/how-to-fork.png)
    第二步：克隆到本地
    ```shell
    git clone https://github.com/xxx/simple-java-projs.git
    # 这里的xxx是你的GitHub用户名
    ```
    第三步：在克隆得到的项目中，增加你自己项目的文件，并通过markdown文件阐述你的想法，比如你想要实现的功能。最终上传到本仓库，具体方式如下：<br>
    ```shell
    git add ./myproj
    git commit -m "这是我的项目，希望大佬们可以帮我实现xxx功能，功能具体内容，请查看项目中的markdown文件。谢谢！"
    git push
    ```
    第四步：在GitHub中发起合并请求，我会不定期查看，然后判断通过与否
### 关于如何对自己的项目进行基础push操作，可以参考下面的图片
![推送测试](img/how-to-push.png)

2. 上传已有的项目代码到这个项目，然后指出在实现过程中，你用到的语法和思路，说说遇到的bug以及修bug的思路和方案

例如这样

`除0异常`
```java
int a = 1;
int b = 0;
// 这行代码报错，导致程序不正常退出
System.out.println(a / b);
```
`解决方案`

通过简单的逻辑判断语句，在执行这条语句之前，判断除数是否为0，
```java
int a = 1;
int b = 0;
if (b != 0) System.out.println(a / b);
else throw new ArithmeticException("除数b="+b);

```
然后根据实际情况编写后续代码

3. 如果你的项目存在bug，或者你在实现项目的时候，对于java的类和方法有不懂的，也可以在这里提出，比如：<br>
> “我不知到在读取用户输入的时候，Scanner和BufferedReader两个类有什么区别，建议用哪一个好？”
---
## 项目链接
markdown功能强大，支持超链接，能够表示图片、视频、音频、markdown等文件，能够在一份markdown文件中，包含其他的markdown文件，具体方式如下：
```markdown
[markdown文件名](markdown文件链接)
```
示例为example项目下的readme.md：
[readme.md](example/readme.md)

鼠标放置在超链接上，按下ctrl在点击鼠标左键，就可以跳转到example目录下的readme.md文件。

由此，这一部分区域将用于展示这个仓库有什么项目。

1. [简单udp聊天程序](simpleChatter/README.md)
2. 待更新

最终项目目标：前后端分离的，类似百度网盘的伟大项目。（目前思路：无）

---
<!-- &nbsp;是html的空格符，这里使用它，是因为我需要缩进来保持美观 -->
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;这一份markdown文件是我用了半个晚上写出来的，我以前其实并没有写过类似这种提议，所以会有疏漏和不足，但是这个项目是开放的，所以大佬们有什么建议，可以向本项目发起issue，所有参与这个项目的人都能看到这个issue，根据实际情况，这个issue会得到不同参与者的赞同或反对，但无论如何，你的issue都会得到考虑，也有可能会最终并入这个项目，因此，希望各位能多多提issue。<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;实际上，GitHub上的开源项目也是找工作的有力助手，你若是有强力的opensource项目，这个项目得到了多少star，多少会对找工作有点帮助，这似乎是国内公司普遍关注的。使用GitHub进行开源项目的实现，也有利于你对GitHub的使用。