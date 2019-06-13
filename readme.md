## 描述

《辐射小马国：粉色双眸》的重排版。

亦是本人对于文案「写作—排版—发布」工作流的一次尝试。

## 项目结构

- readme.md
- main.tex
- struction.tex
- chaps
    - cover.tex
    - copyright.tex
    - preface.tex
    - chap01.tex
    - ...
    - chap20.tex
    - afterword.tex
    - acknowledgement.tex
- main.pdf
    - 文档输出
- archive
    - 原始排版存档

## TODO & Issues

### 已知问题

- 标点避头尾
- 楷体字体标点压缩不正确

### 是否需要？

- 在每一个时间地点处换页
- 版心重新制作
- 将所有英文专有名词放入注释中
- 字体穿透数学公式

### 需要检查

- 是否有侵权内容
    - 分隔线图片
    - 字体
- 确定各样式


### TODO

- 封面设计


## 协议

由于涉及著作权，本文档并非完全开源，请勿商用。

详情见版权页。


## 编译环境

- TeX Live 2019
- XeLaTeX
- 额外字体
    - Noto Serif CJK SC
    - Noto Sans CJK SC

## 存档

### 正则表达式

```
\\textbf{第(\w+)天}\n\n\\textbf{大约时间：(.+)}\n\n\\textbf{地点：(.+)}
\\daytimeplace{$1}{$2}{$3}{}
 
(:\w\w)([AP]M)
$1 $2
 
\includegraphics[width=2.4in,height=0.31944in]{media/image3.png}
\\includegraphics\[.+\]{media/image3\.png}
\\horizonline

(\w)’
$1'
```

### 文案编辑

- 呯 -> 乒
- 艹 -> 肏

具体部分修改见注释。





