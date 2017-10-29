# comtrade

包含comtrade解析模块和comtrade解析工具。

### 依赖

基于python3开发

依赖模块：

- matplotlib
- numpy

安装依赖：

```
pip3 install matplotlib numpy
```

### 文件说明

- **comtrade**: comtrade文件解析工具，是命令行工具，传入参数为comtrade的cfg文件或者dat文件；
- **comtrade.py**: comtrade解析模块，包含解析comtrade文件需要的类，使用方法参考 [comtrade](./comtrade) 的内容；

### 命令行工具功能

可以转换(并显示)comtrade波形文件，支持转换指定目录下的多个波形文件。帮助信息：

```sh
➜  wave-guangxi comtrade -h

comtrade can convert comtrade files to pic file or csv data file. The tool can also show the wave figure. Addionally, It can convert multiple files in the dir.

Usage:
  comtrade [options [args]] [file/dir]

options:
  -h: print the help infomation
  -s: show the figure window
  -f: set the file format convert to, with args specifying file format

args:
  format: pdf, png, eps, svg, ps, csv

file/dir:
  file: specify a couple of comtrade files
  dir: specify a direction, convert the files in the direction

Default:
  default format is pdf.

Example:
  comtrade -f png xxx.cfg
```

#### comtrade文件解析

- [x] 解析二进制的dat文件
- [ ] 解析文本的dat文件

#### 需要实现

- [x] 支持导出波形矢量图或位图文件
- [x] 支持转换为csv文件
- [x] 支持显示波形窗口
- [x] 支持转换指定目录下的comtrade文件
- [x] 支持指定绘制数据类型: analog 或 digital 或 all
- [ ] 支持指定转换后文件的输出目录
- [ ] 支持解析ascii格式的dat文件

