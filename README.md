# Chinese IME Design

[中文版 README](./README_zh.md)

This repository demonstrates a basic example of the architecture design of the core algorithms of a Chinese IME (Input Method Editor).

## 1. Overview

<img src="./architecture.png" width="800" alt="Architecture" />

## 2. Pinyin Splitting

### 2.1 Definition

`zhongwen` to `zhong'wen`

### 2.2 Related Technologies

- [TrieTree - Wikipedia](https://en.wikipedia.org/wiki/Trie)

## 3. Chinese Word Query

### 3.1 Definition

`zhong'wen` to `[ "中文", "仲文" ]`

### 3.2 Related Technologies

- Chinese Pinyin dictionary

## 4. Next-word Prediction

### 4.1 Definition

**Next-word prediction** refers to predicting the most probable next-words (candidates) according to the user input context.

### 4.2 Related Technologies

- N-gram: Peter F Brown, Vincent J Della Pietra, Peter V Desouza, Jennifer C Lai, and Robert L Mercer. 1992. *Class-based n-gram models of natural language*. Computational Linguistics 18, 4 (1992), 467–480.
- Transformers: [pretrained models](https://huggingface.co/transformers/pretrained_models.html), [a GitHub repo](https://github.com/renatoviolin/next_word_prediction)
- [清源 CPM](https://cpm.baai.ac.cn/)
- [jieba](https://github.com/fxsjy/jieba)
- [sego](https://github.com/huichen/sego)

## 5. Emoji Prediction

### 5.1 Definition

**Emoji prediction** refers to predicting the most probable emojis (candidates) associated with the user input context.

### 5.2 Related Technologies

- W. Ma, R. Liu, L. Wang, and S. Vosoughi, *Emoji prediction: Extensions
and benchmarking*, in Proceedings of the Conference on Empirical
Methods in Natural Language Processing, 2020.
- S. Ramaswamy, R. Mathews, K. Rao, and F. Beaufays, *Federated
learning for emoji prediction in a mobile keyboard*, arXiv preprint
arXiv:1906.04329, 2019.
