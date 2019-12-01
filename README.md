# CS492---Auto-Summarization
Reproduce and Develop the ACL 2017 paper "Get To The Point: Summarization with Pointer-Generator Networks"
## Vanilla model: seq2seq with attention
  - Word embedding: learn from scratch (embedding layer)
  - Encoder: Unidirectional (the code creates bidirectional but only use forward states) RNNs with LSTM cells
  - Decoder: Unidirectional RNNs with LSTM cells, use beam code decoding in testing
  - Attention: Bahdanau Attention
  - Tensorflow 2, Python 3
