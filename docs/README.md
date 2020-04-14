# THU_EXP

本项目由 duskmoon 发起，旨在构造一套完整的工具链进行各实验课（e.g. 大物实验、电子电路与系统基础实验）的数据处理和报告撰写

项目基于 python（使用库 numpy、matplotlib、jupyter 等）、Excel、$\LaTeX$、Markdown 等。

## How to use

### 对 python 部分

目前使用的是 3.7.2，不过除了依赖外，与版本的相关性应不大。

1. clone 本项目到本地，在文件夹中创建 python 的虚拟环境，并安装相关依赖（见`tools/Python/requirements.txt`）
   可以参考 python 官网的虚拟环境创建，或者使用 conda
2. 激活虚拟环境，启动 `jupyter notebook`
3. 在弹出的浏览器窗口查看相关 `notebook`

### 对 $\LaTeX$ 报告模板

目前给出的模板是用`texlive2019`制作的，并使用`xelatex`生成 pdf。我目前无法给出更多的可用性保证。

### 对 Excel 部分

由于部分实验（e.g. 大物实验）给出了 Excel 的例子，便直接采用了。出于某些原因，保留一份`Excel使用指南.md`或是最低需要。

### 对 `tools/themes/Markdown` 部分

用于存放 Markdown 导出 PDF 时候控制主题的 CSS 文件等。

来源：

- https://github.com/CowAndSheep/Beautiful-css

## Wiki

Wiki 地址：[传送门](https://duskmoon314.github.io/THU_EXP)

- [ ] LaTeX
  - [ ] Introduction
  - [ ] Install (texlive + vscode + LaTeX Workshop)
  - [ ] Cheatsheet
- [ ] Markdown
  - [x] Introduction
  - [ ] Install (vscode / typora)
  - [ ] PlantUML
- [ ] Python
  - [ ] Introduction
  - [ ] Install (Python + vscode, numpy + matplotlib + jupyter)
  - [ ] Cheatsheet
- [ ] Excel
  - [ ] Introduction
  - [ ] Cheatsheet
- [ ] VSCode
  - [ ] Verilog Format
  - [ ] verilog-formatter
  - [ ] LaTeX Workshop
  - [ ] Markdown PDF

## TODO

- 加入实验内容
- 脱离 python 使用
- 完善文档内容

## How to contribute

我们欢迎任何同学为这个库添加新的内容，只要你认为有必要

- 有关修改的内容

  - 将你想要提交的内容写在已有的（如果需要增加内容）或者全新的`ipynb`文件（即 jupyter notebook）/ `md`文件（即 Markdown）
  - 在提交前对内容的正确性进行了验证
  - 尽量提高**可读性**

- 有关提交方式
  - 任何从 fork 的 master 提起的 pr **不被接受**，你总应该在一个单独的 branch （以一个与这个 pr 相关的名称命名）进行修改，commit，和提起 pr。这是因为当你一旦提交 pr，通过继续向提交 pr 的那个 branch push commit，你可以持续地更新这个 pr。如果你使用 master 提交，而你之后一旦修改了 master，无论是否和这个 pr 相关，所有的更改也会提交到这个 pr。
  - PR 的名称能够体现出更改的含义。
  - PR 所包含的 commits 的 message 需要体现出各个 commit 作出的更改。
  - 在 PR 的文本框内，使用 Markdown 简单地介绍一下更改的内容等等，没有长度要求，只是说在这里写清楚 pr 的目的能够更好地让 reviewer 初步判断你的想法。
