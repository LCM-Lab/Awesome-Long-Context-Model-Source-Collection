# Long Context Modeling in the Large Language Model (LLM) Era — Advances and Challenges

**📘 About the Tutorial (NLPCC'2024 and CCMT'2024)**

This tutorial, presented by [Juntao Li](https://lijuntaopku.github.io/) and [Zecheng Tang](https://zetangforward.github.io/) from the [OpenNLG Group](https://opennlg.cn/) @ Soochow University, delves into the recent advancements and challenges in long-context modeling within the era of large language models (LLMs). It covers the latest research and practical implementations in the long-context model field.

**📑 NLPCC'2024 Tutorial Slides** [[PDF]](./NLPCC2024-Long_context_model.pdf)
**📑 CCMT'2024 Tutorial Slides** [[PDF]](./CCMT2024-Slides-CN.pdf)

# 🔍 Navigation

Click on the links below to jump directly to each section:

- [Tutorial](# Long Context Modeling in the Large Language Model (LLM) Era — Advances and Challenges)
- [📚 Survey Papers Collection](./README.md)

# Resources (Paper and Blog)
**📌 Note** We only cover the paper lists within the tutorial slides. For more papers, plz refer to [https://github.com/Xnhyacinth/Awesome-LLM-Long-Context-Modeling](https://github.com/Xnhyacinth/Awesome-LLM-Long-Context-Modeling)

### Long-context Scaling
- Paper List:
    - [Train Short, Test Long: Attention with Linear Biases Enables Input Length Extrapolation](https://arxiv.org/abs/2108.12409)
    - [Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer](https://papers.cool/arxiv/1910.10683)
    - [RoFormer: Enhanced Transformer with Rotary Position Embedding](https://arxiv.org/pdf/2104.09864)
    - [Extending Context Window of Large Language Models via Positional Interpolation](https://arxiv.org/abs/2306.15595)
- Implementation:
    - [RoFormer_pytorch](https://github.com/JunnYu/RoFormer_pytorch)
- Blog:
    - [让研究人员绞尽脑汁的Transformer位置编码](https://spaces.ac.cn/archives/8130/comment-page-1#T5%E5%BC%8F)
    - [Transformer升级之路：7、长度外推性与局部注意力](https://kexue.fm/archives/9431)
    - [Transformer升级之路：16、“复盘”长度外推技术](https://kexue.fm/archives/9948)


### Long-context Alignment
- Paper List
    - [PoSE: Efficient Context Window Extension of LLMs via Positional Skip-wise Training](https://arxiv.org/abs/2309.10400)
    - [LongAlign: A Recipe for Long Context Alignment of Large Language Models](https://arxiv.org/abs/2401.18058)
    - [Long Context Alignment with Short Instructions and Synthesized Positions](https://arxiv.org/abs/2405.03939)
    - [LOGO — LONG CONTEXT ALIGNMENT VIA EFFICIENT PREFERENCE OPTIMIZATION](https://arxiv.org/pdf/2410.18533v1)
    

##### 1) Efficient Attention
- Paper List
    - [LED: Lightweight and efficient end-to-end speech recognition using low-rank transformer](https://arxiv.org/abs/1910.13923)
    - [Linformer: Self-attention with linear complexity](https://arxiv.org/abs/2006.04768)
    - [Generating Long Sequences with Sparse Transformers](https://arxiv.org/abs/1904.10509)
    - [Big Bird: Transformers for Longer Sequences](https://arxiv.org/abs/2007.14062)
    - [Longformer: The Long-Document Transformer](https://arxiv.org/abs/2004.05150)
    - [Selective Attention Improves Transformer](https://arxiv.org/abs/2410.02703)
    - [RetrievalAttention: Accelerating Long-Context LLM Inference via Vector Retrieval](https://arxiv.org/abs/2409.10516)
    - [Efficient Long-range Language Modeling with Self-supervised Causal Retrieval](https://arxiv.org/abs/2410.01651)
    

##### 2) New Architecture

- Paper List:
  - [Transformers are RNNs: Fast Autoregressive Transformers with Linear Attention](https://arxiv.org/abs/2006.16236)
  - [Efficiently Modeling Long Sequences with Structured State Spaces](https://arxiv.org/abs/2111.00396)
  - [Mamba: Linear-Time Sequence Modeling with Selective State Spaces](https://arxiv.org/abs/2312.00752)
  - [Zoology: Measuring and Improving Recall in Efficient Language Models](https://arxiv.org/abs/2312.04927)
  - [MemLong:MemLong: Memory-Augmented Retrieval for Long Text Modeling](https://arxiv.org/abs/2408.16967)
  - [Revealing and Mitigating the Local Pattern Shortcuts of Mamba](arxiv.org/abs/2410.15678)
- Implementation:
  - [GitHub - sustcsonglin/flash-linear-attention: Efficient implementations of state-of-the-art linear attention](https://github.com/sustcsonglin/flash-linear-attention)
  - [GitHub - state-spaces/mamba: Mamba SSM architecture](https://github.com/state-spaces/mamba)
  - [GitHub - HazyResearch/safari: Convolutions for Sequence Modeling](https://github.com/HazyResearch/safari)
- Blog:
  - [https://spaces.ac.cn/archives/7546](https://spaces.ac.cn/archives/7546)
  - [https://hazyresearch.stanford.edu/blog](https://hazyresearch.stanford.edu/blog)
  - [https://jackcook.com/2024/02/23/mamba.html](https://jackcook.com/2024/02/23/mamba.html)


##### 3) Infrastructure (Ring Attention)
- Paper List
    - [Ring Attention with Blockwise Transformers for Near-Infinite Context](https://arxiv.org/pdf/2310.01889)
    - [Blockwise Parallel Transformer for Large Context Models](https://arxiv.org/pdf/2305.19370)
- Implementation:
    - [https://github.com/haoliuhl/ringattention](https://github.com/haoliuhl/ringattention)
    - [https://github.com/zhuzilin/ring-flash-attention](https://github.com/zhuzilin/ring-flash-attention)
    - [https://github.com/jzhang38/EasyContext](https://github.com/jzhang38/EasyContext)
    - [https://github.com/OpenRLHF/OpenRLHF](https://github.com/OpenRLHF/OpenRLHF)
- Blog:
    - [https://zhuanlan.zhihu.com/p/683714620](https://zhuanlan.zhihu.com/p/683714620)

### Long-context Data Synthesis
- Paper List
    - [Data engineering for scaling language models to 128k context](https://arxiv.org/abs/2402.10171)
    - [Effective long-context scaling of foundation models](https://aclanthology.org/2024.naacl-long.260/)
    - [In-context Pretraining: Language Modeling beyond Document Boundaries](https://arxiv.org/pdf/2310.10638)
    - [Extending Llama-3's Context Ten-Fold Overnight](https://arxiv.org/abs/2404.19553)
    - [Quest: Query-centric Data Synthesis Approach for Long-context Scaling of Large Language Model](https://arxiv.org/abs/2405.19846)


### Long-context Model Evaluation
- Paper List
    - [L-Eval: Instituting Standardized Evaluation for Long Context Language Models](https://arxiv.org/pdf/2307.11088)
    - [LongBench: A Bilingual, Multitask Benchmark for Long Context Understanding](https://arxiv.org/pdf/2308.14508)
    - [RULER: What's the Real Context Size of Your Long-Context Language Models?](https://arxiv.org/pdf/2404.06654)
    - [Counting-Stars: A Simple, Efficient, and Reasonable Strategy for Evaluating Long-Context Large Language Models](https://arxiv.org/pdf/2403.11802)
    - [Summary of a Haystack: A Challenge to Long-Context LLMs and RAG Systems](https://arxiv.org/pdf/2407.01370)
    - [Long-form factuality in large language models](https://arxiv.org/pdf/2403.18802)
    - [LongGenBench: Long-context Generation Benchmark](https://arxiv.org/pdf/2410.04199)
    - [L-CiteEval: Do Long-Context Models Truly Leverage Context for Responding?](https://arxiv.org/abs/2410.02115)
- Implementation
    - [LLMTest_NeedleInAHaystack](https://github.com/gkamradt/LLMTest_NeedleInAHaystack)




