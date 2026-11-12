# 华南理工大学硕/博士课程论文 LaTeX 模板

按研究生院现行《研究生课程论文》Word 模板更新。首页、说明和正文示例与官方模板一致。模板参考了 [maoruimas](https://www.cnblogs.com/maoruimas/p/12774996.html) 和 [mengchaoheng/SCUT_course](https://github.com/mengchaoheng/SCUT_course)。

## 编译

只用 **XeLaTeX** 编译 `main.tex`，参考文献用 **Biber**。不要用 PDFLaTeX，也不要选 BibTeX。

VS Code 或 Cursor 请打开本目录，让 LaTeX Workshop 读到 `.vscode/settings.json`。默认配方是 **`xelatexmk`**（即 `latexmk -xelatex`）。命令面板里选 Build LaTeX project 即可。

命令行在本目录执行：

```bash
latexmk -xelatex main.tex
```

TeXstudio：Default Compiler 选 XeLaTeX，Default Bibliography Tool 选 Biber。

macOS 上若 `biber` 报 `extracting arm64 binary with lipo failed`，本仓库的 `.latexmkrc` 会改用 `bin/biber`，无需再改系统。

## 填写

封面字段在 `main.tex` 顶部。正文示例在 `body.tex`：先是硕士页，后是博士页。蓝色字是格式说明，正式提交时删除，并只保留硕士或博士其中一页。
