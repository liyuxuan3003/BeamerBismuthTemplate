# BeamerBismuthTemplate

BeamerBismuthTemplate是一个开箱即用的LaTeX模板，适用于幻灯片，基于自定义文档类`beamer-bismuth`和自定义宏包`minimus`。

BeamerBismuthTemplate是LumosLaTeX计划的一部分：https://github.com/liyuxuan3003/LumosLaTeX

https://github.com/liyuxuan3003/BeamerBismuthTemplate.git

## 引入方式

克隆模板仓库

```bash
git clone git@github.com/liyuxuan3003/BeamerBismuthTemplate.git
```

初始化项目

```
cd BeamerBismuthTemplate
./init.sh MyProject
```

初始化会自动完成项目重命名、子模块加载、移除模板的远程引用等操作，只能执行一次。

## 目录结构

项目的目录结构如下

```
BeamerBismuthTemplate   # The root of git repo
|- .git
|- MyProject            # The sub dir of source files (run make here!)
.  |- build/
.  |- makefile-latex/
.  |- minimus/
.  |- pyjool
.  |- beamer-bismuth/
.  |- standalone-silicon/
.  |- Makefile
.  |- MyProject.tex
.  |- Section01.tex
.  |- Section02.tex
.  |- Section03.tex
.  |- Section04.tex
.  |- TextA.fig.tex
.  |- TextB.fig.tex
.  |- Reference.bib
|- .gitignore
|- .gitmodules
|- init.sh
|- README.md
|- BeamerBismuth.md
```

请注意，根目录下仅有`.gitignore`和`README.md`等文件，代码均位于一个二级目录下！

## 构建方式

模板提供`Makefile`进行编译，任何`make`命令都需要在二级目录下运行。

编译文档及其插图

```bash
make -j
```

清理文档输出目录

```bash
make clean
```

## 子模块

模板的具体使用方式，请参见各个子模块的文档。

| 子模块 | 文档 |
|--------|------|
| `minimus` | [README](Beamer/minimus/README.md) |
| `beamer-bismuth` | [README](Beamer/beamer-bismuth/README.md) |
| `standalone-silicon` | [README](Beamer/standalone-silicon/README.md) |
| `makefile-latex` | [README](Beamer/makefile-latex/README.md) |
| `pyjool` | [README](Beamer/pyjool/README.md) |
