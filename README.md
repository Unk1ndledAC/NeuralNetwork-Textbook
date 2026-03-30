# Neural Network Textbook

**Neural Networks: A Comprehensive Textbook for AI Students**

A comprehensive, systematic textbook on neural networks covering core topics from fundamental mathematics to state-of-the-art architectures, featuring detailed mathematical derivations, PyTorch practical examples, and real-world application cases.

## Features

- Complete knowledge system from perceptrons to Transformers
- Detailed mathematical derivations with intuitive explanations
- Practical examples using the PyTorch framework
- GPU acceleration and CUDA programming concepts
- Real-world application cases and analysis

## Table of Contents

| Ch. | Topic |
|:---:|:---|
| 1 | Mathematical Foundations |
| 2 | Activation Functions |
| 3 | Loss Functions |
| 4 | Neural Network Architectures |
| 5 | Core Operations |
| 6 | Skip Connections & Attention Mechanisms |
| 7 | Optimizers & Learning Rate Schedulers |
| 8 | Classic Network Architectures |
| 9 | Parameter & Computation Analysis |
| 10 | Training & Frameworks |
| 11 | Dataset Processing |

## Project Structure

```
NeuralNetwork-Textbook/
├── Eng/               
│   ├── opening/            # Front matter (title page, abstract, acknowledgements, etc.)
│   ├── text/
│   │   ├── chapters/       # Main chapters (chapter-01 ~ chapter-11)
│   │   └── appendix/       # Appendix
│   ├── bibliography/       # References
│   ├── glossary/           # Glossary
│   ├── style/              # LaTeX style files
│   ├── main.tex            # Main compilation entry
│   └──   Makefile
└── README.md               # README

```

## Build

### Prerequisites

- **TeX Live 2024+** or **MiKTeX** (full installation)
- **Python 3** with [Pygments](https://pygments.org/) installed (`pip install Pygments`) — required by the `minted` package for code highlighting
- **Biber** — for bibliography processing

### Compilation

```bash
cd Eng
make pdf
```

The Makefile includes the `-shell-escape` flag required by `minted`.

### Clean up

```bash
make clean       # Remove auxiliary files
make cleanall    # Remove auxiliary files + PDF
```

## License

This project is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).

## Acknowledgements

### Template

This textbook is typeset using [Alcazar](https://github.com/dpmj/alcazar) — a free and open-source LaTeX template for academic works. Thanks to Juan Del Pino Mena for this excellent template.

> Del Pino Mena, J. (2024). Alcazar: A free and Open-Source LaTeX template for academic works. Zenodo. https://doi.org/10.5281/zenodo.13935260

### Academic Pioneers

Thanks to Yann LeCun, Geoffrey Hinton, Yoshua Bengio, and many other researchers whose groundbreaking work laid the foundation for modern neural networks and deep learning.

### Open-Source Community

Thanks to the developers of PyTorch, NumPy, and other tools that have made deep learning accessible to researchers and practitioners worldwide.
