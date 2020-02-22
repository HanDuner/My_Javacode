# The door of Git 

**注：[参考地址1](https://blog.csdn.net/qq_41961239/article/details/103935110)、[参考地址2](https://www.bilibili.com/video/av75718460?p=16)**

**编写于2020.2.21**

## 1. Git与Github

### 1.1 两者区别

- Git是一个分布式版本控制系统，简单的说其就是一个软件，用于记录一个或若干文件内容变化，以便将来查阅特定版本修订情况的软件。
- [GitHub](https://www.github.com)是一个为用户提供Git服务的网站，简单说就是一个可以放代码的地方（不过可以放的当然不仅是代码）。Github除了提供管理Git的web界面外，还提供了订阅、关注、讨论组、在线编辑器等丰富的功能。Github被称之为全球最大的基友网站。

### 1.2 Git安装

- 下载得到安装包，并运行
- 选择软件的安装位置
- 选择需安装的组件(默认即可，直接下一步)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111120951139.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

- 选择使用的编辑器(默认即可，直接下一步)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111120948182.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

- 环境变量调节

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121002699.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

- 使用OpenSSH，直接下一步即可

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121004715.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

- 使用OpenSSL库

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121011317.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

- 配置命令行会话（默认即可）

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121015551.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

- 配置终端（默认即可）

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121012552.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

- 配置额外的选项（默认即可）

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121018751.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121039946.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

- 安装完成

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121035841.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

- 测试：在桌面空白处右键鼠标，若出现“Git GUI Here”、“Git Bash Here”则安装成功。

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121032293.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

## 2. Git的使用

### 2.1 本地仓库

#### 2.1.1 工作流程

- Git本地操作的三个区域：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121410708.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

- 流程：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121415548.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

#### 2.1.2 本地仓库操作

什么是仓库呢？仓库又名版本库，英文名Repository，我们可以简单理解成是一个目录，用于存放代码的，这个目录里面的所有文件都可以被Git管理起来，每个文件的修改、删除等操作Git都能跟踪到。

- 在安装好后首次使用需要先进行全局配置
  桌面空白处右键，点击“Git Bash Here”以打开Git命令行窗口

- ```java
  $ git config --global user.name "用户名"
  $ git config --global user.email "邮箱地址"
  ```
```
  

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121538823.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

#### 2.1.3 创建仓库(库的位置都可以)

当我们需要让Git去管理某个新项目/已存在项目的时候，就需要创建仓库了。注意，创建仓库时使用的目录不一定要求是空目录，选择一个非空目录也是可以的，**但是不建议在现有项目上来学习Git，否则造成的一切后果概不负责！**

**注意**：为了避免在学习或使用过程中出现各种奇葩问题，请不要使用包含中文的目录名（父目录亦是如此）。

- 创建空目录(可以使用mkdir也可以直接右键创建 )

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121849985.png)

- 在命令行中进入项目目录pro_git

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111121910369.png)

- Git仓库初始化（让Git知道，它需要来管理这个目录）指令：git init

![在这里插入图片描述](https://img-blog.csdnimg.cn/2020011112192465.png)

**表现：执行之后会在项目目录下创建“.git”的隐藏目录，这个目录是Git所创建的，不能删除，也不能随意更改其中的内容。**

#### 2.1.4 Git常用指令操作

##### 2.1.4.1 查看当前状态：git status 【非必要】

##### 2.1.4.2 添加到缓存区：git add 文件名

##### 2.1.4.3 提交至版本库：git commit -m “注释内容”

​```java
说明：git add指令，可以添加一个文件，也可以同时添加多个文件。
语法1：git add 文件名
语法2：git add 文件名1 文件名2 文件名3 …
语法3：git add .					【添加当前目录到缓存区中】
提交至版本库：git commit -m “注释内容”
```

**在后续对于文件（可以操作1个或多个）操作之后，重复使用git add与git commit指令即可。**

##### 2.1.4.4 时光穿梭机——版本回退

- 版本回退分为两步骤进行操作：

```java
步骤：
	①查看版本，确定需要回到的时刻点
			指令：
				git log
				git log --pretty=oneline //常用这种
	②回退操作
			指令：
				git reset --hard 提交编号

```

案例：想坐时光机回到创建好第一个文件readme.txt的时候。

![在这里插入图片描述](https://img-blog.csdnimg.cn/2020011112221675.png)

注意：回到过去之后，要想再回到之前最新的版本的时候，则需要使用指令去查看历史操作，以得到最新的commit id。
指令：git reflog

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111122301534.png)

**小结：**

> a. 要想回到过去，必须先得到commit id，然后通过git reset –hard 进行回退；
>
> b. 要想回到未来，需要使用git reflog进行历史操作查看，得到最新的commit id：
>
> c. 在写回退指令的时候commitid可以不用写全，git自动识别，但是也不能写太少，至少需要写前4位字符；

### 2.2 远程仓库

线上仓库的操作以Github为例

#### 2.2.1 线上仓库创建

打开创建仓库页面：[https://github.com/new](https://github.com/new)

圈出的部分为必填项，其余根据实际需要选择性补充：

![在这里插入图片描述](https://img-blog.csdnimg.cn/2020011112245485.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

**注意：仓库名要求在当前帐号下唯一。**

#### 2.2.2 两种常规使用方式

##### 2.2.2.1 基于http/https协议

- 创建空目录，名称就称为shop

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111122527910.png)

- 使用clone指令克隆线上仓库到本地

  语法：git clone 线上仓库地址

  ![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111122548688.png)

- 在仓库上做对应的操作（提交暂存区、提交本地仓库、提交线上仓库、拉取线上仓库）
  提交到线上仓库的指令：git push

  ![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111122604970.png)

  第一次需要登录Github

  再次尝试push指令：

  ![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111122701755.png)

  如果看到类似上述效果（没有fatal错误）则表示提交成功。

  【验证】此时可以观察浏览器，刷新线上仓库的地址：

  ![在这里插入图片描述](https://img-blog.csdnimg.cn/202001111227167.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

  拉取线上仓库：git pull

  ![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111122726209.png)

  **提醒：在每天工作的第一件事就是先git pull拉取线上最新的版本；每天下班前要做的是git push，将本地代码提交到线上仓库。**

##### 2.2.2.2 基于ssh协议（推荐）

该方式与前面https方式相比，只是影响github对于用户的身份鉴权方式，对于git的具体操作（如提交本地、添加注释、提交远程等操作）没有任何影响。

- 生成公私玥对指令

  实际操作：

  - 打开提示

    ![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111122813166.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

  - 创建公私玥对文件

    ![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111122830839.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

  - 上传公钥文件内容（id_rsa.pub右键记事本打开）

    填入Github中保存即可。

  - 执行后续git操作，操作与先前一样

    - clone线上仓库到本地（git clone）

      ![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111122911169.png)

    - 修改文件后添加缓存区、提交本地仓库、提交线上仓库

      ![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111122944145.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

- 在push的时候并没有提示要求我们输入帐号密码，因为公私玥已经实现了用户身份鉴权。

  线上仓库的效果：

  ![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111122959222.png)

## 3. 分支管理

### 3.1 什么是分支？

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123032768.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

在版本回退的章节里，每次提交后都会有记录，Git把它们串成时间线，形成类似于时间轴的东西，这个时间轴就是一个分支，我们称之为master分支。
在开发的时候往往是团队协作，多人进行开发，因此光有一个分支是无法满足多人同时开发的需求的，并且在分支上工作并不影响其他分支的正常使用，会更加安全，Git鼓励开发者使用分支去完成一些开发任务。

### 3.2 分支的常用命令

```java
分支相关指令：
查看分支：git branch
创建分支：git branch 分支名
切换分支：git checkout 分支名 
删除分支：git branch -d 分支名
合并分支：git merge 被合并的分支名

```

#### 3.2.1 查看分支：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123050384.png)

注意：当前分支前面有个标记“*”

#### 3.2.2 创建分支：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123100378.png)

#### 3.2.3 切换分支：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123146370.png)

#### 3.2.4 合并分支：

现在先在dev分支下的readme文件中新增一行并提交本地

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123210116.png)

切换到master分支下观察readme文件

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123243161.png)

将dev分支的内容与master分支合并

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123319287.png)

#### 3.2.5 删除分支：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123333865.png)

**注意：在删除分支的时候，一定要先退出要删除的分支，然后才能删除。合并所有分支之后，需要将master分支提交线上远程仓库中**

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123401710.png)

## 4. 冲突的产生与解决

案例：模拟产生冲突。

同事在下班之后修改了线上仓库的代码

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123407956.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

注意：此时我本地仓库的内容与线上不一致的

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123426454.png)



第二天上班的时候，我没有做git pull操作，而是直接修改了本地的对应文件的内容

![在这里插入图片描述](https://img-blog.csdnimg.cn/2020011112343821.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

需要在下班的时候将代码修改提交到线上仓库（git push）

![在这里插入图片描述](https://img-blog.csdnimg.cn/2020011112345830.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)



提示我们要在再次push之前先git pull操作。

**【解决冲突】**

- 先git pull

  ![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123525479.png)

  此时git已经将线上与本地仓库的冲突合并到了对应的文件中。

- 开冲突文件，解决冲突
  解决方法：需要和同事（谁先提交的）进行商量，看代码如何保留，将改好的文件再次提交即可。

  ![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123544221.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)

- 重新提交

  ![在这里插入图片描述](https://img-blog.csdnimg.cn/2020011112355714.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)



线上效果：

![在这里插入图片描述](https://img-blog.csdnimg.cn/20200111123607461.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxOTYxMjM5,size_16,color_FFFFFF,t_70)



**新手上路小技巧：上班第一件事先git pull，可以在一定程度上避免冲突的产生。**

