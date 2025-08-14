# DATVD--A novel vulnerability detection method based on dynamic attention and hybrid convolutional pooling

## 一、Dataset

**Reveal**:https://drive.google.com/drive/folders/1KuIYgFcvWUXheDhT--cBALsfy1I4utOy

## 二、Code

link：https://drive.google.com/file/d/1M77F-qOlGS5hf7-7ebMXZ1h4ciO84iMI/view?usp=sharing

## 三、**Experimental Procedure**

**The experimental workflow was designed to systematically evaluate the proposed DATVD model.**

1. **Graph Representation Construction:**
   Composite code graphs were constructed by integrating abstract syntax tree (AST), control flow graph (CFG), data flow graph (DFG), and natural code sequence (NCS) information from real-world source code fragments.
2. **Node Feature Extraction and Reduction:**
   Node features were extracted using Word2Vec embeddings and reduced to 128 dimensions via principal component analysis (PCA).
3. **Enhanced Graph Neural Network Processing:**
   These graph representations were input into the enhanced GGNN_DAT network, which introduced a dynamic attention mechanism during message passing to prioritize critical nodes for vulnerability-related features. The hybrid convolutional pooling module, which alternated between maximum pooling and average pooling operations, was used to capture both salient features and global contextual information.
4. **Prediction Output:**
   Finally, a multilayer perceptron (MLP) processed the aggregated features to produce binary classification predictions for vulnerability detection.

## 四、Experimental Setup

**The experiments were conducted on a system equipped with an NVIDIA GeForce RTX 3090 GPU and an Intel Core i5-8400 CPU.  The computational framework was implemented in Python 3.8 using PyTorch as the deep learning library for neural network development and execution.**

Key specifications:

**Accelerator**: NVIDIA GeForce RTX 3090 (24GB GDDR6X VRAM)

**Processor**: Intel Core i5-8400 CPU @ 2.80GHz (6 cores)

**Programming Language**: Python 3.8

**Deep Learning Framework**: PyTorch 1. x (with CUDA 11. x acceleration)
