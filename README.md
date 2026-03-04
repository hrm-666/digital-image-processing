# 西安交通大学《数字图像处理》课程作业仓库

本仓库用于整理与提交西安交通大学《数字图像处理》课程的课后作业。

## 仓库简介

- 课程：数字图像处理
- 学校：西安交通大学
- 用途：记录每次课后作业的实现过程、代码与实验结果
- 主要实现环境：Python + Jupyter Notebook（OpenCV / NumPy / Matplotlib）

## 目录结构

```text
第一次作业/
├─ 第一次作业.txt      # 作业题目说明
├─ homework.ipynb      # 作业实现与可视化
├─ 7.bmp               # BMP格式分析示例图
├─ lena.bmp            # 实验图像
└─ elain1.bmp          # 实验图像
```

## 第一次作业内容

根据 `第一次作业/第一次作业.txt`，本次作业包含以下任务：

1. BMP 图像格式简介（以 `7.bmp` 为例）
2. 将 `lena`（512×512）图像灰度级从 8-bit 逐级递减到 1-bit 并显示
3. 计算 `lena` 图像的均值与方差（代码中同时输出标准差）
4. 使用近邻、双线性、双三次插值，将 `lena` 放大到 2048×2048
5. 对 `lena` 和 `elain` 进行水平 shear 与旋转 30°，并分别用三种插值方式变换到 2048×2048

对应实现文件：`第一次作业/homework.ipynb`

## 运行方式

建议使用 Python 3.10+。

### 1) 安装依赖

```bash
pip install opencv-python numpy matplotlib jupyter
```

### 2) 打开并运行 Notebook

```bash
jupyter notebook
```

在浏览器中打开 `第一次作业/homework.ipynb`，按顺序运行各单元即可复现实验结果。

## 说明

- 本仓库用于课程学习与作业记录。
- 后续作业将按“第N次作业”持续补充到仓库中。
