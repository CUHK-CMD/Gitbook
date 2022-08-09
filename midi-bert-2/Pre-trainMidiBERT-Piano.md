---
description: >-
  Github:
  https://github.com/CUHK-CMD/MIDI-BERT-2/tree/feature/pretraining#b-pre-train-a-midibert-piano
---
# B. Pre-train a MidiBERT-Piano

`./MidiBERT/CP`  `./MidiBERT/remi`

* pre-train a MidiBERT-Piano
```python
python3 main.py --name=default
```
- checkpoint 和 log 會在 ```CP_result/pretrain/default/``` 出現。
- 可選擇現有的dataset添加到自定的 pre-training dataset 
* customize your own pre-training dataset
    * 加 ```--dataset``` 和 指定的PATH到```load_data()``` function

  - 例如：
    ```python
    # to pre-train a model with only 2 datasets
    python3 main.py --name=default --dataset pop1k7 asap	
    ``` 

Acknowledgement: [HuggingFace](https://github.com/huggingface/transformers), [codertimo/BERT-pytorch](https://github.com/codertimo/BERT-pytorch)

Special thanks to Chin-Jui Chang