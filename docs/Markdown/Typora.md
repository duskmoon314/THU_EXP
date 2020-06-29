# Typora 使用指南

## 简单介绍

- 轻量
- 所见即所得
- 支持基本 $\LaTeX$
- 支持 Mermaid
- 支持高亮和表情
- 支持更改主题
- 使用 Pandoc 转换成各种格式

## 安装使用

从官网上下载对应OS的版本，然后一路`next->install->finish`就安装完成了

此处提供官网下载地址如下：

> [Download Link](https://www.typora.io/#)

### 基本操作

打开Typora的初始界面是这样的：

![Initial](/assets/images/Typora_01.png)

界面主要构成如下：

顶部是**菜单**栏目，左侧边栏是**文件**和**内容大纲**栏目，底栏左侧有**显示/隐藏侧边栏**和**启用源代码模式**两个选项，右侧有**拼写检查**和**字数统计**两项功能

#### 菜单介绍

1. 文件菜单

    ![File](/assets/images/typora_02.png)

    其中的基本功能，新建、新建窗口、打开、打开文件夹、快速打开、打开最近文件、保存、另存为、保存全部打开的文件、导入、导出、打印、关闭等基本功能与常用软件相仿，此处不再赘述。偏好设置即Typora的设置，具体包括5个部分——通用、外观、编辑器、图像、Markdown：

    ![Settings](/assets/images/typora_03.png)

    通用部分主要包括一些基本的设置特别是语言、检查更新等设置。

    ![Appearance](/assets/images/typora_04.png)

    外观部分就是对于Typora样式的一些调整

    ![Editor](/assets/images/typora_05.png)

    编辑器部分主要就是对于相关的编辑选项的一些设置，主要包括换行符、缩进和拼写检查等内容

    ![Images](/assets/images/typora_06.png)

    图像部分主要就是对于你通过Typora插入的图片进行何种操作的一个设置部分，一般来说，正常使用只要在插入图片时选择无特殊操作即可，如果自己有使用现成的图床，则可以配合PicGo直接将插入的图片进行上传至对应图床的操作，从而加强文档的通用性和易迁移性。如需使用，建议直接下载安装PicGo，安装对应插件（如果需要），并按要求完成配置，然后在Typora中图像部分，将插入图片时后的选项改为上传图片，并在下方选在PicGo及其对应的路径位置，也可按自己的需求选择PicGo核心的命令行来支持上传服务

    ![Markdown](/assets/images/typora_07.png)

    最后的Markdown部分，主要是对于一些markdown语法等个性化的设置，可以根据自己的需求进行相关调整

2. 编辑菜单

    ![Edit](/assets/images/typora_08.png)

    编辑菜单中主要就是一些常规的对于文本的相关操作

3. 段落菜单

    ![Passage](/assets/images/typora_09.png)

    段落菜单主要可以为不熟悉Markdown的朋友提供方便快捷的段落布局等的格式标记

4. 格式菜单

    ![Fromat](/assets/images/typora_10.png)

    格式菜单主要可以为不熟悉Markdown的朋友们提供关于内容和样式等方面的一些格式标记

5. 视图菜单

    ![View](/assets/images/typora_11.png)

    视图菜单主要是管理当前Typora显示的栏目情况和样式等

6. 主题菜单

    ![Theme](/assets/images/typora_12.png)

    主题菜单主要是用于切换你已安装的Markdown的主题（安装新主题可见后文）

7. 帮助菜单

    ![Help](/assets/images/typora_13.png)

    帮助菜单就是一些和Typora相关的信息

### 添加新的主题

点击**帮助**菜单中的`更多主题`进入Typora的support界面，找到对应的Theme栏目，或直接进入Typora的[主题画廊](http://theme.typora.io/)，界面如下：

![Theme-gallery](/assets/images/typora_14.png)

挑选一个你感兴趣/喜欢的主题，如以`OneDark`为例：

![OneDark](/assets/images/typora_15.png)

进入到对应的下载界面进行下载

然后在文件->偏好设置->外观中，点击`打开主题文件夹`这一按钮，将下载下来的内容直接全部解压到这一文件夹中，如下：

![Add-Theme](/assets/images/typora_16.png)

随后重启Typora即可看到对应的主题：

![New-theme](/assets/images/typora_17.png)
