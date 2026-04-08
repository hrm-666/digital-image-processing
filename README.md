# 西安交通大学《数字图像处理》课程作业仓库

本仓库用于整理西安交通大学《数字图像处理》课程的平时作业、实验代码与相关素材，主要实现环境为 Python + Jupyter Notebook。

## 仓库说明

- 课程：数字图像处理
- 学校：西安交通大学
- 形式：按“第 N 次作业”分目录整理
- 主要工具：Python、Jupyter Notebook、OpenCV、NumPy、Matplotlib、scikit-image

## 目录结构

```text
.
├─ 第一次作业
│  ├─ homework.ipynb
│  ├─ 第一次作业.txt
│  ├─ 7.bmp
│  ├─ lena.bmp
│  ├─ elain1.bmp
│  └─ report_assets/
├─ 第二次作业
│  ├─ homework.ipynb
│  ├─ 图像配准题目.txt
│  ├─ 图像配准作业说明.docx
│  ├─ Image A.jpg
│  ├─ Image B.jpg
│  └─ report_assets/
├─ 第三次作业
│  ├─ homework.ipynb
│  ├─ readme-第3次作业.txt
│  ├─ *.bmp
│  └─ report_assets/
├─ 第四次作业
│  ├─ homework.ipynb
│  ├─ 第四次作业.txt
│  ├─ gaussian.pdf
│  ├─ test1.pgm
│  ├─ test2.tif
│  ├─ test3_corrupt.pgm
│  ├─ test4.tif
│  └─ report_assets/
├─ 第五次作业
│  ├─ homework.ipynb
│  ├─ 第5次作业.txt
│  ├─ test1.pgm
│  ├─ test2.tif
│  ├─ test3_corrupt.pgm
│  ├─ test4.tif
│  └─ report_assets/
├─ 第六次作业
│  ├─ homework.ipynb
│  ├─ 第6次作业.txt
│  ├─ lena.bmp
│  └─ report_assets/
├─ 作业报告格式.doc
├─ README.md
└─ .gitignore
```

## 作业内容

### 第一次作业

对应目录：`第一次作业`

主要内容包括：
1. BMP 图像格式简介与结构分析
2. Lena 图像灰度级从 8-bit 递减到 1-bit 的量化实验
3. Lena 图像均值、方差、标准差计算
4. 使用最近邻、双线性、双三次插值将图像放大到 `2048×2048`
5. 对 Lena 和 Elain 图像进行 shear 与旋转后的插值对比

### 第二次作业

对应目录：`第二次作业`

主要内容包括：
1. 人工选取两幅图像中的对应点
2. 输出对应点坐标
3. 计算图像配准所需的单应矩阵
4. 将待配准图像映射到基准图像坐标系
5. 展示最终图像配准结果

### 第三次作业

对应目录：`第三次作业`

主要内容包括：
1. 绘制多幅灰度图像的直方图
2. 对图像进行全局直方图均衡
3. 根据参考图像进行直方图匹配
4. 对 `elain` 和 `lena` 图像进行 `7×7` 局部直方图增强
5. 基于直方图观察对 `elain` 和 `woman` 图像进行阈值分割

### 第四次作业

对应目录：`第四次作业`

主要内容包括：
1. 对测试图像分别使用高斯滤波与中值滤波进行空间域低通处理，并比较不同模板尺寸下的效果
2. 根据讲义公式生成固定 `sigma=1.5` 的高斯滤波器
3. 对测试图像进行高通滤波与边缘检测，包括 Unsharp Masking、Sobel、Laplacian 和 Canny 方法，并分析各自优缺点

### 第五次作业

对应目录：`第五次作业`

主要内容包括：
1. 设计低通滤波器（Butterworth 和 Gaussian），对测试图像进行平滑处理并计算功率谱比
2. 设计高通滤波器（Butterworth 和 Gaussian），在频域增强边缘并计算功率谱比
3. 实现其他高通滤波器：频域拉普拉斯和 Unmask，对测试图像进行滤波处理
4. 将频域滤波与第四次作业中的空域滤波进行对比讨论，分析两者关系与等效性

### 第六次作业

对应目录：`第六次作业`

主要内容包括：
1. 在测试图像上产生高斯噪声（可指定均值和方差），并用多种滤波器恢复图像，分析各自优缺点
2. 在测试图像加入椒盐噪声（椒和盐噪声密度均是 0.1），用学过的滤波器恢复图像，分析反谐波均值 Q 大于 0 和小于 0 的作用
3. 推导并实现维纳滤波器，包括运动模糊退化函数、逆滤波和维纳滤波的对比分析

## 运行方式

建议使用 Python 3.10 及以上版本。

### 1. 安装依赖

```bash
pip install opencv-python numpy matplotlib scikit-image jupyter
```

### 2. 启动 Jupyter Notebook

```bash
jupyter notebook
```

随后在浏览器中打开对应作业目录下的 `homework.ipynb`，按顺序运行单元即可复现实验过程与结果。

## 提交说明

- 仓库主要用于保存作业代码、notebook 与实验素材。
- 含个人信息的作业报告、PDF、AI 协同日志等文件默认通过 `.gitignore` 排除，不作为公开仓库的主要内容。
- `report_assets` 中与报告正文强绑定的封面图已默认忽略，其余实验结果图可按需要保留。
- 上传 GitHub 前建议执行一次 `git status`，确认没有将报告、日志、临时文件或包含个人信息的文件纳入版本控制。
