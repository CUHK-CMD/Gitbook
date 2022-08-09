---
description: >-
  Github:
  https://github.com/CUHK-CMD/MIDI-BERT-2/tree/feature/performance-tuning#a-prepare-data
---

# 預備 Data

全部CP/REMI token DATA 都是儲存在 `data/CP` 和 `data/remi`，其中包括 train, valid, test split。

## 1. 下載DATASET和PREPROCESS

- 將DATASET 儲存在 `Dataset/`
  * [SOD](https://qsdfo.github.io/LOP/database)
    * 點擊連結下載 SOD
    * 我們主要用SOD DATASET 做PREPROCESS，全部都是'2/4','3/4','4/4' 拍
      * [StringQuartets Data](https://github.com/CUHK-CMD/Time-Signature-Detection)
      * 找合格的DATA [CoLab](https://colab.research.google.com/drive/1GLXNTe8HsqzX9AayA4-IN3cQBAw4oKSr?usp=sharing#scrollTo=z-WtA0XCoWyz)
  * [Pop1K7](https://github.com/YatingMusic/compound-word-transformer)
  * [ASAP](https://github.com/fosfrancesco/asap-dataset)
    * 點擊連結下載 ASAP dataset
  * [POP909](https://github.com/music-x-lab/POP909-Dataset)
    * preprocess 有 865 份合格的 4/4 拍 .mid
    * ```cd preprocess_pop909```
    * ```exploratory.py``` 提取合格的 4/4 拍 .mid並儲存到 ```qual_pieces.pkl```
    * ```preprocess.py``` 去 realign and preprocess
    * 感謝 Shih-Lun (Sean) Wu
  * [Pianist8](https://zenodo.org/record/5089279)
    * Step 1: 點擊連結下載 Pianist8 dataset
    * Step 2: Run `python3 pianist8.py` 分 data 到 `Dataset/pianist8_(mode).pkl`
  * [EMOPIA](https://annahung31.github.io/EMOPIA/)
    * Step 1: 點擊連結下載 Emopia dataset 
    * Step 2: Run `python3 emopia.py` 分 data 到 `Dataset/emopia_(mode).pkl`

## 2.  Prepare Dictionary

- `dict/make_dict.py` customize the events & words you'd like to add.

In this paper, we only use Bar, Position, Pitch, Duration. And we provide our dictionaries in CP & REMI representation.

`dict/CP.pkl`

`dict/remi.pkl`

