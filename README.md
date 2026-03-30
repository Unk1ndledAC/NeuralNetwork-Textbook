# Neural Network Textbook / 神经网络教材

**Neural Networks: A Comprehensive Textbook for AI Students**
**神经网络：面向人工智能专业学生的综合教材**

本项目提供一份全面系统的神经网络教材，涵盖从基础数学到前沿架构的核心内容，包含详细的数学推导、PyTorch 实践示例以及真实应用案例。教材提供中文和英文两个版本。

## 特点

- 从感知机到 Transformer 的完整知识体系
- 详细的数学推导与直观的解释
- 基于 PyTorch 框架的实践示例
- GPU 加速与 CUDA 编程概念
- 真实世界的应用案例与分析

## 目录 / Table of Contents

| 章节 | 中文版 / Chinese | English |
|:---:|:---|:---|
| 第1章 | 数学基础 | Mathematical Foundations |
| 第2章 | 激活函数 | Activation Functions |
| 第3章 | 损失函数 | Loss Functions |
| 第4章 | 神经网络架构 | Neural Network Architectures |
| 第5章 | 神经网络核心操作 | Core Operations |
| 第6章 | 跳跃连接与注意力机制 | Skip Connections & Attention Mechanisms |
| 第7章 | 优化器与学习率调度器 | Optimizers & Learning Rate Schedulers |
| 第8章 | 经典网络架构 | Classic Network Architectures |
| 第9章 | 参数量与计算量分析 | Parameter & Computation Analysis |
| 第10章 | 训练过程与框架 | Training & Frameworks |
| 第11章 | 数据集处理 | Dataset Processing |

## 项目结构

```
NeuralNetwork-Textbook/
├── chinese/                # 中文版
│   ├── opening/            # 前置部分（封面、摘要、致谢、目录等）
│   ├── text/
│   │   ├── chapters/       # 正文章节（chapter-01 ~ chapter-11）
│   │   └── appendix/       # 附录
│   ├── bibliography/       # 参考文献
│   ├── glossary/           # 术语表
│   ├── style/              # LaTeX 样式文件
│   ├── main.tex            # 主编译入口
│   └── Makefile
├── english/                # 英文版（结构同中文版）
└── README.md
```

## 编译 / Build

### 前置要求

- **TeX Live 2024+** 或 **MiKTeX**
- **Python 3**
- **Biber**
- 中文版需要 **XeLaTeX** 编译（推荐）或 LuaLaTeX

### 编译命令

**英文版（pdfLaTeX）：**
```bash
cd english
make pdf
```

**中文版（XeLaTeX）：**
```bash
cd chinese
xelatex main
biber main
xelatex main
xelatex main
```


## 许可证

本项目采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 许可证。

## 致谢 / Acknowledgements

### 模板

本教材的排版基于 [Alcazar](https://github.com/dpmj/alcazar) — 一个免费开源的 LaTeX 学术写作模板。感谢作者 Juan Del Pino Mena 的工作。

> Del Pino Mena, J. (2024). Alcazar: A free and Open-Source LaTeX template for academic works. Zenodo. https://doi.org/10.5281/zenodo.13935260

### 学术先驱

感谢 Yann LeCun、Geoffrey Hinton、Yoshua Bengio 等研究者的开创性工作，奠定了现代神经网络与深度学习的基础。

### 开源社区

感谢 PyTorch、NumPy 等开源工具的开发者，使深度学习技术得以在全球范围内普及。
