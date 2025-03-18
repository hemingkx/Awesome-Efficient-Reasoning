This repository contains a regularly updated paper list for **Efficient Reasoning**.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](./LICENSE) ![GitHub last commit (branch)](https://img.shields.io/github/last-commit/hemingkx/Awesome-Efficient-Reasoning/main?logo=github&color=blue) ![Static Badge](https://img.shields.io/badge/Contributions-welcome-blue.svg?style=flat) 

## Content

- [Keywords Convention](#keywords-convention)
- [Papers](#papers)
  - [Latent Chain-of-Thought](#latent-chain-of-thought)
  - [Chain-of-Thought Compression](#chain-of-thought-compression)
  - [Balanced Chain-of-Thought](#balanced-chain-of-thought)
  - [Reasoning Shortcuts](#reasoning-shortcuts)
  - [Reasoning Step Decomposition](#reasoning-step-decomposition)
  - [Efficient Sampling](#efficient-sampling)
  - [Efficient Self-Consistency](#efficient-self-consistency)
  - [Other Work](#other-work)
  - [Analysis](#analysis)
- [Resources](#resources)
- [Contribution](#contribution)
  - [Contributors](#contributors)
  - [Contributing to this paper list](#contributing-to-this-paper-list)
  

## Keywords Convention

![](https://img.shields.io/badge/COCONUT-blue) Abbreviation

![](https://img.shields.io/badge/ACL2024-orange) Conference

![](https://img.shields.io/badge/Multimodal-green) Main Features

## Papers

### Latent Chain-of-Thought

> For most recent latentCoT research, see [Awesome-Latent-CoT](https://github.com/EIT-NLP/Awesome-Latent-CoT).

- **Think before you speak: Training Language Models With Pause Tokens**  
  *Sachin Goyal, Ziwei Ji, Ankit Singh Rawat, Aditya Krishna Menon, Sanjiv Kumar, Vaishnavh Nagarajan*. [[pdf](https://openreview.net/pdf?id=ph04CRkPdC)], 2023.10. ![](https://img.shields.io/badge/ICLR2024-orange)
- **Guiding Language Model Reasoning with Planning Tokens**  
  *Xinyi Wang, Lucas Caccia, Oleksiy Ostapenko, Xingdi Yuan, William Yang Wang, Alessandro Sordoni*. [[pdf](https://openreview.net/pdf?id=wi9IffRhVM)], 2023.10. ![](https://img.shields.io/badge/COLM2024-orange)
- **Implicit Chain of Thought Reasoning via Knowledge Distillation**   
  *Yuntian Deng, Kiran Prasad, Roland Fernandez, Paul Smolensky, Vishrav Chaudhary, Stuart Shieber*. [[pdf](https://arxiv.org/pdf/2311.01460)], 2023.11. ![](https://img.shields.io/badge/Arxiv-orange)
- **Diffusion of Thoughts: Chain-of-Thought Reasoning in Diffusion Language Models**  
  *Jiacheng Ye, Shansan Gong, Liheng Chen, Lin Zheng, Jiahui Gao, Han Shi, Chuan Wu, Xin Jiang, Zhenguo Li, Wei Bi, Lingpeng Kong*. [[pdf](https://openreview.net/pdf?id=G0v0TxX01N)], 2024.02. ![](https://img.shields.io/badge/NIPS2024-orange) ![](https://img.shields.io/badge/DoT-blue)
- **Let's Think Dot by Dot: Hidden Computation in Transformer Language Models**  
  *Jacob Pfau, William Merrill, Samuel R. Bowman*. [[pdf](https://openreview.net/pdf?id=NikbrdtYvG)], 2024.04. ![](https://img.shields.io/badge/COLM2024-orange) ![](https://img.shields.io/badge/Filler-blue)
- **From Explicit CoT to Implicit CoT: Learning to Internalize CoT Step by Step**  
  *Yuntian Deng, Yejin Choi, Stuart Shieber*. [[pdf](https://arxiv.org/pdf/2405.14838)], 2024.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ImplicitCoT-blue)
- **Expediting and Elevating Large Language Model Reasoning via Hidden Chain-of-Thought Decoding**  
  *Tianqiao Liu, Zui Chen, Zitao Liu, Mi Tian, Weiqi Luo*. [[pdf](https://arxiv.org/pdf/2409.08561)], 2024.09. ![](https://img.shields.io/badge/Arxiv-orange)
- **Do LLMs Really Think Step-by-step In Implicit Reasoning?**  
  *Yijiong Yu*. [[pdf](https://arxiv.org/pdf/2411.15862v3)], 2024.11. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Analysis-green)
- **Disentangling Memory and Reasoning Ability in Large Language Models**   
  *Mingyu Jin, Weidi Luo, Sitao Cheng, Xinyi Wang, Wenyue Hua, Ruixiang Tang, William Yang Wang, Yongfeng Zhang*. [[pdf](https://arxiv.org/pdf/2411.13504)], [[code](https://github.com/MingyuJ666/Disentangling-Memory-and-Reasoning)], 2024.11. ![](https://img.shields.io/badge/Arxiv-orange)
- **Training Large Language Models to Reason in a Continuous Latent Space**  
  *Shibo Hao, Sainbayar Sukhbaatar, DiJia Su, Xian Li, Zhiting Hu, Jason Weston, Yuandong Tian*. [[pdf](https://openreview.net/pdf?id=G0v0TxX01N)], [[code](https://github.com/facebookresearch/coconut)], 2024.12. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/COCONUT-blue)
- **Compressed Chain of Thought: Efficient Reasoning Through Dense Representations**  
  *Jeffrey Cheng, Benjamin Van Durme*. [[pdf](https://arxiv.org/pdf/2412.13171)], 2024.12. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CCoT-blue)
- **Efficient Reasoning with Hidden Thinking**  
  *Xuan Shen, Yizhou Wang, Xiangxi Shi, Yanzhi Wang, Pu Zhao, Jiuxiang Gu*. [[pdf](https://arxiv.org/pdf/2501.19201)], 2025.01. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Heima-blue) ![](https://img.shields.io/badge/Multimodal-green)
- **Inner Thinking Transformer: Leveraging Dynamic Depth Scaling to Foster Adaptive Internal Thinking**  
  *Yilong Chen, Junyuan Shang, Zhenyu Zhang, Yanxi Xie, Jiawei Sheng, Tingwen Liu, Shuohuan Wang, Yu Sun, Hua Wu, Haifeng Wang*. [[pdf](https://arxiv.org/pdf/2502.13842)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ITT-blue)
- **LightThinker: Thinking Step-by-Step Compression**  
  *Jintian Zhang, Yuqi Zhu, Mengshu Sun, Yujie Luo, Shuofei Qiao, Lun Du, Da Zheng, Huajun Chen, Ningyu Zhang*. [[pdf](https://arxiv.org/pdf/2502.15589)], [[code](https://github.com/zjunlp/LightThinker)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/LightThinker-blue)
- **Reasoning with Latent Thoughts: On the Power of Looped Transformers**  
  *Nikunj Saunshi, Nishanth Dikkala, Zhiyuan Li, Sanjiv Kumar, Sashank J. Reddi*. [[pdf](https://openreview.net/pdf?id=din0lGfZFd)], 2025.02. ![](https://img.shields.io/badge/ICLR2025-orange)
- **CODI: Compressing Chain-of-Thought into Continuous Space via Self-Distillation**  
  *Zhenyi Shen, Hanqi Yan, Linhai Zhang, Zhanghao Hu, Yali Du, Yulan He*. [[pdf](https://arxiv.org/pdf/2502.21074)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CODI-blue)
- **Scaling up Test-Time Compute with Latent Reasoning: A Recurrent Depth Approach**  
  *Jonas Geiping, Sean McLeish, Neel Jain, John Kirchenbauer, Siddharth Singh, Brian R. Bartoldson, Bhavya Kailkhura, Abhinav Bhatele, Tom Goldstein*. [[pdf](https://arxiv.org/pdf/2502.05171)], [[code](https://github.com/seal-rg/recurrent-pretraining)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange)
- **LLM Pretraining with Continuous Concepts**  
  *Jihoon Tack, Jack Lanchantin, Jane Yu, Andrew Cohen, Ilia Kulikov, Janice Lan, Shibo Hao, Yuandong Tian, Jason Weston, Xian Li*. [[pdf](https://arxiv.org/pdf/2502.08524)], [[code](https://github.com/facebookresearch/RAM/tree/main/projects/cocomix)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CoCoMix-blue) ![](https://img.shields.io/badge/Pretrain-green)
- **Scalable Language Models with Posterior Inference of Latent Thought Vectors**  
  *Deqian Kong, Minglu Zhao, Dehong Xu, Bo Pang, Shu Wang, Edouardo Honig, Zhangzhang Si, Chuan Li, Jianwen Xie, Sirui Xie, Ying Nian Wu*. [[pdf](https://arxiv.org/pdf/2502.01567)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/LTM-blue)
- **Enhancing Auto-regressive Chain-of-Thought through Loop-Aligned Reasoning**  
  *Qifan Yu, Zhenyu He, Sijie Li, Xun Zhou, Jun Zhang, Jingjing Xu, Di He*. [[pdf](https://arxiv.org/pdf/2502.08482)], [[code](https://github.com/qifanyu/RELAY)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/RELAY-blue)
- **Token Assorted: Mixing Latent and Text Tokens for Improved Language Model Reasoning**  
  *DiJia Su, Hanlin Zhu, Yingchen Xu, Jiantao Jiao, Yuandong Tian, Qinqing Zheng*. [[pdf](https://arxiv.org/pdf/2502.03275)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange)
- **SoftCoT: Soft Chain-of-Thought for Efficient Reasoning with LLMs**  
  *Yige Xu, Xu Guo, Zhiwei Zeng, Chunyan Miao*. [[pdf](https://arxiv.org/pdf/2502.12134)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SoftCoT-blue)
- **Implicit Reasoning in Transformers is Reasoning through Shortcuts**  
  *Tianhe Lin, Jian Xie, Siyu Yuan, Deqing Yang*. [[pdf](https://arxiv.org/pdf/2503.07604)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Analysis-green)

### Chain-of-Thought Compression

- **Chain-of-Symbol Prompting Elicits Planning in Large Langauge Models**  
  *Hanxu Hu, Hongyuan Lu, Huajian Zhang, Yun-Ze Song, Wai Lam, Yue Zhang*. [[pdf](https://arxiv.org/pdf/2305.10276)], [[code](https://github.com/hanxuhu/chain-of-symbol-planning)], 2023.05. ![](https://img.shields.io/badge/Arxiv-orange)
- **C3oT: Generating Shorter Chain-of-Thought without Compromising Effectiveness**  
  *Yu Kang, Xianghui Sun, Liangyu Chen, Wei Zou*. [[pdf](https://arxiv.org/pdf/2412.11664)], 2024.12. ![](https://img.shields.io/badge/AAAI2025-orange) ![](https://img.shields.io/badge/C3oT-blue)
- **Token-Budget-Aware LLM Reasoning**  
  *Tingxu Han, Zhenting Wang, Chunrong Fang, Shiyu Zhao, Shiqing Ma, Zhenyu Chen*. [[pdf](https://arxiv.org/pdf/2412.18547)], [[code](https://github.com/GeniusHTX/TALE)], 2024.12. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/TALE-blue) ![](https://img.shields.io/badge/Prompt-green)
- **CoT-Valve: Length-Compressible Chain-of-Thought Tuning**  
  *Xinyin Ma, Guangnian Wan, Runpeng Yu, Gongfan Fang, Xinchao Wang*. [[pdf](https://arxiv.org/pdf/2502.09601)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CoT--Valve-blue)
- **TokenSkip: Controllable Chain-of-Thought Compression in LLMs**  
  *Heming Xia, Yongqi Li, Chak Tou Leong, Wenjie Wang, Wenjie Li*. [[pdf](https://arxiv.org/pdf/2502.12067)], [[code](https://github.com/hemingkx/TokenSkip)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/TokenSkip-blue) ![](https://img.shields.io/badge/Controllable_Compression-green)
- **Self-Training Elicits Concise Reasoning in Large Language Models**  
  *Tergel Munkhbat, Namgyu Ho, Seo Hyun Kim, Yongjin Yang, Yujin Kim, Se-Young Yun*. [[pdf](https://arxiv.org/pdf/2502.20122)], [[code](https://github.com/TergelMunkhbat/concise-reasoning)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange)
- **Chain of Draft: Thinking Faster by Writing Less**  
  *Silei Xu, Wenhao Xie, Lingxiao Zhao, Pengcheng He*. [[pdf](https://arxiv.org/pdf/2502.18600)], [[code](https://github.com/sileix/chain-of-draft)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CoD-blue) ![](https://img.shields.io/badge/Prompt-green)
- **How Well do LLMs Compress Their Own Chain-of-Thought? A Token Complexity Approach**  
  *Ayeong Lee, Ethan Che, Tianyi Peng*. [[pdf](https://arxiv.org/pdf/2503.01141)], [[code](https://github.com/Compressed-CoT/compressed-cot)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Prompt-green)
- **Sketch-of-Thought: Efficient LLM Reasoning with Adaptive Cognitive-Inspired Sketching**  
  *Simon A. Aytes, Jinheon Baek, Sung Ju Hwang*. [[pdf](https://arxiv.org/pdf/2503.05179)], [[code](https://github.com/SimonAytes/SoT)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SoT-blue) ![](https://img.shields.io/badge/Prompt-green)

### Balanced Chain-of-Thought

> Balanced CoT allocates more compute to hard questions, reduces compute for simpler ones.

- **Efficiently Serving LLM Reasoning Programs with Certaindex**  
  *Yichao Fu, Junda Chen, Siqi Zhu, Zheyu Fu, Zhongdongming Dai, Aurick Qiao, Hao Zhang*. [[pdf](https://arxiv.org/pdf/2412.20993)], 2024.12. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Dynasor-blue)
- **O1-Pruner: Length-Harmonizing Fine-Tuning for O1-Like Reasoning Pruning**  
  *Haotian Luo, Li Shen, Haiying He, Yibo Wang, Shiwei Liu, Wei Li, Naiqiang Tan, Xiaochun Cao, Dacheng Tao*. [[pdf](https://arxiv.org/pdf/2501.12570)], [[code](https://github.com/StarDewXXX/O1-Pruner)], 2025.01. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/O1--Pruner-blue)
- **Kimi k1.5: Scaling Reinforcement Learning with LLMs**  
  *Kimi Team*. [[pdf](https://arxiv.org/pdf/2501.12599)], 2025.01. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Kimi_k1.5-blue)
- **Training Language Models to Reason Efficiently**  
  *Daman Arora, Andrea Zanette*. [[pdf](https://arxiv.org/pdf/2502.04463)], [[code](https://github.com/Zanette-Labs/efficient-reasoning)], [[homepage](https://zanette-labs.github.io/efficient-reasoning/)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange)
- **Meta-Reasoner: Dynamic Guidance for Optimized Inference-time Reasoning in Large Language Models**  
  *Yuan Sui, Yufei He, Tri Cao, Simeng Han, Bryan Hooi*. [[pdf](https://arxiv.org/pdf/2502.19918)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Meta--Reasoner-blue)
- **DAST: Difficulty-Adaptive Slow-Thinking for Large Reasoning Models**  
  *Yi Shen, Jian Zhang, Jieyun Huang, Shuming Shi, Wenjing Zhang, Jiangze Yan, Ning Wang, Kai Wang, Shiguo Lian*. [[pdf](https://arxiv.org/pdf/2503.04472)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DAST-blue)

### Reasoning Shortcuts

- **Not All Neuro-Symbolic Concepts Are Created Equal: Analysis and Mitigation of Reasoning Shortcuts**  
  *Emanuele Marconato, Stefano Teso, Antonio Vergari, Andrea Passerini*. [[pdf](https://arxiv.org/pdf/2305.19951)], 2023.05. ![](https://img.shields.io/badge/NIPS2023-orange)
- **Break the Chain: Large Language Models Can be Shortcut Reasoners**  
  *Mengru Ding, Hanmeng Liu, Zhizhang Fu, Jian Song, Wenbo Xie, Yue Zhang*. [[pdf](https://arxiv.org/pdf/2406.06580)], 2024.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Break_the_Chain-blue)
- **Can Language Models Learn to Skip Steps?**  
  *Tengxiao Liu, Qipeng Guo, Xiangkun Hu, Cheng Jiayang, Yue Zhang, Xipeng Qiu, Zheng Zhang*. [[pdf](https://arxiv.org/pdf/2411.01855)], [[code](https://github.com/tengxiaoliu/LM_skip)], 2024.11. ![](https://img.shields.io/badge/NIPS2024-orange) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **TokenSkip: Controllable Chain-of-Thought Compression in LLMs**  
  *Heming Xia, Yongqi Li, Chak Tou Leong, Wenjie Wang, Wenjie Li*. [[pdf](https://arxiv.org/pdf/2502.12067)], [[code](https://github.com/hemingkx/TokenSkip)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/TokenSkip-blue) ![](https://img.shields.io/badge/Token_Shortcut-green)
- **Stepwise Perplexity-Guided Refinement for Efficient Chain-of-Thought Reasoning in Large Language Models**  
  *Yingqian Cui, Pengfei He, Jingying Zeng, Hui Liu, Xianfeng Tang, Zhenwei Dai, Yan Han, Chen Luo, Jing Huang, Zhen Li, Suhang Wang, Yue Xing, Jiliang Tang, Qi He*. [[pdf](https://arxiv.org/pdf/2502.13260)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Step_Shortcut-green)

### Reasoning Step Decomposition

- **Markov Chain of Thought for Efficient Mathematical Reasoning**  
  *Wen Yang, Minpeng Liao, Kai Fan*. [[pdf](https://arxiv.org/pdf/2410.17635)], [[code](https://github.com/james-yw/Markov-Chain-of-Thought)], 2024.10. ![](https://img.shields.io/badge/NAACL2025-orange) ![](https://img.shields.io/badge/MCoT-blue) ![](https://img.shields.io/badge/Intermediate_CoT_Summarization-green)
- **Atom of Thoughts for Markov LLM Test-Time Scaling**  
  *Fengwei Teng, Zhaoyang Yu, Quan Shi, Jiayi Zhang, Chenglin Wu, Yuyu Luo*. [[pdf](https://arxiv.org/pdf/2502.12018)], [[code](https://github.com/qixucen/atom)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/AoT-blue)
- **DISC: Dynamic Decomposition Improves LLM Inference Scaling**  
  *Jonathan Light, Wei Cheng, Wu Yue, Masafumi Oyamada, Mengdi Wang, Santiago Paternain, Haifeng Chen*. [[pdf](https://arxiv.org/pdf/2502.16706)], 2025.02. ![](https://img.shields.io/badge/ICLR2025_SSI--FM_workshop-orange) ![](https://img.shields.io/badge/DISC-blue)
- **Can Atomic Step Decomposition Enhance the Self-structured Reasoning of Multimodal Large Models?**  
  *Kun Xiang, Zhili Liu, Zihao Jiang, Yunshuang Nie, Kaixin Cai, Yiyang Yin, Runhui Huang, Haoxiang Fan, Hanhui Li, Weiran Huang, Yihan Zeng, Yu-Jie Yuan, Jianhua Han, Lanqing Hong, Hang Xu, Xiaodan Liang*. [[pdf](https://arxiv.org/pdf/2503.06252)], [[code](https://github.com/Quinn777/AtomThink)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SCoT-blue) ![](https://img.shields.io/badge/Multimodal-green)

### Efficient Sampling

- **Fast Best-of-N Decoding via Speculative Rejection**  
  *Hanshi Sun, Momin Haider, Ruiqi Zhang, Huitao Yang, Jiahao Qiu, Ming Yin, Mengdi Wang, Peter Bartlett, Andrea Zanette*. [[pdf](https://openreview.net/pdf?id=348hfcprUs)], [[code](https://github.com/Zanette-Labs/SpeculativeRejection)], 2024.10. ![](https://img.shields.io/badge/NIPS2024-orange) ![](https://img.shields.io/badge/Speculative_Rejection-blue)
- **Non-myopic Generation of Language Models for Reasoning and Planning**  
  *Chang Ma, Haiteng Zhao, Junlei Zhang, Junxian He, Lingpeng Kong*. [[pdf](https://openreview.net/forum?id=OoNazl6T7D)], [[code](https://github.com/chang-github-00/LLM-Predictive-Decoding)], 2024.10. ![](https://img.shields.io/badge/ICLR2025-orange) ![](https://img.shields.io/badge/Predictive--Decoding-blue)
- **FastMCTS: A Simple Sampling Strategy for Data Synthesis**  
  *Peiji Li, Kai Lv, Yunfan Shao, Yichuan Ma, Linyang Li, Xiaoqing Zheng, Xipeng Qiu, Qipeng Guo*. [[pdf](https://www.arxiv.org/pdf/2502.11476)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/FastMCTS-blue)
- **Dynamic Parallel Tree Search for Efficient LLM Reasoning**  
  *Yifu Ding, Wentao Jiang, Shunyu Liu, Yongcheng Jing, Jinyang Guo, Yingjie Wang, Jing Zhang, Zengmao Wang, Ziwei Liu, Bo Du, Xianglong Liu, Dacheng Tao*. [[pdf](https://arxiv.org/pdf/2502.16235)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DPTS-blue)
- **Sampling-Efficient Test-Time Scaling: Self-Estimating the Best-of-N Sampling in Early Decoding**  
  *Yiming Wang, Pei Zhang, Siyuan Huang, Baosong Yang, Zhuosheng Zhang, Fei Huang, Rui Wang*. [[pdf](https://arxiv.org/pdf/2503.01422)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ST--BoN-blue)
- **Language Models can Self-Improve at State-Value Estimation for Better Search**  
  *Ethan Mendes, Alan Ritter*. [[pdf](https://arxiv.org/pdf/2503.02878)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--taught_Lookahead-blue)
- **ϕ-Decoding: Adaptive Foresight Sampling for Balanced Inference-Time Exploration and Exploitation**  
  *Fangzhi Xu, Hang Yan, Chang Ma, Haiteng Zhao, Jun Liu, Qika Lin, Zhiyong Wu*. [[pdf](https://arxiv.org/pdf/2503.13288)], [[code](https://github.com/xufangzhi/phi-Decoding)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ϕ--Decoding-blue)

### Efficient Self-Consistency

- **Escape Sky-high Cost: Early-stopping Self-Consistency for Multi-step Reasoning**  
  *Yiwei Li, Peiwen Yuan, Shaoxiong Feng, Boyuan Pan, Xinglin Wang, Bin Sun, Heda Wang, Kan Li*. [[pdf](https://openreview.net/pdf?id=ndR8Ytrzhh)], [[code](https://github.com/Yiwei98/ESC)], 2024.01. ![](https://img.shields.io/badge/ICLR2024-orange) ![](https://img.shields.io/badge/ESC-blue)
- **Make Every Penny Count: Difficulty-Adaptive Self-Consistency for Cost-Efficient Reasoning**  
  *Xinglin Wang, Shaoxiong Feng, Yiwei Li, Peiwen Yuan, Yueqi Zhang, Chuyi Tan, Boyuan Pan, Yao Hu, Kan Li*. [[pdf](https://arxiv.org/pdf/2408.13457)], [[code](https://github.com/WangXinglin/DSC)], 2024.08. ![](https://img.shields.io/badge/NAACL2025--Findings-orange) ![](https://img.shields.io/badge/DSC-blue)
- **Path-Consistency: Prefix Enhancement for Efficient Inference in LLM**  
  *Jiace Zhu, Yingtao Shen, Jie Zhao, An Zou*. [[pdf](https://arxiv.org/pdf/2409.01281)], 2024.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Path--Consistency-blue)
- **Reasoning Aware Self-Consistency: Leveraging Reasoning Paths for Efficient LLM Sampling**  
  *Guangya Wan, Yuqi Wu, Jie Chen, Sheng Li*. [[pdf](https://arxiv.org/pdf/2408.17017)], [[code](https://github.com/wan19990901/RASC/tree/Submission_Code)], 2024.08. ![](https://img.shields.io/badge/NAACL2025-orange) ![](https://img.shields.io/badge/RASC-blue)
- **Efficient Test-Time Scaling via Self-Calibration**  
  *Chengsong Huang, Langlin Huang, Jixuan Leng, Jiacheng Liu, Jiaxin Huang*. [[pdf](https://arxiv.org/pdf/2503.00031)], [[code](https://github.com/Chengsong-Huang/Self-Calibration)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--Calibration-blue)
- **Confidence Improves Self-Consistency in LLMs**  
  *Amir Taubenfeld, Tom Sheffer, Eran Ofek, Amir Feder, Ariel Goldstein, Zorik Gekhman, Gal Yona*. [[pdf](https://arxiv.org/pdf/2502.06233)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CISC-blue)
- **Bridging Internal Probability and Self-Consistency for Effective and Efficient LLM Reasoning**  
  *Zhi Zhou, Tan Yuhao, Zenan Li, Yuan Yao, Lan-Zhe Guo, Xiaoxing Ma, Yu-Feng Li*. [[pdf](https://arxiv.org/pdf/2502.00511)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/RPC-blue)

### Other Work

- **Thinking Slow, Fast: Scaling Inference Compute with Distilled Reasoners**  
  *Daniele Paliotta, Junxiong Wang, Matteo Pagliardini, Kevin Y. Li, Aviv Bick, J. Zico Kolter, Albert Gu, François Fleuret, Tri Dao*. [[pdf](https://arxiv.org/pdf/2502.20339)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CoT_Distillation-green)
- **Unveiling the Key Factors for Distilling Chain-of-Thought Reasoning**  
  *Xinghao Chen, Zhijing Sun, Wenjin Guo, Miaoran Zhang, Yanjun Chen, Yirong Sun, Hui Su, Yijie Pan, Dietrich Klakow, Wenjie Li, Xiaoyu Shen*. [[pdf](https://arxiv.org/pdf/2502.18001)], [[code](https://github.com/EIT-NLP/Distilling-CoT-Reasoning)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CoT_Distillation-green)
- **Skeleton-of-Thought: Large Language Models Can Do Parallel Decoding**  
  *Xuefei Ning, Zinan Lin, Zixuan Zhou, Zifu Wang, Huazhong Yang, Yu Wang*. [[pdf](https://openreview.net/pdf?id=mqVgBbNCm9)], [[code](https://github.com/imagination-research/sot)], [[homepage](https://sites.google.com/view/sot-llm)], 2023.06. ![](https://img.shields.io/badge/ICLR2024-orange) ![](https://img.shields.io/badge/SoT-blue) ![](https://img.shields.io/badge/Parallel_CoT-green)
- **Adaptive Skeleton Graph Decoding**  
  *Shuowei Jin, Yongji Wu, Haizhong Zheng, Qingzhao Zhang, Matthew Lentz, Z. Morley Mao, Atul Prakash, Feng Qian, Danyang Zhuo*. [[pdf](https://arxiv.org/pdf/2402.12280)], 2024.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Parallel_CoT-green)
- **Reward-Guided Speculative Decoding for Efficient LLM Reasoning**  
  *Baohao Liao, Yuhui Xu, Hanze Dong, Junnan Li, Christof Monz, Silvio Savarese, Doyen Sahoo, Caiming Xiong*. [[pdf](https://arxiv.org/pdf/2501.19324)], [[code](https://github.com/BaohaoLiao/RSD)], 2025.01. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/RSD-blue) ![](https://img.shields.io/badge/Speculative_Decoding-green)
- **InftyThink: Breaking the Length Limits of Long-Context Reasoning in Large Language Models**  
  *Yuchen Yan, Yongliang Shen, Yang Liu, Jin Jiang, Mengdi Zhang, Jian Shao, Yueting Zhuang*. [[pdf](https://arxiv.org/pdf/2503.06692)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/InftyThink-blue) ![](https://img.shields.io/badge/Intermediate_CoT_Summarization-green)
- **L1: Controlling How Long A Reasoning Model Thinks With Reinforcement Learning**  
  *Pranjal Aggarwal, Sean Welleck*. [[pdf](https://www.arxiv.org/pdf/2503.04697)], [[code](https://github.com/cmu-l3/l1)], [[homepage](https://cmu-l3.github.io/l1/)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/L1-blue) ![](https://img.shields.io/badge/Length_Control-green)

### Analysis

- **Do NOT Think That Much for 2+3=? On the Overthinking of o1-Like LLMs**  
  *Xingyu Chen, Jiahao Xu, Tian Liang, Zhiwei He, Jianhui Pang, Dian Yu, Linfeng Song, Qiuzhi Liu, Mengfei Zhou, Zhuosheng Zhang, Rui Wang, Zhaopeng Tu, Haitao Mi, Dong Yu*. [[pdf](https://arxiv.org/pdf/2412.21187)], 2024.12. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Over--thinking-green)
- **Towards Thinking-Optimal Scaling of Test-Time Compute for LLM Reasoning**  
  *Wenkai Yang, Shuming Ma, Yankai Lin, Furu Wei*. [[pdf](https://arxiv.org/pdf/2502.18080)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Over--thinking-green)
- **Thoughts Are All Over the Place: On the Underthinking of o1-Like LLMs**  
  *Yue Wang, Qiuzhi Liu, Jiahao Xu, Tian Liang, Xingyu Chen, Zhiwei He, Linfeng Song, Dian Yu, Juntao Li, Zhuosheng Zhang, Rui Wang, Zhaopeng Tu, Haitao Mi, Dong Yu*. [[pdf](https://arxiv.org/pdf/2501.18585)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Under--thinking-green)
- **The Relationship Between Reasoning and Performance in Large Language Models -- o3 (mini) Thinks Harder, Not Longer**  
  *Marthe Ballon, Andres Algaba, Vincent Ginis*. [[pdf](https://arxiv.org/pdf/2502.15631)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange)

## Resources

**Reading lists related to Efficient Reasoning**

- [Blueyee/Efficient-CoT-LRMs](https://github.com/Blueyee/Efficient-CoT-LRMs)
- [Hongcheng-Gao/Awesome-Long2short-on-LRMs](https://github.com/Hongcheng-Gao/Awesome-Long2short-on-LRMs)
- [EIT-NLP/Awesome-Latent-CoT](https://github.com/EIT-NLP/Awesome-Latent-CoT)
- [yzhangchuck/awesome-llm-reasoning-long2short-papers](https://github.com/yzhangchuck/awesome-llm-reasoning-long2short-papers)

## Contributors

<a href="https://github.com/hemingkx/Awesome-Efficient-Reasoning/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=hemingkx/Awesome-Efficient-Reasoning" />
</a>

## Contributing to this paper list

-  There are cases where we miss important works in this field, please feel free to contribute and promote your awesome work or other related works here! Thanks for the efforts in advance.

