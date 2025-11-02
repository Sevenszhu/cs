# latex

## 1. 文本格式化和创建宏

### 创建具有标题的文档

```latex
\document[a4paper]{article}

\title{Example}
\author{My name}
\date{May 5, 2021}

\begin{document}

\maketitle

\section{What's this}
This is a document.
\end{document}
```

### 文档结构

- 诸如`\documentclass` 之类的以反斜杠开头的词，被称为命令或宏。
  - 诸如`\title, \author, \date` 这种命令储存了属性，但是并不打印内容。

- 文档的第一个部分被称为序言，通常在这里选择类、指定属性，并对整篇文档进行定义。
- `\begin{document}` 标志着序言的结束和正文的开始。`\end{document}` 标志着文档结束，该命令后的所有命令都会被latex忽略。通常，这样一段由`\begin` 和`\end` 命令构成的代码叫做环境。
- 实际文档中使用了`\maketitle` 命令，它以一种优雅的样式打印标题作者和日期。
- 使用`\section` 命令创建了小标题，它比普通文本字体更大更粗。
- 然后输入一些文字。
- 序言之后的内容都位于文档环境之内，将被打印出来。序言本身并不生成**任何**输出。