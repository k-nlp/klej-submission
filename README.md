# KLEJ submissions
Details of KLEJ submissions: https://klejbenchmark.com/leaderboard/

## XLM-RoBERTa (large)

Transfomer model: xlm-roberta-large

* effective batch size: 32
* learning rate: 2e-5
* adam epsilon: 1e-8
* num train epochs: 4
* weight decay: 0.0
* max grad norm: 1.0
* warmup steps: 100

## XLM-RoBERTa (large) - FT2

Based on submission: XLM-RoBERTa (large)

The only change is a data oversampling for the CBD task. Every positive example is duplicated 4 times.
