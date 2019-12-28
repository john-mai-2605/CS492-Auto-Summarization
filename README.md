# CS492---Auto-Summarization
Reproduce and Develop the ACL 2017 paper "Get To The Point: Summarization with Pointer-Generator Networks"
## Code: Replication of the code for the above paper See et.al. 2017 with some modifications
### Vanilla model 1.1: seq2seq + attention
  - Word embedding: learn from scratch (embedding layer)
  - Encoder: Unidirectional (the code creates bidirectional but only use forward states) RNNs with LSTM cells
  - Decoder: Unidirectional RNNs with LSTM cells, use beam code decoding in testing
  - Attention: Bahdanau Attention
  - Tensorflow 2, Python 3
### Model 2.1: seq2seq + attention + coverage
  - Word embedding: embedding layer
  - Encoder: Unidirectional (the code creates bidirectional but only use forward states) RNNs with LSTM cells
  - Decoder: Unidirectional RNNs with GRU cells, use greedy search in testing
  - Attention: Bahdanau Attention with optional coverage
  - Tensorflow 2, Python 3
### Model 3.1: seq2seq + attention + pointer + coverage
  - Word embedding: embedding layer
  - Encoder: Unidirectional (the code creates bidirectional but only use forward states) RNNs with LSTM cells
  - Decoder: Unidirectional RNNs with GRU cells with pointer network, use greedy search in testing
  - Attention: Bahdanau Attention with optional coverage
  - Tensorflow 2, Python 3
### Model x.2: Model x.1 with embedding
  - Word embedding: GloVE, Word2Vec, Bio
### Model x.3: Model x.1 with ROUGE point implemented
## Proposal: Overview of the original paper and proposed changes
## Paper: Detail explanation about the original paper
## Poster: Poster about this project
## Report: Report about this project
