# 🌈IlovePaddleModel

集锦PaddlePaddle为我们提供的方便的模型和解决方案 | The best model, the best US.

<img align='right' src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif" width="230">

- 上次更新时间：
```
2022.06.10
```
- 最新更新内容：
```
- PULC
- PP-ShiTu
```
- 标注
```
🌟：表示热门模型
⚡：最新更新模型
```

<p id="top"></p>

## 📄目录|contents

- [🟣PaddleHub](#1)
- [🔵PaddleClas](#2)
   - [⚡PULC](#2.1) -> 超轻量图像分类模型库
   - [⚡PP-ShiTu](#2.2) -> 轻量级通用图像识别系统
- [🔴PaddleDetection](#3)
   - [676类目标检测](#3.1) -> [676目标检测](https://github.com/PaddlePaddle/PaddleDetection/blob/release/2.4/static/dataset/voc/generic_det_label_list_zh.txt)
- [🟡PaddleOCR](#4)
   - [PP-OCRv3](#4.1) -> OCR识别
- [🟢PaddleSeg](#5)
  - [Matting](#5.1) -> 抠图 
- [🟠PaddleGAN](#6)

<img src="https://github.com/WangRongsheng/IlovePaddleModel/blob/main/images/fenge.png" width="1000" height="200"/>

<p id="1"></p>

## 🟣PaddleHub

> 便捷地获取PaddlePaddle生态下的预训练模型，完成模型的管理和一键预测。配合使用Fine-tune API，可以基于大规模预训练模型快速完成迁移学习，让预训练模型能更好地服务于用户特定场景的应用。

📦[Github：PaddleHub](https://github.com/PaddlePaddle/PaddleHub)  🌐[Home：PaddleHub](https://www.paddlepaddle.org.cn/hub)

[⬆️返回顶部](#top)

---

<p id="2"></p>

## 🔵PaddleClas

> 飞桨图像识别套件PaddleClas是飞桨为工业界和学术界所准备的一个图像识别任务的工具集，助力使用者训练出更好的视觉模型和应用落地。

📦[Github：PaddleClas](https://github.com/PaddlePaddle/PaddleClas)

<p id="2.1"></p>

1. [PULC超轻量图像分类方案](https://github.com/PaddlePaddle/PaddleClas/blob/develop/docs/zh_CN/PULC/PULC_quickstart.md) ->PULC 方法产出的系列模型在人、车、OCR等方向的多个场景中均验证有效，用超轻量模型就可实现与 SwinTransformer 模型接近的精度，预测速度提高 40+ 倍。并且打通数据、模型训练、压缩和推理部署全流程。

<p id="2.2"></p>

2. [PP-ShiTu图像识别系统](https://github.com/PaddlePaddle/PaddleClas/blob/develop/docs/zh_CN/quick_start/quick_start_recognition.md) ->PP-ShiTu是一个实用的轻量级通用图像识别系统，主要由主体检测、特征学习和向量检索三个模块组成。该系统从骨干网络选择和调整、损失函数的选择、数据增强、学习率变换策略、正则化参数选择、预训练模型使用以及模型裁剪量化8个方面，采用多种策略，对各个模块的模型进行优化，最终得到在CPU上仅0.2s即可完成10w+库的图像识别的系统。

[⬆️返回顶部](#top)

---

<p id="3"></p>

## 🔴PaddleDetection

> PaddleDetection为基于飞桨PaddlePaddle的端到端目标检测套件，内置30+模型算法及250+预训练模型，覆盖目标检测、实例分割、跟踪、关键点检测等方向，其中包括服务器端和移动端高精度、轻量级产业级SOTA模型、冠军方案和学术前沿算法，并提供配置化的网络模块组件、十余种数据增强策略和损失函数等高阶优化支持和多种部署方案，在打通数据处理、模型开发、训练、压缩、部署全流程的基础上，提供丰富的案例及教程，加速算法产业落地应用。

📦[Github：PaddleDetection](https://github.com/PaddlePaddle/PaddleDetection)

<p id="3.1"></p>

1. [676类目标检测](https://github.com/PaddlePaddle/PaddleDetection/blob/release/2.4/static/docs/featured_model/LARGE_SCALE_DET_MODEL.md) ->结合服务器端实用目标检测方案，融合OpenImages V5和Objects365训练集数据(二者包含许多重复类别)，生成了包含676个类别的新数据集。训练了服务器端实用目标检测模型，适用于绝大部分应用场景，方便用户直接部署使用，用户也可以根据提供的预训练模型，在自己的数据集上进行模型微调，加快收敛并获得更高的精度指标。

[⬆️返回顶部](#top)

---

<p id="4"></p>

## 🟡PaddleOCR

> PaddleOCR旨在打造一套丰富、领先、且实用的OCR工具库，助力开发者训练出更好的模型，并应用落地。

📦[Github：PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR)

<p id="4.1"></p>

1. [PP-OCRv3](https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.5/doc/doc_ch/quickstart.md) [介绍](https://github.com/PaddlePaddle/PaddleOCR/blob/release/2.5/doc/doc_ch/ppocr_introduction.md#pp-ocrv3) ->PP-OCRv3在PP-OCRv2的基础上进一步升级。整体的框架图保持了与PP-OCRv2相同的pipeline，针对检测模型和识别模型进行了优化。其中，检测模块仍基于DB算法优化，而识别模块不再采用CRNN，换成了IJCAI 2022最新收录的文本识别算法SVTR，并对其进行产业适配。

[⬆️返回顶部](#top)

---

<p id="5"></p>

## 🟢PaddleSeg

> PaddleSeg是基于飞桨PaddlePaddle开发的端到端图像分割开发套件，涵盖了高精度和轻量级等不同方向的大量高质量分割模型。通过模块化的设计，提供了配置化驱动和API调用两种应用方式，帮助开发者更便捷地完成从训练到部署的全流程图像分割应用。

📦[Github：PaddleSeg](https://github.com/PaddlePaddle/PaddleSeg)

<p id="5.1"></p>

1. [Matting](https://github.com/PaddlePaddle/PaddleSeg/tree/release/2.5/Matting) ->Matting（精细化分割/影像去背/抠图）是指借由计算前景的颜色和透明度，将前景从影像中撷取出来的技术，可用于替换背景、影像合成、视觉特效，在电影工业中被广泛地使用。 

[⬆️返回顶部](#top)

---

<p id="6"></p>

## 🟠PaddleGAN

> 飞桨生成对抗网络开发套件，提供经典及前沿的生成对抗网络高性能实现，覆盖影像修复、图像生成、动作迁移等多种应用场景，支撑开发者快速构建、训练及部署生成对抗网络，以供学术、娱乐及产业应用。

📦[Github：PaddleGAN](https://github.com/PaddlePaddle/PaddleGAN)  🌐[Home：PaddleGAN](https://www.paddlepaddle.org.cn/paddlegan)

[⬆️返回顶部](#top)

---
<p align="center">🔰版权所有&copy王荣胜 |💬QQ：603329354 |📁反馈意见：wrswyz@88.com or <a href="https://github.com/WangRongsheng/IlovePaddleModel/issues">issue</a></p> 

<center><img src="https://cdn.jsdelivr.net/gh/drew233/cdn//20191003172815.webp" height="350" width="1000"></center>
