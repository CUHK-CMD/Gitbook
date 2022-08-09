## E. Skyline

用skyline algorithm 找 pop909 Accuracy

```python
python3 cal_acc.py
```

因為 POP909 包含 *melody*, *bridge*, *accompaniment*，所以skyline algorithm 不能分別出 melody 和 bridge 

最後得出兩個 accuracy 結果

1. 考慮 *Bridge* as *Accompaniment*, 78.54% accuracy
2. 考慮 *Bridge* as *Melody*,  79.51% accuracy

Special thanks to Wen-Yi Hsiao for providing the code for skyline algorithm.