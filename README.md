# KLEJ submissions
Details of KLEJ submissions: https://klejbenchmark.com/leaderboard/

## XLM-RoBERTa (large)

Library: transformers
Model: xlm-roberta-large

* effective batch size: 32
* learning rate: 2e-5
* adam epsilon: 1e-8
* num train epochs: 4
* weight decay: 0.0
* max grad norm: 1.0
* warmup steps: 100

| Run     | NKJP-NER | CDSC-E | CDSC-R | CBD   | PolEmo2.0-IN | PolEmo2.0-OUT | DYK   | PSC   | AR    | Avg     |
|---------|----------|--------|--------|-------|--------------|---------------|-------|-------|-------|---------|
| 1       |   94.6   |  94.4  |  94.7  | 50.7  |     90.4     |     79.8      | 71.6  | 98.2  | 87.5  |  84.7   |

## XLM-RoBERTa (large) - FT2

Based on submission: XLM-RoBERTa (large)

The only change is for the CBD task:
* every positive example is duplicated 4 times
* num train epochs: 1
* weight decay: 0.01
* max grad norm: 5.0
* learning rate: 1e-5

| Run     | NKJP-NER | CDSC-E | CDSC-R | CBD   | PolEmo2.0-IN | PolEmo2.0-OUT | DYK   | PSC   | AR    | Avg     |
|---------|----------|--------|--------|-------|--------------|---------------|-------|-------|-------|---------|
| 1       |   94.6   |  94.4  |  94.7  | **67.9** |  90.4     |     79.8      | 71.6  | 98.2  | 87.5  |  86.6   |

## XLM-RoBERTa (large) - FT3

Library: fairseq
Model: xlm-roberta-large

Models were trained using original scripts from [Polish RoBERTa](https://github.com/sdadas/polish-roberta).

| Run     | NKJP-NER | CDSC-E | CDSC-R | CBD   | PolEmo2.0-IN | PolEmo2.0-OUT | DYK   | PSC   | AR    | Avg     |
|---------|----------|--------|--------|-------|--------------|---------------|-------|-------|-------|---------|
| 1 | 94,1 | 94,4 | 94,7 | 70,6 | 92,4 | 81 | 72,8 | 98,9 | 88,4 | 87,5 |
| 2 | 94,7 | 94,3 | 94,6 | 67,4 | 92,5 | 81,6 | 73,9 | 98,0 | 89,3 | 87,4 |
| 3 | 94,6 | 94,5 | 95 | 67,2 | 92,4 | 82 | 73,4 | 98,8 | 89,1 | 87,4 |
| 4 | 94,8 | 94,3 | 94,8 | 67,5 | 92,7 | 80,6 | 75,3 | 98,3 | 88,5 | 87,4 |
| 5 | 94,4 | 94,0 | 94,8 | 68,5 | 92,5 | 81,2 | 77,1 | 98,6 | 88,5 | 87,7 |

## XLMR+NKJP

XLM-RoBERTa (large) model has been further trained on NCP (National Corpus of Polish).

Models were fine-tuned using original scripts from [Polish RoBERTa](https://github.com/sdadas/polish-roberta).


| Run     | NKJP-NER | CDSC-E | CDSC-R | CBD   | PolEmo2.0-IN | PolEmo2.0-OUT | DYK   | PSC   | AR    | Avg     |
|---------|----------|--------|--------|-------|--------------|---------------|-------|-------|-------|---------|
 | 1 | 94,2 | 94,2 | 94,5 | 72,4 | 93,1 | 77,9 | 77,5 | 98,6 | 88,2 | 87,8 | 
 | 2 | 94,9 | 94,5 | 94,6 | 68,2 | 92,8 | 82 | 74,6 | 99,1 | 88,5 | 87,7 | 
 | 3 | 95,1 | 94,5 | 94,7 | 67,8 | 91,8 | 81,8 | 75 | 97,9 | 88,2 | 87,4 | 
 | 4 | 94,7 | 93,5 | 94,8 | 69,2 | 92,2 | 82,8 | 73,6 | 98 | 88,7 | 87,5 | 
 | 5 | 95,2 | 94,4 | 94,7 | 70,3 | 92,7 | 83,8 | 76,6 | 98,9 | 88,8 | 88,4 | 
 | Avg  | 94,8 | 94,2 | 94,7 | 69,6 | 92,5 | 81,7 | 75,5 | 98,5 | 88,5 | 87,8 | 


### Contact

LinkedIn: https://www.linkedin.com/in/wrobelkrzysztof/
