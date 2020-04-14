# Introduction

Markdown 是 John Gruber 发明的一种轻量级标记语言，具有轻量化、易读易写特性，并且对于图片，图表、数学式都有支持。当前许多网站广泛使用 Markdown 来撰写文档。此外，Markdown 亦可以用于简单地编辑结构化的文章。

> 以下介绍的 Markdown 以 GitHub Flavored Markdown 为主体

## 示例

### 标题

```markdown
# h1

## h2

### h3

#### h4

##### h5

###### h6
```

# h1

## h2

### h3

#### h4

##### h5

###### h6

### 文本

```markdown
_Italic_
_Italic_

**Bold**
**Bold**

`code`

---

> ref

> ref
>
> ref
```

_Italic_
_Italic_

**Bold**
**Bold**

`code`

---

> ref

> ref
>
> ref

### 列表

> 对于无序列表，`+`、`-`、`*`等价

```markdown
- 张三

* 李四
  - 王五 -赵六
```

- 张三

* 李四
  - 王五
    - 赵六

```markdown
1. Hello
2. World
3. !
```

1. Hello
2. World
3. !

```markdown
TODO List

- [ ] TODO 1
- [ ] TODO 2
  - [ ] TODO 2.1
  - [x] TODO 2.2
```

TODO List

- [ ] TODO 1
- [ ] TODO 2
  - [ ] TODO 2.1
  - [x] TODO 2.2

### 表格

```markdown
| col1 | col2 | col3 |
| :--- | :--: | ---: |
| 1    |  1   |    1 |
```

| col1 | col2 | col3 |
| :--- | :--: | ---: |
| 1    |  1   |    1 |

### 链接

```markdown
[Markdown By JOHN GRUBER](https://daringfireball.net/projects/markdown/)
![example pic]()
```

[Markdown By JOHN GRUBER](https://daringfireball.net/projects/markdown/)
![example pic]()

### 代码块

````markdown
```python
print("hello world")
```
````

```python
print("hello world")
```

---

## More Reference

> [GitHub Flavored Markdown Spec](https://github.github.com/gfm/)
>
> [Markdown Reference by typora](http://support.typora.io/Markdown-Reference/)
