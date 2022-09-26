# BioBERT-CFA-MTM

This is the implementation of Biomedical Named Entity Recognition with the Combined Feature Attention and Fully-Shared Multi-Task Learning

# Requirements

-  `python3`
- `pip3 install -r requirements.txt`
- Downloading [BioBERT](https://github.com/naver/biobert-pretrained) and using our [vocat.txt](./vocab.txt)

# Run

`python run_ner_multi.py --data_dir=data/all/ --bert_model=./biobert-base-cased-v1.1 --task_n
ame=ner --output_dir=./output/all_c --max_seq_length=128 --do_train --num_train_epochs=10 --do_eval --warmup_proportion=0.1 --
learning_rate=5e-5 --train_batch_size=64`


# Example

## BioBERT-MTM

### NCBI-disease
```
             precision    recall  f1-score   support

          I     0.8789    0.8920    0.8854       537
          B     0.8987    0.9146    0.9066       960

avg / total     0.8916    0.9065    0.8990      1497
```
