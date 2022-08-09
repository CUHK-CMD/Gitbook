# D. Baseline Model (Bi-LSTM)
```./MidiBERT/CP``` 和 ```./MidiBERT/remi```

We seperate our baseline model to note-level tasks, which used a Bi-LSTM, and sequence-level tasks, which used a Bi-LSTM + Self-attention model.

For evaluation, in note-level task, please specify the checkpoint name.
In sequence-level task, please specify only the output name you set when you trained.

* Train a Bi-LSTM
	* note-level task
	```python
	python3 main.py --task=melody --name=0710
	```
	* sequence-level task
	```python
	python3 main.py --task=composer --output=0710
	```

* Evaluate
	* note-level task:
	```python
	python3 eval.py --task=melody --ckpt=result/melody-LSTM/0710/LSTM-melody-classification.pth
	```
	* sequence-level task
	```python
	python3 eval.py --task='composer' --ckpt=0710
	```

The same logic applies to REMI representation. 

Special thanks to Ching-Yu (Sunny) Chiu