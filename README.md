# CS492---Auto-Summarization
Reproduce and Develop the ACL 2017 paper "Get To The Point: Summarization with Pointer-Generator Networks"
## Vanilla model: seq2seq + attention
  - Word embedding: learn from scratch (embedding layer)
  - Encoder: Unidirectional (the code creates bidirectional but only use forward states) RNNs with LSTM cells
  - Decoder: Unidirectional RNNs with LSTM cells, use beam code decoding in testing
  - Attention: Bahdanau Attention
  - Tensorflow 2, Python 3
## Model: seq2seq + attention with embedding
  - Word embedding: pretrained embedding
  - Encoder: Unidirectional (the code creates bidirectional but only use forward states) RNNs with LSTM cells
  - Decoder: Unidirectional RNNs with LSTM cells, use beam code decoding in testing
  - Attention: Bahdanau Attention
  - Tensorflow 2, Python 3
## Model: seq2seq + attention + coverage
  - Word embedding: embedding layer
  - Encoder: Unidirectional (the code creates bidirectional but only use forward states) RNNs with LSTM cells
  - Decoder: Unidirectional RNNs with GRU cells, use greedy search in testing
  - Attention: Bahdanau Attention with optional coverage
  - Tensorflow 2, Python 3
## Model: seq2seq + attention + coverage with embedding
  - Word embedding: pretrained embedding
  - Encoder: Unidirectional (the code creates bidirectional but only use forward states) RNNs with LSTM cells
  - Decoder: Unidirectional RNNs with GRU cells, pointer network and use (optional) greedy/beam search in testing
  - Attention: Bahdanau Attention with optional coverage
  - Tensorflow 2, Python 3
## Model: seq2seq + attention + pointer + coverage
  - Word embedding: embedding layer
  - Encoder: Unidirectional (the code creates bidirectional but only use forward states) RNNs with LSTM cells
  - Decoder: Unidirectional RNNs with GRU cells with pointer network, use greedy search in testing
  - Attention: Bahdanau Attention with optional coverage
  - Tensorflow 2, Python 3
