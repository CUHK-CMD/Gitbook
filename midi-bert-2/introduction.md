---
description: >-
  Github:
  https://github.com/CUHK-CMD/MIDI-BERT-2/tree/feature/performance-tuning
---

# 介紹

我們參考了： [MidiBERT-Piano: Large-scale Pre-training for Symbolic Music Understanding](https://arxiv.org/pdf/2107.05223.pdf)


# Quick Start

1. 請下載 [checkpoints](https://drive.google.com/drive/folders/1ceIfC1UugZQHPgpEEMkdAF0VhZ1EeLl3?usp=sharing)，並重命名文件，如下所示
    ```
    MidiBERT/CP/
    result
    └── finetune
        └── melody_default
            └── model_best.ckpt
        └── velocity_default
            └── model_best.ckpt
        └── composer_default
            └── model_best.ckpt
        └── emotion_default
            └── model_best.ckpt
    ```
2. 請參考 [evaluation](https://github.com/CUHK-CMD/MIDI-BERT-2/tree/feature/performance-tuning#2-evaluation)

3. You are free to go! Evaluation 不需要GPU的 ：）
   