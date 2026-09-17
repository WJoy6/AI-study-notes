# Assignment 1 · 本地运行说明（Windows）

本作业官方流程用 Google Colab，但在本地 Jupyter 里完全可以跑，你已具备全部条件（Python 3.12 + numpy + matplotlib + JupyterLab）。

## 运行前必做

1. **CIFAR-10 数据集**：已提前下载并解压到 `cs231n/datasets/cifar-10-batches-py/`，无需再下载。

2. **跳过第 1 个代码单元**：每个 notebook 的第 1 个代码单元是"挂载 Google Drive"（`from google.colab import drive`），本地没有 Colab 会报错——**不要运行它**，直接从第 2 个代码单元（`# Run some setup code`）开始。

## 怎么运行

1. 打开 Anaconda Prompt 或 cmd，进入本目录：
   ```
   cd C:\Users\Lenovo\study-notes\assignments\assignment1
   ```
2. 启动 Jupyter：
   ```
   jupyter lab
   ```
3. 在浏览器里依次打开并完成 5 个 notebook：
   - `knn.ipynb` — Q1 kNN 分类器（第 1-2 周任务）
   - `softmax.ipynb` — Q2 Softmax 分类器
   - `two_layer_net.ipynb` — Q3 两层神经网络
   - `features.ipynb` — Q4 高级特征
   - `FullyConnectedNets.ipynb` — Q5 全连接网络

## 完成一个 notebook 后的提交动作

```
git add -A
git commit -m "Assignment1: 完成kNN"
git push
```

## 小提示

- 数据量：训练集 5 万张、测试集 1 万张，本机 8GB 显存/内存无压力
- kNN 的 O(n²) 距离计算用 GPU 没必要，numpy 向量化即可（本作业 Q1 主要练这个）
- 做作业是重点：**作业 = 面试证据**，别只抄答案，一行行看懂为什么
