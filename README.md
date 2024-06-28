[![author](https://img.shields.io/badge/author-mohd--faizy-red)](https://github.com/mohd-faizy)
![made-with-Markdown](https://img.shields.io/badge/Made%20with-markdown-blue)
![Language](https://img.shields.io/github/languages/top/mohd-faizy/Learn_Seaborn)
![Maintained](https://img.shields.io/maintenance/yes/2024)
![Last Commit](https://img.shields.io/github/last-commit/mohd-faizy/Learn_Seaborn)
[![contributions welcome](https://img.shields.io/static/v1.svg?label=Contributions&message=Welcome&color=0059b3&style=flat-square)](https://github.com/mohd-faizy/Learn_Seaborn)
![Size](https://img.shields.io/github/repo-size/mohd-faizy/Learn_Seaborn)

# Learn_Seaborn

![Seaborn-banner](https://github.com/mohd-faizy/Learn_Seaborn/blob/main/_img/Seaborn-banner.jpg)

Welcome to the Learn_Seaborn repository! This repo is dedicated to providing helpful resources, tutorials, and examples for using the Seaborn library in Python.

## Table of Contents

- [Learn\_Seaborn](#learn_seaborn)
  - [Table of Contents](#table-of-contents)
  - [Roadmap](#roadmap)
  - [Introduction](#introduction)
  - [Installation](#installation)
  - [Usage](#usage)
    - [Basic Plot](#basic-plot)
    - [Categorical Plot](#categorical-plot)
    - [Matrix Plot](#matrix-plot)
    - [Multi-plot Grids](#multi-plot-grids)
  - [Features](#features)

## Roadmap

![Seaborn-roadmap](https://github.com/mohd-faizy/Learn_Seaborn/blob/main/_img/Seaborn-Roadmap.png)

## Introduction

Seaborn is a Python visualization library based on Matplotlib that provides a high-level interface for drawing attractive statistical graphics. It is built on top of Matplotlib and is closely integrated with pandas data structures.

This repository aims to help users of all skill levels to better understand and utilize the Seaborn library through comprehensive guides, code snippets, and example projects.

## Installation

To install Seaborn, you can use pip, the Python package installer. Ensure you have Python installed, then run:

```bash
pip install seaborn
```

For more detailed installation instructions, please refer to the [official Seaborn installation guide](https://seaborn.pydata.org/installing.html).

## Usage

Here are some basic examples to get you started with Seaborn:

### Basic Plot

```python
import seaborn as sns
import matplotlib.pyplot as plt

data = sns.load_dataset('iris')
sns.scatterplot(x='sepal_length', y='sepal_width', data=data)
plt.title('Basic Scatter Plot')
plt.show()
```

### Categorical Plot

```python
import seaborn as sns
import matplotlib.pyplot as plt

data = sns.load_dataset('tips')
sns.catplot(x='day', y='total_bill', hue='sex', kind='bar', data=data)
plt.title('Categorical Plot')
plt.show()
```

### Matrix Plot

```python
import seaborn as sns
import matplotlib.pyplot as plt

data = sns.load_dataset('flights')
data = data.pivot('month', 'year', 'passengers')
sns.heatmap(data, annot=True, fmt='d', cmap='YlGnBu')
plt.title('Heatmap')
plt.show()
```

### Multi-plot Grids

```python
import seaborn as sns
import matplotlib.pyplot as plt

data = sns.load_dataset('iris')
g = sns.PairGrid(data, hue='species')
g = g.map_diag(plt.hist)
g = g.map_offdiag(plt.scatter)
g = g.add_legend()
plt.title('Pair Grid')
plt.show()
```

For more examples and detailed tutorials, please refer to the [official Seaborn documentation](https://seaborn.pydata.org/).

## Features

- High-level interface for drawing attractive statistical graphics
- Built on top of Matplotlib and closely integrated with pandas
- Themes for styling matplotlib graphics
- Functions for visualizing univariate and bivariate data
- Tools for fitting and visualizing linear regression models
- Functions for visualizing matrices and data frames
- Utilities for creating complex visualizations

## ⚖ ➤ License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

## ❤️ Support

If you find this repository helpful, show your support by starring it! For questions or feedback, reach out on [Twitter(`X`)](https://twitter.com/F4izy).

#### $\color{skyblue}{\textbf{Connect with me:}}$

➤ If you have questions or feedback, feel free to reach out!!!

[<img align="left" src="https://cdn4.iconfinder.com/data/icons/social-media-icons-the-circle-set/48/twitter_circle-512.png" width="32px"/>][twitter]
[<img align="left" src="https://cdn-icons-png.flaticon.com/512/145/145807.png" width="32px"/>][linkedin]
[<img align="left" src="https://cdn-icons-png.flaticon.com/512/2626/2626299.png" width="32px"/>][Portfolio]

[twitter]: https://twitter.com/F4izy
[linkedin]: https://www.linkedin.com/in/mohd-faizy/
[Portfolio]: https://ai.stackexchange.com/users/36737/faizy?tab=profile

---

<img src="https://github-readme-stats.vercel.app/api?username=mohd-faizy&show_icons=true" width=380px height=200px />
