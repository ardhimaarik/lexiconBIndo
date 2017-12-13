# article
http://semangatkecil.blogspot.co.id/2017/12/building-new-dic-dictionary-lexicon-for.html

# how to use
g2p-seq2seq --interactive --model commonwordmodeldic

# depedency
https://github.com/cmusphinx/g2p-seq2seq

# train data
g2p-seq2seq --train newcommonword_lex.dic --model commonwordmodeldic

# result of train model
```
Preparing G2P data
Creating vocabulary commonwordmodeldic/vocab.phoneme
Creating vocabulary commonwordmodeldic/vocab.grapheme
Reading development and training data.
W tensorflow/core/platform/cpu_feature_guard.cc:45] The TensorFlow library wasn't compiled to use SSE3 instructions, but these are available on your machine and could speed up CPU computations.
W tensorflow/core/platform/cpu_feature_guard.cc:45] The TensorFlow library wasn't compiled to use SSE4.1 instructions, but these are available on your machine and could speed up CPU computations.
W tensorflow/core/platform/cpu_feature_guard.cc:45] The TensorFlow library wasn't compiled to use SSE4.2 instructions, but these are available on your machine and could speed up CPU computations.
W tensorflow/core/platform/cpu_feature_guard.cc:45] The TensorFlow library wasn't compiled to use AVX instructions, but these are available on your machine and could speed up CPU computations.
W tensorflow/core/platform/cpu_feature_guard.cc:45] The TensorFlow library wasn't compiled to use AVX2 instructions, but these are available on your machine and could speed up CPU computations.
W tensorflow/core/platform/cpu_feature_guard.cc:45] The TensorFlow library wasn't compiled to use FMA instructions, but these are available on your machine and could speed up CPU computations.
Creating model with parameters:
Learning rate:        0.5
LR decay factor:      0.99
Max gradient norm:    5.0
Batch size:           64
Size of layer:        64
Number of layers:     2
Steps per checkpoint: 200
Max steps:            0
Optimizer:            sgd

Created model with fresh parameters.
global step 200 learning rate 0.5000 step-time 0.08 perplexity 6.41
  eval: perplexity 2.20
global step 400 learning rate 0.5000 step-time 0.08 perplexity 2.10
  eval: perplexity 1.66
global step 600 learning rate 0.5000 step-time 0.08 perplexity 1.18
  eval: perplexity 1.55
global step 800 learning rate 0.5000 step-time 0.05 perplexity 1.02
  eval: perplexity 1.60
No improvement over last 1 times. Training will stop after -1iterations if no improvement was seen.
Training done.
Loading vocabularies from commonwordmodeldic
Creating 2 layers of 64 units.
Reading model parameters from commonwordmodeldic
Beginning calculation word error rate (WER) on test sample.
Words: 20
Errors: 16
WER: 0.800
Accuracy: 0.200
```

# note
you need more data to increase accuracy
