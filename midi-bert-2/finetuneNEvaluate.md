# C. Fine-tune & Evaluate on Downstream Tasks

```./MidiBERT/CP``` and ```./MidiBERT/remi```

### 1. Fine-tuning

* ```finetune.py```
```python
python3 finetune.py --task=melody --name=default
```
Checkpoint 和 log 會在```CP_result/finetune/{name}/``` 出現。

### 2. Evaluation

* ```eval.py```
```python
python3 eval.py --task=melody --cpu --ckpt=[ckpt_path]
```
會 Print `Test loss & accuracy` 和 儲存 confusion matrix

*The same logic applies to REMI representation.*
