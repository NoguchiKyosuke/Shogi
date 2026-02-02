# Pre-study Sources

## YouTube

https://www.youtube.com/watch?v=TWXP88bTyoQ

This video covers the following topics:

- History of Shogi AI
- Evaluation functions
    - 1974: Minimax algorithm
    - Post-Minimax: Alpha-Beta pruning
    - DL-based: Training via SGD (Stochastic Gradient Descent)
    - Typical optimizers used in Shogi AI include AdaGrad, Adam, etc.
- 10 Major Impacts on Shogi AI
    - Reinforcement learning
    - Shogi AI competitions
    - YaneuraOu open source project
    - Evolution of Stockfish
    - NNUE evaluation function
    - AlphaZero
    - nnue-pytorch
    - 『強い将棋ソフトの創り方』 (dlshogi book)
    - Availability of high-quality public training data
        - 山岡忠夫さん: Public training data from 『強い将棋ソフトの創り方』
        - たややんさん: Public training data worth 1 million yen
    - Influence of SNS
- Elo rating: A measure of Shogi AI strength
    - Amateur player: ~1000 Elo
    - Professional player: ~3000 Elo
    - 「お前，CSA会員にならねーか?」: 4914 Elo
- Shogi AI architectures
    - NNUE vs. DL-based architectures
    - NNUE (uses Alpha-Beta pruning):
        - Optimized for CPU calculation
        - Structural limitations (cannot easily increase network depth and width)
    - DL-based (Deep Learning):
        - Typically uses ResNet
        - Incorporates attention mechanisms (e.g., Transformers)

## papers
### 局面に対応したコメント検索を用いた大規模言語モデルによる将棋解説文生成
Authors: 大田 皐介, 中沢 実
URL: https://ipsj.ixsq.nii.ac.jp/records/2005498

points

1. はじめに
- LLM can generate natural commentary for shogi positions.
- LLM coused hallucination. It is a problem.
- To reduce hallucination, use a RAG (Retrieval-Augmented Generation) approach.
- RAG is a method that retrieves relevant document from a database and uses it as context for LLM to generate text.
- This paper proposes a method that uses a commentary by a professional shogi player.
2. Related Research
- Contrastive Language-Image Pre-training (CLIP) is a method that learns a joint representation of images and text.