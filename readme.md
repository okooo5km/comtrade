# comtrade

包含comtrade解析库和comtrade解析工具。

### 依赖

基于python3开发

- matplotlib
- numpy

安装依赖：

```
pip3 install matplotlib numpy
```

### 文件说明

- **comtrade**: comtrade文件解析工具，是命令行工具，传入参数为comtrade的cfg文件或者dat文件；
- **comtrade.py**: comtrade解析库，包含解析comtrade文件需要的类，使用方法参考 [comtrade](./comtrade) 的内容；

### 功能

#### 解析comtrade文件

- [x] 解析二进制的dat文件
- [ ] 解析文本的dat文件

#### 显示并保存模拟波形

默认保存图像为pdf格式。
