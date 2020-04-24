# Install LaTeX

![](https://img.shields.io/badge/Unfinished-helpNeed-red)

## TeX Live

## VSCode

### 插件 LaTeX Workshop

需要编译内容包含中文的文档，建议使用 XeLaTeX 进行编译，仿照下方更改插件设置：

```json
"latex-workshop.latex.recipes": [
  {
    "name": "xelatex",
    "tools": ["xelatex"]
  },
  {
    "name": "xelatex -> bibtex -> xelatex",
    "tools": ["xelatex", "bibtex", "xelatex", "xelatex"]
  }
],
"latex-workshop.latex.tools": [
  {
    "name": "xelatex",
    "command": "xelatex",
    "args": [
      "-synctex=1",
      "-interaction=nonstopmode",
      "-file-line-error",
      "%DOCFILE%"
    ]
  },
  {
    "name": "bibtex",
    "command": "bibtex",
    "args": ["%DOCFILE%"]
  }
]
```

这两段分别制定使用什么工具进行编译，和编译顺序。

> 这里使用`%DOCFILE%`可以保证在中文路径下的`tex`文件能正确编译。但在 Windows 上如果不设置 UTF8 支持，目前编译**中文文件名**的文件似乎仍有问题。
