# 中山大学毕业论文/设计 LaTeX 模板（本科/研究生）（试用）

[![GitHub release](https://img.shields.io/github/release/1FCENdoge/SYSUThesis/all.svg)](https://github.com/1FCENdoge/SYSUThesis/releases/latest)
[![GitHub commits](https://img.shields.io/github/commits-since/1FCENdoge/SYSUThesis/latest.svg)](https://github.com/1FCENdoge/SYSUThesis/commits/main/)

本项目是中山大学的毕业论文/设计 LaTeX 模板 sysuthesis，基于中国科学技术大学学位论文LaTeX模板开发，兼容最新版的 TeX Live、MacTeX 、MiKTeX 发行版，支持跨平台使用。由于学校规定的研究生论文格式过于粗糙，部分格式参照中科大研究生论文格式进行设定。

注意：

1. 使用说明文档 `sysuthesis-guide.pdf` 在发布版中附带，用户也可自行编译；**使用模板前应仔细阅读**。

2. 本科论文模板格式参照计算机学院的模板，全校通用。研究生模板由于学校并无详细的规定，因此为试用模板，但已经得到下列学院支持：
   -[x]数学学院
   -[x]中法核工程与技术学院
   -[x]生命科学学院
   希望更多的院系能加入进来，做为中山大学研究生论文的共同标准。

3. 本模板要求 TeX Live、MacTeX、MiKTeX 不低于 2017 年的发行版，
并且尽可能升级到最新。安装和升级方法见
[新手指南](https://github.com/ustctug/ustcthesis/wiki/新手指南)（借用中科大LaTeX模板的wiki页面）。

4. **不支持** [CTeX 套装](https://github.com/ustctug/ustcthesis/wiki/常见问题#3-模板支持用-ctex-套装编译吗)。


## 下载地址

- GitHub Releases：<https://github.com/1FCENdoge/SYSUThesis/releases>

## 编译文档

- 编译模板的使用说明文档 `sysuthesis-guide.pdf`：
   ```
   latexmk -xelatex sysuthesis-guide.tex
   ```
- 编译论文 `main.pdf`：
   ```
   latexmk -xelatex main.tex
   ```
- 如需清理论文编译过程中的临时文件，可以：
   ```
   latexmk -c
   ```

- 以上编译过程也可以用 `make` 工具：
   ```
   make doc        # 编译生成 sysuthesis-guide.pdf
   make            # 编译生成论文 main.pdf
   make clean      # 删除编译过程中生成的临时文件
   ```

## 反馈问题

如果发现模板有问题，请按照以下步骤操作：

1. 阅读学校的标准，判断是否符合学校的要求；
2. 阅读 [常见问题 FAQ](https://github.com/ustctug/ustcthesis/wiki/常见问题)；
3. 将 TeX 发行版和宏包升级到最新，并且将模板升级到 Github 上最新版本，
查看问题是否已经修复；
4. 在 [GitHub Issues](https://github.com/ustctug/ustcthesis/issues)
中搜索该问题的关键词；
5. 在 [GitHub Issues](https://github.com/1FCENdoge/SYSUThesis/issues)
中提出新 issue，并回答以下问题：
    - 使用了什么版本的 TeX Live / MacTeX / MiKTeX ？
    - 具体的问题是什么？
    - 正确的结果应该是什么样的？
    - 是否应该附上相关源码或者截图？

如果导师或者院系在格式上有额外的要求，请将老师的邮件转发给模板作者。
作者会考虑增加接口以便修改格式。


## 更多资料

- [本科生论文规范](https://lingnan.sysu.edu.cn/undergraduateprogram/node/753)
- [研究生论文规范](https://graduate.sysu.edu.cn/sites/default/files/2019-04/%E4%B8%AD%E5%B1%B1%E5%A4%A7%E5%AD%A6%E7%A0%94%E7%A9%B6%E7%94%9F%E5%AD%A6%E4%BD%8D%E8%AE%BA%E6%96%87%E6%A0%BC%E5%BC%8F%E8%A6%81%E6%B1%82.pdf)
- [LaTeX 新手入门指南](https://github.com/ustctug/ustcthesis/wiki/新手指南)
- [常见问题 FAQ](https://github.com/ustctug/ustcthesis/wiki/常见问题)
- [参与开发](https://github.com/ustctug/ustcthesis/wiki/参与开发)
