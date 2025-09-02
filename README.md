This repository contains a regularly updated paper list for **Efficient Reasoning**.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![License](https://img.shields.io/badge/License-Apache_2.0-green.svg)](./LICENSE) ![GitHub last commit (branch)](https://img.shields.io/github/last-commit/hemingkx/Awesome-Efficient-Reasoning/main?logo=github&color=blue) ![Static Badge](https://img.shields.io/badge/Contributions-welcome-blue.svg?style=flat) 

## Content

- [Keywords Convention](#keywords-convention)
- [Papers](#papers)
  - [Survey](#survey)
  - [Efficient Training](#efficient-training)
  - [Latent Chain-of-Thought](#latent-chain-of-thought)
  - [Long-to-Short Chain-of-Thought](#long-to-short-chain-of-thought)
  - [Adaptive Thinking](#adaptive-thinking)
  - [Reasoning Shortcuts](#reasoning-shortcuts)
  - [Reasoning Step Decomposition](#reasoning-step-decomposition)
  - [Small Reasoning Models & CoT Distillation](#small-reasoning-models--cot-distillation)
  - [Small & Large Reasoning Model Collaboration](#small--large-reasoning-model-collaboration)
  - [Speculative Decoding for CoT Efficiency](#speculative-decoding-for-cot-efficiency)
  - [Sparse Attention & KV Cache](#sparse-attention--kv-cache)
  - [Optimal Test-Time Scaling](#optimal-test-time-scaling)
  - [Efficient Sampling](#efficient-sampling)
  - [Efficient Self-Consistency](#efficient-self-consistency)
  - [Long-Context Reasoning Efficiency](#long-context-reasoning-efficiency)
  - [Multimodal Reasoning Efficiency](#multimodal-reasoning-efficiency)
  - [Other Work](#other-work)
  - [Benchmarks](#benchmarks)
  - [Analysis](#analysis)
  - [Applications](#applications)
- [Blogs](#blog--project)
- [Talks](#talks)
- [Resources](#resources)
- [Contribution](#contribution)
  - [Contributors](#contributors)
  - [Contributing to this paper list](#contributing-to-this-paper-list)


## Keywords Convention

![](https://img.shields.io/badge/COCONUT-blue) Abbreviation

![](https://img.shields.io/badge/ACL2024-orange) Conference

![](https://img.shields.io/badge/Multimodal-green) Main Features

## Papers

### Survey

- **Stop Overthinking: A Survey on Efficient Reasoning for Large Language Models**  
  *Yang Sui, Yu-Neng Chuang, Guanchu Wang, Jiamu Zhang, Tianyi Zhang, Jiayi Yuan, Hongyi Liu, Andrew Wen, Shaochen (Henry) Zhong, Hanjie Chen, Xia Hu*. [[pdf](https://arxiv.org/pdf/2503.16419)], [[paper list](https://github.com/Eclipsess/Awesome-Efficient-Reasoning-LLMs)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange)
- **A Survey of Efficient Reasoning for Large Reasoning Models: Language, Multimodality, and Beyond**  
  *Xiaoye Qu, Yafu Li, Zhaochen Su, Weigao Sun, Jianhao Yan, Dongrui Liu, Ganqu Cui, Daizong Liu, Shuxian Liang, Junxian He, Peng Li, Wei Wei, Jing Shao, Chaochao Lu, Yue Zhang, Xian-Sheng Hua, Bowen Zhou, Yu Cheng*. [[pdf](https://arxiv.org/pdf/2503.21614)], [[paper list](https://github.com/XiaoYee/Awesome_Efficient_LRM_Reasoning)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange)
- **Efficient Inference for Large Reasoning Models: A Survey**  
  *Yue Liu, Jiaying Wu, Yufei He, Hongcheng Gao, Hongyu Chen, Baolong Bi, Jiaheng Zhang, Zhiqi Huang, Bryan Hooi*. [[pdf](https://arxiv.org/pdf/2503.23077)], [[paper list](https://github.com/yueliu1999/Awesome-Efficient-Inference-for-LRMs)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange)
- **Harnessing the Reasoning Economy: A Survey of Efficient Reasoning for Large Language Models**  
  *Rui Wang, Hongru Wang, Boyang Xue, Jianhui Pang, Shudong Liu, Yi Chen, Jiahao Qiu, Derek Fai Wong, Heng Ji, Kam-Fai Wong*. [[pdf](https://arxiv.org/pdf/2503.24377)], [[paper list](https://github.com/DevoAllen/Awesome-Reasoning-Economy-Papers)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange)
- **Efficient Reasoning Models: A Survey**  
  *Sicheng Feng, Gongfan Fang, Xinyin Ma, Xinchao Wang*. [[pdf](https://arxiv.org/pdf/2504.10903)], [[paper list](https://github.com/fscdc/Awesome-Efficient-Reasoning-Models)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange)
- **Reasoning Beyond Language: A Comprehensive Survey on Latent Chain-of-Thought Reasoning**  
  *Xinghao Chen, Anhao Zhao, Heming Xia, Xuan Lu, Hanlin Wang, Yanjun Chen, Wei Zhang, Jian Wang, Wenjie Li, Xiaoyu Shen*. [[pdf](https://arxiv.org/pdf/2505.16782)], [[paper list](https://github.com/EIT-NLP/Awesome-Latent-CoT)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange)
- **Reasoning on a Budget: A Survey of Adaptive and Controllable Test-Time Compute in LLMs**  
  *Mohammad Ali Alomrani, Yingxue Zhang, Derek Li, Qianyi Sun, Soumyasundar Pal, Zhanguang Zhang, Yaochen Hu, Rohan Deepak Ajwani, Antonios Valkanas, Raika Karimi, Peng Cheng, Yunzhou Wang, Pengyi Liao, Hanrui Huang, Bin Wang, Jianye Hao, Mark Coates*. [[pdf](https://arxiv.org/pdf/2507.02076)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange)
- **A Survey on Latent Reasoning**  
  *Rui-Jie Zhu, Tianhao Peng, Tianhao Cheng, Xingwei Qu, Jinfa Huang, Dawei Zhu, Hao Wang, Kaiwen Xue, Xuanliang Zhang, Yong Shan, Tianle Cai, Taylor Kergan, Assel Kembay, Andrew Smith, Chenghua Lin, Binh Nguyen, Yuqi Pan, Yuhong Chou, Zefan Cai, Zhenhe Wu, Yongchi Zhao, Tianyu Liu, Jian Yang, Wangchunshu Zhou, Chujie Zheng, Chongxuan Li, Yuyin Zhou, Zhoujun Li, Zhaoxiang Zhang, Jiaheng Liu, Ge Zhang, Wenhao Huang, Jason Eshraghian*. [[pdf](https://arxiv.org/pdf/2507.06203)], [[paper list](https://github.com/multimodal-art-projection/LatentCoT-Horizon/)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange)
- **Towards Concise and Adaptive Thinking in Large Reasoning Models: A Survey**  
  *Jason Zhu, Hongyu Li*. [[pdf](https://arxiv.org/pdf/2507.09662)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange)
- **Don't Overthink It: A Survey of Efficient R1-style Large Reasoning Models**  
  *Linan Yue, Yichao Du, Yizhi Wang, Weibo Gao, Fangzhou Yao, Li Wang, Ye Liu, Ziyu Xu, Qi Liu, Shimin Di, Min-Ling Zhang*. [[pdf](https://arxiv.org/pdf/2508.02120)], [[paper list](https://github.com/yuelinan/Awesome-Efficient-R1-style-LRMs)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange)

### Efficient Training

- **s1: Simple test-time scaling**  
  *Niklas Muennighoff, Zitong Yang, Weijia Shi, Xiang Lisa Li, Li Fei-Fei, Hannaneh Hajishirzi, Luke Zettlemoyer, Percy Liang, Emmanuel Candès, Tatsunori Hashimoto*. [[pdf](https://arxiv.org/pdf/2501.19393)], [[code](https://github.com/simplescaling/s1)], 2025.01. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/s1-blue)
- **LIMO: Less is More for Reasoning**  
  *Yixin Ye, Zhen Huang, Yang Xiao, Ethan Chern, Shijie Xia, Pengfei Liu*. [[pdf](https://arxiv.org/pdf/2502.03387)], [[code](https://github.com/GAIR-NLP/LIMO)], 2025.02. ![](https://img.shields.io/badge/COLM2025-orange) ![](https://img.shields.io/badge/LIMO-blue)
- **Light-R1: Curriculum SFT, DPO and RL for Long COT from Scratch and Beyond**  
  *Liang Wen, Yunke Cai, Fenrui Xiao, Xin He, Qi An, Zhenyu Duan, Yimin Du, Junchen Liu, Lifu Tang, Xiaowei Lv, Haosheng Zou, Yongchao Deng, Shousheng Jia, Xiangzheng Zhang*. [[pdf](https://aclanthology.org/2025.acl-industry.24/)], [[code](https://github.com/Qihoo360/Light-R1)], 2025.03. ![](https://img.shields.io/badge/ACL2025--industry-orange) ![](https://img.shields.io/badge/Light--R1-blue)
- **DAPO: An Open-Source LLM Reinforcement Learning System at Scale**  
  *Qiying Yu, Zheng Zhang, Ruofei Zhu, Yufeng Yuan, Xiaochen Zuo, Yu Yue, Tiantian Fan, Gaohong Liu, Lingjun Liu, Xin Liu, Haibin Lin, Zhiqi Lin, Bole Ma, Guangming Sheng, Yuxuan Tong, Chi Zhang, Mofan Zhang, Wang Zhang, Hang Zhu, Jinhua Zhu, Jiaze Chen, Jiangjie Chen, Chengyi Wang, Hongli Yu, Weinan Dai, Yuxuan Song, Xiangpeng Wei, Hao Zhou, Jingjing Liu, Wei-Ying Ma, Ya-Qin Zhang, Lin Yan, Mu Qiao, Yonghui Wu, Mingxuan Wang*. [[pdf](https://arxiv.org/pdf/2503.14476)], [[code](https://github.com/BytedTsinghua-SIA/DAPO)], [[homepage](https://dapo-sia.github.io/)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DAPO-blue)
- **FastCuRL: Curriculum Reinforcement Learning with Progressive Context Extension for Efficient Training R1-like Reasoning Models**  
  *Mingyang Song, Mao Zheng, Zheng Li, Wenjie Yang, Xuan Luo, Yue Pan, Feng Zhang*. [[pdf](https://arxiv.org/pdf/2503.17287)], [[code](https://github.com/nick7nlp/FastCuRL)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/FastCuRL-blue)
- **Understanding R1-Zero-Like Training: A Critical Perspective**  
  *Zichen Liu, Changyu Chen, Wenjun Li, Penghui Qi, Tianyu Pang, Chao Du, Wee Sun Lee, Min Lin*. [[pdf](https://arxiv.org/pdf/2503.20783)], [[code](https://github.com/sail-sg/understand-r1-zero)], 2025.03. ![](https://img.shields.io/badge/COLM2025-orange) ![](https://img.shields.io/badge/Dr.GRPO-blue)
- **Trajectory Balance with Asynchrony: Decoupling Exploration and Learning for Fast, Scalable LLM Post-Training**  
  *Brian R. Bartoldson, Siddarth Venkatraman, James Diffenderfer, Moksh Jain, Tal Ben-Nun, Seanie Lee, Minsu Kim, Johan Obando-Ceron, Yoshua Bengio, Bhavya Kailkhura*. [[pdf](https://arxiv.org/pdf/2503.18929)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/TBA-blue)
- **CPPO: Accelerating the Training of Group Relative Policy Optimization-Based Reasoning Models**  
  *Zhihang Lin, Mingbao Lin, Yuan Xie, Rongrong Ji*. [[pdf](https://arxiv.org/pdf/2503.22342)], [[code](https://github.com/lzhxmu/CPPO)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CPPO-blue)
- **Efficient Reinforcement Finetuning via Adaptive Curriculum Learning**  
  *Taiwei Shi, Yiyang Wu, Linxin Song, Tianyi Zhou, Jieyu Zhao*. [[pdf](https://arxiv.org/pdf/2504.05520)], [[code](https://github.com/uscnlp-lime/verl)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ADARFT-blue)
- **VAPO: Efficient and Reliable Reinforcement Learning for Advanced Reasoning Tasks**  
  *Yu Yue, Yufeng Yuan, Qiying Yu, Xiaochen Zuo, Ruofei Zhu, Wenyuan Xu, Jiaze Chen, Chengyi Wang, TianTian Fan, Zhengyin Du, Xiangpeng Wei, Xiangyu Yu, Gaohong Liu, Juncai Liu, Lingjun Liu, Haibin Lin, Zhiqi Lin, Bole Ma, Chi Zhang, Mofan Zhang, Wang Zhang, Hang Zhu, Ru Zhang, Xin Liu, Mingxuan Wang, Yonghui Wu, Lin Yan*. [[pdf](https://arxiv.org/pdf/2504.05118)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/VAPO-blue)
- **Accelerating RL for LLM Reasoning with Optimal Advantage Regression**  
  *Kianté Brantley, Mingyu Chen, Zhaolin Gao, Jason D. Lee, Wen Sun, Wenhao Zhan, Xuezhou Zhang*. [[pdf](https://arxiv.org/pdf/2505.20686)], [[code](https://github.com/ZhaolinGao/A-PO)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/A*--PO-blue)
- **Beyond the 80/20 Rule: High-Entropy Minority Tokens Drive Effective Reinforcement Learning for LLM Reasoning**  
  *Shenzhi Wang, Le Yu, Chang Gao, Chujie Zheng, Shixuan Liu, Rui Lu, Kai Dang, Xionghui Chen, Jianxin Yang, Zhenru Zhang, Yuqiong Liu, An Yang, Andrew Zhao, Yang Yue, Shiji Song, Bowen Yu, Gao Huang, Junyang Lin*. [[pdf](https://arxiv.org/pdf/2506.01939)], [[homepage](https://shenzhi-wang.github.io/high-entropy-minority-tokens-rlvr/)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Training_with_High--Entropy_Tokens-green)
- **Act Only When It Pays: Efficient Reinforcement Learning for LLM Reasoning via Selective Rollouts**  
  *Haizhong Zheng, Yang Zhou, Brian R. Bartoldson, Bhavya Kailkhura, Fan Lai, Jiawei Zhao, Beidi Chen*. [[pdf](https://arxiv.org/pdf/2506.02177)], [[homepage](https://infini-ai-lab.github.io/GRESO/)], [[code](https://github.com/Infini-AI-Lab/GRESO)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Selective_Rollouts-green)
- **EPiC: Towards Lossless Speedup for Reasoning Training through Edge-Preserving CoT Condensation**  
  *Jinghan Jia, Hadi Reisizadeh, Chongyu Fan, Nathalie Baracaldo, Mingyi Hong, Sijia Liu*. [[pdf](https://arxiv.org/pdf/2506.04205)], [[code](https://github.com/OPTML-Group/EPiC)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/EPiC-blue) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **SPEED-RL: Faster Training of Reasoning Models via Online Curriculum Learning**  
  *Ruiqi Zhang, Daman Arora, Song Mei, Andrea Zanette*. [[pdf](https://arxiv.org/pdf/2506.09016)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SPEED--RL-blue)
- **Truncated Proximal Policy Optimization**  
  *Tiantian Fan, Lingjun Liu, Yu Yue, Jiaze Chen, Chengyi Wang, Qiying Yu, Chi Zhang, Zhiqi Lin, Ruofei Zhu, Yufeng Yuan, Xiaochen Zuo, Bole Ma, Mofan Zhang, Gaohong Liu, Ru Zhang, Haotian Zhou, Cong Xie, Ruidong Zhu, Zhi Zhang, Xin Liu, Mingxuan Wang, Lin Yan, Yonghui Wu*. [[pdf](https://arxiv.org/pdf/2506.15050)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/T--PPO-blue)
- **QFFT, Question-Free Fine-Tuning for Adaptive Reasoning**  
  *Wanlong Liu, Junxiao Xu, Fei Yu, Yukang Lin, Ke Ji, Wenyu Chen, Yan Xu, Yasheng Wang, Lifeng Shang, Benyou Wang*. [[pdf](https://arxiv.org/pdf/2506.12860)], [[code](https://github.com/LWL-cpu/Question-Free-Fine-Tuning)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/QFFT-blue)

### Latent Chain-of-Thought

- **Reasoning Beyond Language: A Comprehensive Survey on Latent Chain-of-Thought Reasoning**  
  *Xinghao Chen, Anhao Zhao, Heming Xia, Xuan Lu, Hanlin Wang, Yanjun Chen, Wei Zhang, Jian Wang, Wenjie Li, Xiaoyu Shen*. [[pdf](https://arxiv.org/pdf/2505.16782)], [[paper list](https://github.com/EIT-NLP/Awesome-Latent-CoT)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Survey-green)
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
  *Yilong Chen, Junyuan Shang, Zhenyu Zhang, Yanxi Xie, Jiawei Sheng, Tingwen Liu, Shuohuan Wang, Yu Sun, Hua Wu, Haifeng Wang*. [[pdf](https://arxiv.org/pdf/2502.13842)], 2025.02. ![](https://img.shields.io/badge/ACL2025-orange) ![](https://img.shields.io/badge/ITT-blue)
- **LightThinker: Thinking Step-by-Step Compression**  
  *Jintian Zhang, Yuqi Zhu, Mengshu Sun, Yujie Luo, Shuofei Qiao, Lun Du, Da Zheng, Huajun Chen, Ningyu Zhang*. [[pdf](https://arxiv.org/pdf/2502.15589)], [[code](https://github.com/zjunlp/LightThinker)], 2025.02. ![](https://img.shields.io/badge/EMNLP2025-orange) ![](https://img.shields.io/badge/LightThinker-blue)
- **Reasoning with Latent Thoughts: On the Power of Looped Transformers**  
  *Nikunj Saunshi, Nishanth Dikkala, Zhiyuan Li, Sanjiv Kumar, Sashank J. Reddi*. [[pdf](https://openreview.net/pdf?id=din0lGfZFd)], 2025.02. ![](https://img.shields.io/badge/ICLR2025-orange)
- **CODI: Compressing Chain-of-Thought into Continuous Space via Self-Distillation**  
  *Zhenyi Shen, Hanqi Yan, Linhai Zhang, Zhanghao Hu, Yali Du, Yulan He*. [[pdf](https://arxiv.org/pdf/2502.21074)], 2025.02. ![](https://img.shields.io/badge/EMNLP2025-orange) ![](https://img.shields.io/badge/CODI-blue)
- **Scaling up Test-Time Compute with Latent Reasoning: A Recurrent Depth Approach**  
  *Jonas Geiping, Sean McLeish, Neel Jain, John Kirchenbauer, Siddharth Singh, Brian R. Bartoldson, Bhavya Kailkhura, Abhinav Bhatele, Tom Goldstein*. [[pdf](https://arxiv.org/pdf/2502.05171)], [[code](https://github.com/seal-rg/recurrent-pretraining)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange)
- **LLM Pretraining with Continuous Concepts**  
  *Jihoon Tack, Jack Lanchantin, Jane Yu, Andrew Cohen, Ilia Kulikov, Janice Lan, Shibo Hao, Yuandong Tian, Jason Weston, Xian Li*. [[pdf](https://arxiv.org/pdf/2502.08524)], [[code](https://github.com/facebookresearch/RAM/tree/main/projects/cocomix)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CoCoMix-blue) ![](https://img.shields.io/badge/Pretrain-green)
- **Scalable Language Models with Posterior Inference of Latent Thought Vectors**  
  *Deqian Kong, Minglu Zhao, Dehong Xu, Bo Pang, Shu Wang, Edouardo Honig, Zhangzhang Si, Chuan Li, Jianwen Xie, Sirui Xie, Ying Nian Wu*. [[pdf](https://arxiv.org/pdf/2502.01567)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/LTM-blue)
- **Enhancing Auto-regressive Chain-of-Thought through Loop-Aligned Reasoning**  
  *Qifan Yu, Zhenyu He, Sijie Li, Xun Zhou, Jun Zhang, Jingjing Xu, Di He*. [[pdf](https://arxiv.org/pdf/2502.08482)], [[code](https://github.com/qifanyu/RELAY)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/RELAY-blue)
- **Token Assorted: Mixing Latent and Text Tokens for Improved Language Model Reasoning**  
  *DiJia Su, Hanlin Zhu, Yingchen Xu, Jiantao Jiao, Yuandong Tian, Qinqing Zheng*. [[pdf](https://arxiv.org/pdf/2502.03275)], 2025.02. ![](https://img.shields.io/badge/ICML2025-orange)
- **Implicit Reasoning in Transformers is Reasoning through Shortcuts**  
  *Tianhe Lin, Jian Xie, Siyu Yuan, Deqing Yang*. [[pdf](https://arxiv.org/pdf/2503.07604)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Analysis-green)
- **Reasoning to Learn from Latent Thoughts**  
  *Yangjun Ruan, Neil Band, Chris J. Maddison, Tatsunori Hashimoto*. [[pdf](https://arxiv.org/pdf/2503.18866)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange)
- **Think Before Recommend: Unleashing the Latent Reasoning Power for Sequential Recommendation**  
  *Jiakai Tang, Sunhao Dai, Teng Shi, Jun Xu, Xu Chen, Wen Chen, Wu Jian, Yuning Jiang*. [[pdf](https://arxiv.org/pdf/2503.22675)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ReaRec-blue) ![](https://img.shields.io/badge/Sequential_Recommendation-green)
- **Efficient Pretraining Length Scaling**  
  *Bohong Wu, Shen Yan, Sijun Zhang, Jianqiao Lu, Yutao Zeng, Ya Wang, Xun Zhou*. [[pdf](https://arxiv.org/pdf/2504.14992)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/PHD--Transformer-blue)
- **Soft Thinking: Unlocking the Reasoning Potential of LLMs in Continuous Concept Space**  
  *Zhen Zhang, Xuehai He, Weixiang Yan, Ao Shen, Chenyang Zhao, Shuohang Wang, Yelong Shen, Xin Eric Wang*. [[pdf](https://arxiv.org/pdf/2505.15778)], [[code](https://github.com/eric-ai-lab/Soft-Thinking)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Soft--Thinking-blue)
- **Think Silently, Think Fast: Dynamic Latent Compression of LLM Reasoning Chains**  
  *Wenhui Tan, Jiaze Li, Jianzhong Ju, Zhenbo Luo, Jian Luan, Ruihua Song*. [[pdf](https://arxiv.org/pdf/2505.16552)], [[homepage](https://colar-latent-reasoning.github.io/)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CoLaR-blue)
- **Efficient Post-Training Refinement of Latent Reasoning in Large Language Models**  
  *Xinyuan Wang, Dongjie Wang, Wangyang Ying, Haoyue Bai, Nanxu Gong, Sixun Dong, Kunpeng Liu, Yanjie Fu*. [[pdf](https://arxiv.org/pdf/2506.08552)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **DART: Distilling Autoregressive Reasoning to Silent Thought**  
  *Nan Jiang, Ziming Wu, De-Chuan Zhan, Fuming Lai, Shaobing Lian*. [[pdf](https://arxiv.org/pdf/2506.11752)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **Parallel Continuous Chain-of-Thought with Jacobi Iteration**  
  *Haoyi Wu, Zhihao Teng, Kewei Tu*. [[pdf](https://arxiv.org/pdf/2506.18582)], [[code](https://github.com/whyNLP/PCCoT)], 2025.06. ![](https://img.shields.io/badge/EMNLP2025-orange) ![](https://img.shields.io/badge/PCCoT-blue)
- **Multimodal Chain of Continuous Thought for Latent-Space Reasoning in Vision-Language Models**  
  *Tan-Hanh Pham, Chris Ngo*. [[pdf](https://arxiv.org/pdf/2508.12587)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/MCOUT-blue)
- **LLMs are Single-threaded Reasoners: Demystifying the Working Mechanism of Soft Thinking**  
  *Chünhung Wu, Jinliang Lu, Zixuan Ren, Gangqiang Hu, Zhi Wu, Dai Dai, Hua Wu*. [[pdf](https://arxiv.org/pdf/2508.03440)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange)

### Long-to-Short Chain-of-Thought

- **Chain-of-Symbol Prompting Elicits Planning in Large Langauge Models**  
  *Hanxu Hu, Hongyuan Lu, Huajian Zhang, Yun-Ze Song, Wai Lam, Yue Zhang*. [[pdf](https://arxiv.org/pdf/2305.10276)], [[code](https://github.com/hanxuhu/chain-of-symbol-planning)], 2023.05. ![](https://img.shields.io/badge/Arxiv-orange)
- **The Benefits of a Concise Chain of Thought on Problem-Solving in Large Language Models**  
  *Matthew Renze, Erhan Guven*. [[pdf](https://arxiv.org/pdf/2401.05618)], [[code](https://github.com/matthewrenze/jhu-concise-cot)], 2024.01. ![](https://img.shields.io/badge/FLLM2024-orange) ![](https://img.shields.io/badge/CCoT-blue)
- **Efficiently Serving LLM Reasoning Programs with Certaindex**  
  *Yichao Fu, Junda Chen, Siqi Zhu, Zheyu Fu, Zhongdongming Dai, Aurick Qiao, Hao Zhang*. [[pdf](https://arxiv.org/pdf/2412.20993)], 2024.12. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Dynasor-blue)
- **C3oT: Generating Shorter Chain-of-Thought without Compromising Effectiveness**  
  *Yu Kang, Xianghui Sun, Liangyu Chen, Wei Zou*. [[pdf](https://arxiv.org/pdf/2412.11664)], 2024.12. ![](https://img.shields.io/badge/AAAI2025-orange) ![](https://img.shields.io/badge/C3oT-blue)
- **Token-Budget-Aware LLM Reasoning**  
  *Tingxu Han, Zhenting Wang, Chunrong Fang, Shiyu Zhao, Shiqing Ma, Zhenyu Chen*. [[pdf](https://arxiv.org/pdf/2412.18547)], [[code](https://github.com/GeniusHTX/TALE)], 2024.12. ![](https://img.shields.io/badge/ACL2025--findings-orange) ![](https://img.shields.io/badge/TALE-blue) ![](https://img.shields.io/badge/Prompt-green)
- **O1-Pruner: Length-Harmonizing Fine-Tuning for O1-Like Reasoning Pruning**  
  *Haotian Luo, Li Shen, Haiying He, Yibo Wang, Shiwei Liu, Wei Li, Naiqiang Tan, Xiaochun Cao, Dacheng Tao*. [[pdf](https://arxiv.org/pdf/2501.12570)], [[code](https://github.com/StarDewXXX/O1-Pruner)], 2025.01. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/O1--Pruner-blue)
- **Kimi k1.5: Scaling Reinforcement Learning with LLMs**  
  *Kimi Team*. [[pdf](https://arxiv.org/pdf/2501.12599)], 2025.01. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Kimi_k1.5-blue)
- **Training Language Models to Reason Efficiently**  
  *Daman Arora, Andrea Zanette*. [[pdf](https://arxiv.org/pdf/2502.04463)], [[code](https://github.com/Zanette-Labs/efficient-reasoning)], [[homepage](https://zanette-labs.github.io/efficient-reasoning/)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange)
- **Meta-Reasoner: Dynamic Guidance for Optimized Inference-time Reasoning in Large Language Models**  
  *Yuan Sui, Yufei He, Tri Cao, Simeng Han, Bryan Hooi*. [[pdf](https://arxiv.org/pdf/2502.19918)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Meta--Reasoner-blue)
- **CoT-Valve: Length-Compressible Chain-of-Thought Tuning**  
  *Xinyin Ma, Guangnian Wan, Runpeng Yu, Gongfan Fang, Xinchao Wang*. [[pdf](https://arxiv.org/pdf/2502.09601)], [[code](https://github.com/horseee/CoT-Valve)], 2025.02. ![](https://img.shields.io/badge/ACL2025-orange) ![](https://img.shields.io/badge/CoT--Valve-blue)
- **TokenSkip: Controllable Chain-of-Thought Compression in LLMs**  
  *Heming Xia, Yongqi Li, Chak Tou Leong, Wenjie Wang, Wenjie Li*. [[pdf](https://arxiv.org/pdf/2502.12067)], [[code](https://github.com/hemingkx/TokenSkip)], 2025.02. ![](https://img.shields.io/badge/EMNLP2025-orange) ![](https://img.shields.io/badge/TokenSkip-blue) ![](https://img.shields.io/badge/Controllable_Compression-green)
- **Self-Training Elicits Concise Reasoning in Large Language Models**  
  *Tergel Munkhbat, Namgyu Ho, Seo Hyun Kim, Yongjin Yang, Yujin Kim, Se-Young Yun*. [[pdf](https://arxiv.org/pdf/2502.20122)], [[code](https://github.com/TergelMunkhbat/concise-reasoning)], 2025.02. ![](https://img.shields.io/badge/ACL2025--findings-orange)
- **Chain of Draft: Thinking Faster by Writing Less**  
  *Silei Xu, Wenhao Xie, Lingxiao Zhao, Pengcheng He*. [[pdf](https://arxiv.org/pdf/2502.18600)], [[code](https://github.com/sileix/chain-of-draft)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CoD-blue) ![](https://img.shields.io/badge/Prompt-green)
- **L1: Controlling How Long A Reasoning Model Thinks With Reinforcement Learning**  
  *Pranjal Aggarwal, Sean Welleck*. [[pdf](https://www.arxiv.org/pdf/2503.04697)], [[code](https://github.com/cmu-l3/l1)], [[homepage](https://cmu-l3.github.io/l1/)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/L1-blue) ![](https://img.shields.io/badge/Length_Control-green)
- **DAST: Difficulty-Adaptive Slow-Thinking for Large Reasoning Models**  
  *Yi Shen, Jian Zhang, Jieyun Huang, Shuming Shi, Wenjing Zhang, Jiangze Yan, Ning Wang, Kai Wang, Shiguo Lian*. [[pdf](https://arxiv.org/pdf/2503.04472)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DAST-blue)
- **How Well do LLMs Compress Their Own Chain-of-Thought? A Token Complexity Approach**  
  *Ayeong Lee, Ethan Che, Tianyi Peng*. [[pdf](https://arxiv.org/pdf/2503.01141)], [[code](https://github.com/Compressed-CoT/compressed-cot)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Prompt-green)
- **Sketch-of-Thought: Efficient LLM Reasoning with Adaptive Cognitive-Inspired Sketching**  
  *Simon A. Aytes, Jinheon Baek, Sung Ju Hwang*. [[pdf](https://arxiv.org/pdf/2503.05179)], [[code](https://github.com/SimonAytes/SoT)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SoT-blue) ![](https://img.shields.io/badge/Prompt-green)
- **Adaptive Group Policy Optimization: Towards Stable Training and Token-Efficient Reasoning**  
  *Chen Li, Nazhou Liu, Kai Yang*. [[pdf](https://arxiv.org/pdf/2503.15952)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/AGPO-blue) ![](https://img.shields.io/badge/length--based_reward-green)
- **Unlocking Efficient Long-to-Short LLM Reasoning with Model Merging**  
  *Han Wu, Yuxuan Yao, Shuqi Liu, Zehua Liu, Xiaojin Fu, Xiongwei Han, Xing Li, Hui-Ling Zhen, Tao Zhong, Mingxuan Yuan*. [[pdf](https://arxiv.org/pdf/2503.20641)], [[code](https://github.com/hahahawu/Long-to-Short-via-Model-Merging)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Model_Merging-green)
- **Think When You Need: Self-Adaptive Chain-of-Thought Learning**  
  *Junjie Yang, Ke Lin, Xing Yu*. [[pdf](https://arxiv.org/pdf/2504.03234)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange)
- **ThinkPrune: Pruning Long Chain-of-Thought of LLMs via Reinforcement Learning**  
  *Bairu Hou, Yang Zhang, Jiabao Ji, Yujian Liu, Kaizhi Qian, Jacob Andreas, Shiyu Chang*. [[pdf](https://arxiv.org/pdf/2504.01296)], [[code](https://github.com/UCSB-NLP-Chang/ThinkPrune)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ThinkPrune-blue)
- **Reasoning Models Can Be Effective Without Thinking**  
  *Wenjie Ma, Jingxuan He, Charlie Snell, Tyler Griggs, Sewon Min, Matei Zaharia*. [[pdf](https://arxiv.org/pdf/2504.09858)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/NoThinking-blue) ![](https://img.shields.io/badge/Prompt-green)
- **ShorterBetter: Guiding Reasoning Models to Find Optimal Inference Length for Efficient Reasoning**  
  *Jingyang Yi, Jiazheng Wang*. [[pdf](https://arxiv.org/pdf/2504.21370)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ShorterBetter-blue) ![](https://img.shields.io/badge/Group--Relative_Length_Reward-green)
- **Dynamic Early Exit in Reasoning Models**  
  *Chenxu Yang, Qingyi Si, Yongjie Duan, Zheliang Zhu, Chenyu Zhu, Zheng Lin, Li Cao, Weiping Wang*. [[pdf](https://arxiv.org/pdf/2504.15895)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DEER-blue) ![](https://img.shields.io/badge/Early_Exit-green)
- **AdaR1: From Long-CoT to Hybrid-CoT via Bi-Level Adaptive Reasoning Optimization**  
  *Haotian Luo, Haiying He, Yibo Wang, Jinluan Yang, Rui Liu, Naiqiang Tan, Xiaochun Cao, Dacheng Tao, Li Shen*. [[pdf](https://arxiv.org/pdf/2504.21659)], [[code](https://github.com/StarDewXXX/AdaR1)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/AdaR1-blue)
- **Concise Reasoning via Reinforcement Learning**  
  *Mehdi Fatemi, Banafsheh Rafiee, Mingjie Tang, Kartik Talamadupula*. [[pdf](https://arxiv.org/pdf/2504.05185)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange)
- **Long-Short Chain-of-Thought Mixture Supervised Fine-Tuning Eliciting Efficient Reasoning in Large Language Models**  
  *Bin Yu, Hang Yuan, Yuliang Wei, Bailing Wang, Weizhen Qi, Kai Chen*. [[pdf](https://arxiv.org/pdf/2505.03469)], [[code](https://github.com/ZGCA-AI4Edu/LS-Mixture)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/LS--Mixture_SFT-blue)
- **ConCISE: Confidence-guided Compression in Step-by-step Efficient Reasoning**  
  *Ziqing Qiao, Yongheng Deng, Jiali Zeng, Dong Wang, Lai Wei, Fandong Meng, Jie Zhou, Ju Ren, Yaoxue Zhang*. [[pdf](https://arxiv.org/pdf/2505.04881)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ConCISE-blue)
- **Scalable Chain of Thoughts via Elastic Reasoning**  
  *Yuhui Xu, Hanze Dong, Lei Wang, Doyen Sahoo, Junnan Li, Caiming Xiong*. [[pdf](https://arxiv.org/pdf/2505.05315)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Elastic_Reasoning-blue) ![](https://img.shields.io/badge/Length_Control-green)
- **S-GRPO: Early Exit via Reinforcement Learning in Reasoning Models**  
  *Muzhi Dai, Chenxu Yang, Qingyi Si*. [[pdf](https://arxiv.org/pdf/2505.07686)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/S--GRPO-blue) ![](https://img.shields.io/badge/Early_Exit-green)
- **Making Small Language Models Efficient Reasoners: Intervention, Supervision, Reinforcement**  
  *Xuechen Zhang, Zijian Huang, Chenchun Ni, Ziyang Xiong, Jiasi Chen, Samet Oymak*. [[pdf](https://arxiv.org/pdf/2505.07961)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Length_Penalty-green)
- **Accelerating Chain-of-Thought Reasoning: When Goal-Gradient Importance Meets Dynamic Skipping**  
  *Ren Zhuang, Ben Wang, Shuifa Sun*. [[pdf](https://arxiv.org/pdf/2505.08392)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Token_Skipping-green)
- **SelfBudgeter: Adaptive Token Allocation for Efficient LLM Reasoning**  
  *Zheng Li, Qingxiu Dong, Jingyuan Ma, Di Zhang, Zhifang Sui*. [[pdf](https://arxiv.org/pdf/2505.11274)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SelfBudgeter-blue) ![](https://img.shields.io/badge/Adaptive_Token_Budget-green)
- **Not All Thoughts are Generated Equal: Efficient LLM Reasoning via Multi-Turn Reinforcement Learning**  
  *Yansong Ning, Wei Li, Jun Fang, Naiqiang Tan, Hao Liu*. [[pdf](https://arxiv.org/pdf/2505.11827)], [[code](https://github.com/yasNing/Long-otimes-Short/)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange)
- **Fractured Chain-of-Thought Reasoning**  
  *Baohao Liao, Hanze Dong, Yuhui Xu, Doyen Sahoo, Christof Monz, Junnan Li, Caiming Xiong*. [[pdf](https://arxiv.org/pdf/2505.12992)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange)
- **Efficient RL Training for Reasoning Models via Length-Aware Optimization**  
  *Danlong Yuan, Tian Xie, Shaohan Huang, Zhuocheng Gong, Huishuai Zhang, Chong Luo, Furu Wei, Dongyan Zhao*. [[pdf](https://arxiv.org/pdf/2505.12284)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange)
- **Can Pruning Improve Reasoning? Revisiting Long-CoT Compression with Capability in Mind for Better Reasoning**  
  *Shangziqi Zhao, Jiahao Yuan, Guisong Yang, Usman Naseem*. [[pdf](https://arxiv.org/pdf/2505.14582)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Prune--on--Logic-blue)
- **DRP: Distilled Reasoning Pruning with Skill-aware Step Decomposition for Efficient Large Reasoning Models**  
  *Yuxuan Jiang, Dawei Li, Frank Ferraro*. [[pdf](https://arxiv.org/pdf/2505.13975)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DRP-blue) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **SEAL: Steerable Reasoning Calibration of Large Language Models for Free**  
  *Runjin Chen, Zhenyu Zhang, Junyuan Hong, Souvik Kundu, Zhangyang Wang*. [[pdf](https://arxiv.org/pdf/2504.07986)], [[code](https://github.com/VITA-Group/SEAL)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SEAL-blue) ![](https://img.shields.io/badge/Steering-green)
- **FlashThink: An Early Exit Method For Efficient Reasoning**  
  *Guochao Jiang, Guofeng Quan, Zepeng Ding, Ziqin Luo, Dixuan Wang, Zheng Hu*. [[pdf](https://arxiv.org/pdf/2505.13949)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/FlashThink-blue) ![](https://img.shields.io/badge/Early_Exit-green)
- **Optimizing Anytime Reasoning via Budget Relative Policy Optimization**  
  *Penghui Qi, Zichen Liu, Tianyu Pang, Chao Du, Wee Sun Lee, Min Lin*. [[pdf](https://arxiv.org/pdf/2505.13438)], [[code](https://github.com/sail-sg/AnytimeReasoner)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/BRPO-blue) ![](https://img.shields.io/badge/Early_Exit-green)
- **VeriThinker: Learning to Verify Makes Reasoning Model Efficient**  
  *Zigeng Chen, Xinyin Ma, Gongfan Fang, Ruonan Yu, Xinchao Wang*. [[pdf](https://arxiv.org/pdf/2505.17941)], [[code](https://github.com/czg1225/VeriThinker)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/VeriThinker-blue) ![](https://img.shields.io/badge/CoTs_by_InstructLM-green)
- **Reasoning Path Compression: Compressing Generation Trajectories for Efficient LLM Reasoning**  
  *Jiwon Song, Dongwon Jo, Yulhwa Kim, Jae-Joon Kim*. [[pdf](https://arxiv.org/pdf/2505.13866)], [[code](https://github.com/jiwonsong-dev/ReasoningPathCompression)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/KV_Cache_Pruning-green)
- **ThinkLess: A Training-Free Inference-Efficient Method for Reducing Reasoning Redundancy**  
  *Gengyang Li, Yifeng Gao, Yuming Li, Yunfang Wu*. [[pdf](https://arxiv.org/pdf/2505.15684)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ThinkLess-blue) ![](https://img.shields.io/badge/Early_Exit-green)
- **Learn to Reason Efficiently with Adaptive Length-based Reward Shaping**  
  *Wei Liu, Ruochen Zhou, Yiyun Deng, Yuzhen Huang, Junteng Liu, Yuntian Deng, Yizhe Zhang, Junxian He*. [[pdf](https://arxiv.org/pdf/2505.15612)], [[code](https://github.com/hkust-nlp/Laser)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Laser-blue)
- **R1-Compress: Long Chain-of-Thought Compression via Chunk Compression and Search**  
  *Yibo Wang, Li Shen, Huanjin Yao, Tiansheng Huang, Rui Liu, Naiqiang Tan, Jiaxing Huang, Kai Zhang, Dacheng Tao*. [[pdf](https://arxiv.org/pdf/2505.16838)], [[code](https://github.com/w-yibo/R1-Compress)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/R1--Compress-blue) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **Incentivizing Dual Process Thinking for Efficient Large Language Model Reasoning**  
  *Xiaoxue Cheng, Junyi Li, Zhenduo Zhang, Xinyu Tang, Wayne Xin Zhao, Xinyu Kong, Zhiqiang Zhang*. [[pdf](https://arxiv.org/pdf/2505.16315)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ACPO-blue)
- **Plan and Budget: Effective and Efficient Test-Time Scaling on Large Language Model Reasoning**  
  *Junhong Lin, Xinyue Zeng, Jie Zhu, Song Wang, Julian Shun, Jun Wu, Dawei Zhou*. [[pdf](https://www.arxiv.org/pdf/2505.16122)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange)
- **ConciseRL: Conciseness-Guided Reinforcement Learning for Efficient Reasoning Models**  
  *Razvan-Gabriel Dumitru, Darius Peteleaza, Vikas Yadav, Liangming Pan*. [[pdf](https://www.arxiv.org/pdf/2505.17250)], [[code](https://github.com/RazvanDu/ConciseRL)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ConciseRL-blue)
- **TrimR: Verifier-based Training-Free Thinking Compression for Efficient Test-Time Scaling**  
  *Weizhe Lin, Xing Li, Zhiyuan Yang, Xiaojin Fu, Hui-Ling Zhen, Yaoyuan Wang, Xianzhi Yu, Wulong Liu, Xiaosong Li, Mingxuan Yuan*. [[pdf](https://arxiv.org/pdf/2505.17155)], 2025.05. ![](https://img.shields.io/badge/SCALR@COLM2025-orange) ![](https://img.shields.io/badge/TrimR-blue)  
- **Not All Tokens Are What You Need In Thinking**  
  *Hang Yuan, Bin Yu, Haotian Li, Shijun Yang, Christina Dan Wang, Zhou Yu, Xueyin Xu, Weizhen Qi, Kai Chen*. [[pdf](https://arxiv.org/pdf/2505.17827)], [[code](https://github.com/Faustrazor/Not-All-Thinking-Tokens)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Token_Skipping-green)
- **LIMOPro: Reasoning Refinement for Efficient and Effective Test-time Scaling**  
  *Yang Xiao, Jiashuo Wang, Ruifeng Yuan, Chunpu Xu, Kaishuai Xu, Wenjie Li, Pengfei Liu*. [[pdf](https://arxiv.org/pdf/2505.19187)], [[code](https://github.com/GAIR-NLP/LIMOPro)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/LIMOPro-blue) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **Walk Before You Run! Concise LLM Reasoning via Reinforcement Learning**  
  *Mingyang Song, Mao Zheng*. [[pdf](https://arxiv.org/pdf/2505.21178)], [[code](https://github.com/nick7nlp/ConciseR)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Length_Penalty-green)
- **CoThink: Token-Efficient Reasoning via Instruct Models Guiding Reasoning Models**  
  *Siqi Fan, Peng Han, Shuo Shang, Yequan Wang, Aixin Sun*. [[pdf](https://arxiv.org/pdf/2505.22017)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Outline_by_InstructLM-green)
- **Stable Reinforcement Learning for Efficient Reasoning**  
  *Muzhi Dai, Shixuan Liu, Qingyi Si*. [[pdf](https://arxiv.org/pdf/2505.18086)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Length_Penalty-green)
- **Don't Think Longer, Think Wisely: Optimizing Thinking Dynamics for Large Reasoning Models**  
  *Sohyun An, Ruochen Wang, Tianyi Zhou, Cho-Jui Hsieh*. [[pdf](https://arxiv.org/pdf/2505.21765)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DTO-blue) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **A\*-Thought: Efficient Reasoning via Bidirectional Compression for Low-Resource Settings**  
  *Xiaoang Xu, Shuo Wang, Xu Han, Zhenghao Liu, Huijia Wu, Peipei Li, Zhiyuan Liu, Maosong Sun, Zhaofeng He*. [[pdf](https://arxiv.org/pdf/2505.24550)], [[code](https://github.com/AI9Stars/AStar-Thought)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/A*--Thought-blue)
- **TL;DR: Too Long, Do Re-weighting for Efficient LLM Reasoning Compression**  
  *Zhong-Zhi Li, Xiao Liang, Zihao Tang, Lei Ji, Peijie Wang, Haotian Xu, Xing W, Haizhen Huang, Weiwei Deng, Ying Nian Wu, Yeyun Gong, Zhijiang Guo, Xiao Liu, Fei Yin, Cheng-Lin Liu*. [[pdf](https://arxiv.org/pdf/2506.02678)], [[code](https://github.com/zzli2022/TLDR)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/TL;DR-blue)
- **Answer Convergence as a Signal for Early Stopping in Reasoning**  
  *Xin Liu, Lu Wang*. [[pdf](https://arxiv.org/pdf/2506.02536)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Early_Exit-green)
- **How Far Are We from Optimal Reasoning Efficiency?**  
  *Jiaxuan Gao, Shu Yan, Qixin Tan, Lu Yang, Shusheng Xu, Wei Fu, Zhiyu Mei, Kaifeng Lyu, Yi Wu*. [[pdf](https://arxiv.org/pdf/2506.07104)], [[code](https://github.com/samjia2000/Optimal-Reasoning-Efficiency)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/REO--RL-blue)
- **Overclocking LLM Reasoning: Monitoring and Controlling Thinking Path Lengths in LLMs**  
  *Roy Eisenstadt, Itamar Zimerman, Lior Wolf*. [[pdf](https://arxiv.org/pdf/2506.07240)], [[homepage](https://royeisen.github.io/OverclockingLLMReasoning-paper/)], [[code](https://github.com/royeisen/reasoning_loading_bar)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **Bingo: Boosting Efficient Reasoning of LLMs via Dynamic and Significance-based Reinforcement Learning**  
  *Hanbing Liu, Lang Cao, Yuanyi Ren, Mengyu Zhou, Haoyu Dong, Xiaojun Ma, Shi Han, Dongmei Zhang*. [[pdf](https://arxiv.org/pdf/2506.08125)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Significance--aware_Length_Penalty-green)
- **Brevity is the soul of sustainability: Characterizing LLM response lengths**  
  *Soham Poddar, Paramita Koley, Janardan Misra, Sanjay Podder, Navveen Balani, Niloy Ganguly, Saptarshi Ghosh*. [[pdf](https://arxiv.org/pdf/2506.08686)], 2025.06. ![](https://img.shields.io/badge/ACL2025--findings-orange) ![](https://img.shields.io/badge/Prompting-green)
- **Wait, We Don't Need to "Wait"! Removing Thinking Tokens Improves Reasoning Efficiency**  
  *Chenlong Wang, Yuanning Feng, Dongping Chen, Zhaoyang Chu, Ranjay Krishna, Tianyi Zhou*. [[pdf](https://arxiv.org/pdf/2506.08343)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/NoWait-blue)
- **Causal Sufficiency and Necessity Improves Chain-of-Thought Reasoning**  
  *Xiangning Yu, Zhuohan Wang, Linyi Yang, Haoxuan Li, Anjie Liu, Xiao Xue, Jun Wang, Mengyue Yang*. [[pdf](https://arxiv.org/pdf/2506.09853)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/In--context_Learning&SFT-green)
- **PREMISE: Scalable and Strategic Prompt Optimization for Efficient Mathematical Reasoning in Large Models**  
  *Ye Yu, Yaoning Yu, Haohan Wang*. [[pdf](https://arxiv.org/pdf/2506.10716)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Prompting-green)
- **Just Enough Thinking: Efficient Reasoning with Adaptive Length Penalties Reinforcement Learning**  
  *Violet Xiang, Chase Blagden, Rafael Rafailov, Nathan Lile, Sang Truong, Chelsea Finn, Nick Haber*. [[pdf](https://arxiv.org/pdf/2506.05256)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ALP-blue) ![](https://img.shields.io/badge/Length_Control-green)
- **ReCUT: Balancing Reasoning Length and Accuracy in LLMs via Stepwise Trails and Preference Optimization**  
  *Zhensheng Jin, Xinze Li, Yifan Ji, Chunyi Peng, Zhenghao Liu, Qi Shi, Yukun Yan, Shuo Wang, Furong Peng, Ge Yu*. [[pdf](https://arxiv.org/pdf/2506.10822)], [[code](https://github.com/NEUIR/ReCUT)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **Fast on the Easy, Deep on the Hard: Efficient Reasoning via Powered Length Penalty**  
  *Zehui Ling, Deshu Chen, Hongwei Zhang, Yifeng Jiao, Xin Guo, Yuan Cheng*. [[pdf](https://arxiv.org/pdf/2506.10446)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **Efficient Reasoning Through Suppression of Self-Affirmation Reflections in Large Reasoning Models**  
  *Kaiyuan Liu, Chen Shen, Zhanwei Zhang, Junjie Liu, Xiaosong Yuan, Jieping ye*. [[pdf](https://arxiv.org/pdf/2506.12353)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **Steering LLM Thinking with Budget Guidance**  
  *Junyan Li, Wenshuo Zhao, Yang Zhang, Chuang Gan*. [[pdf](https://arxiv.org/pdf/2506.13752)], [[code](https://github.com/UMass-Embodied-AGI/BudgetGuidance)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **Optimizing Length Compression in Large Reasoning Models**  
  *Zhengxiang Cheng, Dongping Chen, Mingyang Fu, Tianyi Zhou*. [[pdf](https://arxiv.org/pdf/2506.14755)], [[code](https://github.com/zxiangx/LC-R1)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **Exploring and Exploiting the Inherent Efficiency within Large Reasoning Models for Self-Guided Efficiency Enhancement**  
  *Weixiang Zhao, Jiahe Guo, Yang Deng, Xingyu Sui, Yulin Hu, Yanyan Zhao, Wanxiang Che, Bing Qin, Tat-Seng Chua, Ting Liu*. [[pdf](https://arxiv.org/pdf/2506.15647)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Steering-green)
- **ConciseHint: Boosting Efficient Reasoning via Continuous Concise Hints during Generation**  
  *Siao Tang, Xinyin Ma, Gongfan Fang, Xinchao Wang*. [[pdf](https://arxiv.org/pdf/2506.18810)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **AdapThink: Adaptive Thinking Preferences for Reasoning Language Model**  
  *Xu Wan, Wei Wang, Wenyue Xu, Wotao Yin, Jie Song, Mingyang Sun*. [[pdf](https://arxiv.org/pdf/2506.18237)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **Less Data Less Tokens: Multilingual Unification Learning for Efficient Test-Time Reasoning in LLMs**  
  *Kang Chen, Mengdi Zhang, Yixin Cao*. [[pdf](https://arxiv.org/pdf/2506.18341)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Multilingual-green)
- **AALC: Large Language Model Efficient Reasoning via Adaptive Accuracy-Length Control**  
  *Ruosen Li, Ziming Luo, Quan Zhang, Ruochen Li, Ben Zhou, Ali Payani, Xinya Du*. [[pdf](https://arxiv.org/pdf/2506.20160)], [[code](https://github.com/du-nlp-lab/LengthReward)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **Do Thinking Tokens Help or Trap? Towards More Efficient Large Reasoning Model**  
  *Bowen Ding, Yuhan Chen, Futing Wang, Lingfeng Ming, Tao Lin*. [[pdf](https://arxiv.org/pdf/2506.23840)], [[code](https://github.com/Danield21/Dual-Policy-Preference-Optimization)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange)
- **EfficientXLang: Towards Improving Token Efficiency Through Cross-Lingual Reasoning**  
  *Sanchit Ahuja, Praneetha Vaddamanu, Barun Patra*. [[pdf](https://arxiv.org/pdf/2507.00246)], [[code](https://github.com/microsoft/EfficientXLang)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Multilingual-green)
- **Activation Steering for Chain-of-Thought Compression**  
  *Seyedarmin Azizi, Erfan Baghaei Potraghloo, Massoud Pedram*. [[pdf](https://arxiv.org/pdf/2507.04742)], [[code](https://github.com/ArminAzizi98/ASC)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Steering-green)
- **SmartThinker: Learning to Compress and Preserve Reasoning by Step-Level Length Control**  
  *Xingyang He, Xiao Ling, Jie Liu*. [[pdf](https://arxiv.org/pdf/2507.04348)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange)
- **Controlling Thinking Speed in Reasoning Models**  
  *Zhengkai Lin, Zhihang Fu, Ze Chen, Chao Chen, Liang Xie, Wenxiao Wang, Deng Cai, Zheng Wang, Jieping Ye*. [[pdf](https://arxiv.org/pdf/2507.03704v1)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Steering-green)
- **Verbosity-Aware Rationale Reduction: Sentence-Level Rationale Reduction for Efficient and Effective Reasoning**  
  *Joonwon Jang, Jaehee Kim, Wonbin Kweon, Seonghyeon Lee, Hwanjo Yu*. [[pdf](https://aclanthology.org/2025.findings-acl.1068.pdf)], 2025.07. ![](https://img.shields.io/badge/ACL2025--findings-orange)
- **Test-time Prompt Intervention**  
  *Chenxu Yang, Qingyi Si, Muzhi Dai, Dingyu Yao, Mingyu Zheng, Minghui Chen, Zheng Lin, Weiping Wang*. [[pdf](https://arxiv.org/pdf/2508.02511)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/PI-blue)
- **Reconsidering Overthinking: Penalizing Internal and External Redundancy in CoT Reasoning**  
  *Jialiang Hong, Taihang Zhen, Kai Chen, Jiaheng Liu, Wenpeng Zhu, Jing Huo, Yang Gao, Depeng Wang, Haitao Wan, Xi Yang, Boyan Wang, Fanyu Meng*. [[pdf](https://www.arxiv.org/pdf/2508.02178)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange)
- **Compressing Chain-of-Thought in LLMs via Step Entropy**  
  *Zeju Li, Jianyuan Zhong, Ziyang Zheng, Xiangyu Wen, Zhijian Xu, Yingying Cheng, Fan Zhang, Qiang Xu*. [[pdf](https://arxiv.org/pdf/2508.03346)], [[code](https://github.com/staymylove/COT_Compresstion_via_Step_entropy)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **Efficient Reasoning for Large Reasoning Language Models via Certainty-Guided Reflection Suppression**  
  *Jiameng Huang, Baijiong Lin, Guhao Feng, Jierun Chen, Di He, Lu Hou*. [[pdf](https://arxiv.org/pdf/2508.05337)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CGRS-blue)
- **Train Long, Think Short: Curriculum Learning for Efficient Reasoning**  
  *Hasan Abed Al Kader Hammoud, Kumail Alhamoud, Abed Hammoud, Elie Bou-Zeid, Marzyeh Ghassemi, Bernard Ghanem*. [[pdf](https://arxiv.org/pdf/2508.08940)], [[code](https://github.com/hammoudhasan/curriculum_grpo)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange)
- **Sample More to Think Less: Group Filtered Policy Optimization for Concise Reasoning**  
  *Vaishnavi Shrivastava, Ahmed Awadallah, Vidhisha Balachandran, Shivam Garg, Harkirat Behl, Dimitris Papailiopoulos*. [[pdf](https://arxiv.org/pdf/2508.09726)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/GFPO-blue)
- **SABER: Switchable and Balanced Training for Efficient LLM Reasoning**  
  *Kai Zhao, Yanjun Zhao, Jiaming Song, Shien He, Lusheng Zhang, Qiang Zhang, Tianjiao Li*. [[pdf](https://arxiv.org/pdf/2508.10026)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SABER-blue)
- **Promoting Efficient Reasoning with Verifiable Stepwise Reward**  
  *Chuhuai Yue, Chengqi Dong, Yinan Gao, Hang He, Jiajun Chai, Guojun Yin, Wei Lin*. [[pdf](https://arxiv.org/pdf/2508.10293)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/VSRM-blue)
- **Aware First, Think Less: Dynamic Boundary Self-Awareness Drives Extreme Reasoning Efficiency in Large Language Models**  
  *Qiguang Chen, Dengyun Peng, Jinhao Liu, HuiKang Su, Jiannan Guan, Libo Qin, Wanxiang Che*. [[pdf](https://arxiv.org/pdf/2508.11582)], [[code](https://github.com/sfasfaffa/DR_SAF)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DR.SAF-blue)
- **Stop Spinning Wheels: Mitigating LLM Overthinking via Mining Patterns for Early Reasoning Exit**  
  *Zihao Wei, Liang Pang, Jiahao Liu, Jingcheng Deng, Shicheng Xu, Zenghao Duan, Jingang Wang, Fei Sun, Xunliang Cai, Huawei Shen, Xueqi Cheng*. [[pdf](https://arxiv.org/pdf/2508.17627)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Early_Exit-green)
- **BudgetThinker: Empowering Budget-aware LLM Reasoning with Control Tokens**  
  *Hao Wen, Xinrui Wu, Yi Sun, Feifei Zhang, Liye Chen, Jie Wang, Yunxin Liu, Ya-Qin Zhang, Yuanchun Li*. [[pdf](https://arxiv.org/pdf/2508.17196)], [[code](https://github.com/MobileLLM/BudgetThinker)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/BudgetThinker-blue)
- **DRQA: Dynamic Reasoning Quota Allocation for Controlling Overthinking in Reasoning Large Language Models**  
  *Kaiwen Yan, Xuanqing Shi, Hongcheng Guo, Wenxuan Wang, Zhuosheng Zhang, Chengwei Qin*. [[pdf](https://arxiv.org/pdf/2508.17803)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DRQA-blue)
- **CAC-CoT: Connector-Aware Compact Chain-of-Thought for Efficient Reasoning Data Synthesis Across Dual-System Cognitive Tasks**  
  *Sunguk Choi, Yonghoon Kwon, Heondeuk Lee*. [[pdf](https://arxiv.org/pdf/2508.18743)], 2025.08. ![](https://img.shields.io/badge/EMNLP2025--findings-orange) ![](https://img.shields.io/badge/CAC--CoT-blue)
- **ThinkDial: An Open Recipe for Controlling Reasoning Effort in Large Language Models**  
  *Qianyu He, Siyu Yuan, Xuefeng Li, Mingxuan Wang, Jiangjie Chen*. [[pdf](https://arxiv.org/pdf/2508.18773)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ThinkDial-blue) ![](https://img.shields.io/badge/gpt--oss--style-green)

### Adaptive Thinking

- **Learning When to Think: Shaping Adaptive Reasoning in R1-Style Models via Multi-Stage RL**  
  *Songjun Tu, Jiahao Lin, Qichao Zhang, Xiangyu Tian, Linjing Li, Xiangyuan Lan, Dongbin Zhao*. [[pdf](https://arxiv.org/pdf/2505.10832)], [[code](https://github.com/TU2021/AutoThink)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange)
- **AdaptThink: Reasoning Models Can Learn When to Think**  
  *Jiajie Zhang, Nianyi Lin, Lei Hou, Ling Feng, Juanzi Li*. [[pdf](https://arxiv.org/pdf/2505.13417)], [[code](https://github.com/THU-KEG/AdaptThink)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/AdaptThink-blue)
- **Thinkless: LLM Learns When to Think**  
  *Gongfan Fang, Xinyin Ma, Xinchao Wang*. [[pdf](https://arxiv.org/pdf/2505.13379)], [[code](https://github.com/VainF/Thinkless)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Thinkless-blue)
- **Think Only When You Need with Large Hybrid-Reasoning Models**  
  *Lingjie Jiang, Xun Wu, Shaohan Huang, Qingxiu Dong, Zewen Chi, Li Dong, Xingxing Zhang, Tengchao Lv, Lei Cui, Furu Wei*. [[pdf](https://arxiv.org/pdf/2505.14631)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange)
- **ThinkSwitcher: When to Think Hard, When to Think Fast**  
  *Guosheng Liang, Longguang Zhong, Ziyi Yang, Xiaojun Quan*. [[pdf](https://arxiv.org/pdf/2505.14183)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ThinkSwitcher-blue)
- **Prolonged Reasoning Is Not All You Need: Certainty-Based Adaptive Routing for Efficient LLM/MLLM Reasoning**  
  *Jinghui Lu, Haiyang Yu, Siliang Xu, Shiwei Ran, Guozhi Tang, Siqi Wang, Bin Shan, Teng Fu, Hao Feng, Jingqun Tang, Han Wang, Can Huang*. [[pdf](https://arxiv.org/pdf/2505.15154)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/CAR-blue)
- **When to Continue Thinking: Adaptive Thinking Mode Switching for Efficient Reasoning**  
  *Xiaoyun Zhang, Jingqing Ruan, Xing Ma, Yawen Zhu, Haodong Zhao, Hao Li, Jiansong Chen, Ke Zeng, Xunliang Cai*. [[pdf](https://arxiv.org/pdf/2505.15400)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ASRR-blue)
- **AdaCoT: Pareto-Optimal Adaptive Chain-of-Thought Triggering via Reinforcement Learning**  
  *Chenwei Lou, Zewei Sun, Xinnian Liang, Meng Qu, Wei Shen, Wenqi Wang, Yuntao Li, Qingping Yang, Shuangzhi Wu*. [[pdf](https://arxiv.org/pdf/2505.11896)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/AdaCoT-blue)
- **AutoL2S: Auto Long-Short Reasoning for Efficient Large Language Models**  
  *Feng Luo, Yu-Neng Chuang, Guanchu Wang, Hoang Anh Duy Le, Shaochen Zhong, Hongyi Liu, Jiayi Yuan, Yang Sui, Vladimir Braverman, Vipin Chaudhary, Xia Hu*. [[pdf](https://arxiv.org/pdf/2505.22662)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/AutoL2S-blue)
- **AlphaOne: Reasoning Models Thinking Slow and Fast at Test Time**  
  *Junyu Zhang, Runpei Dong, Han Wang, Xuying Ning, Haoran Geng, Peihao Li, Xialin He, Yutong Bai, Jitendra Malik, Saurabh Gupta, Huan Zhang*. [[pdf](https://arxiv.org/pdf/2505.24863)], [[homepage](https://alphaone-project.github.io/)], [[code](https://github.com/ASTRAL-Group/AlphaOne)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/AlphaOne-blue)
- **OThink-R1: Intrinsic Fast/Slow Thinking Mode Switching for Over-Reasoning Mitigation**  
  *Shengjia Zhang, Junjie Wu, Jiawei Chen, Changwang Zhang, Xingyu Lou, Wangchunshu Zhou, Sheng Zhou, Can Wang, Jun Wang*. [[pdf](https://arxiv.org/pdf/2506.02397)], [[code](https://github.com/AgenticIR-Lab/OThink-R1)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/OThink--R1-blue)
- **Long or short CoT? Investigating Instance-level Switch of Large Reasoning Models**  
  *Ruiqi Zhang, Changyi Xiao, Yixin Cao*. [[pdf](https://arxiv.org/pdf/2506.04182)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SwitchCoT-blue)
- **Token Signature: Predicting Chain-of-Thought Gains with Token Decoding Feature in Large Language Models**  
  *Peijie Liu, Fengli Xu, Yong Li*. [[pdf](https://arxiv.org/pdf/2506.06008)], [[code](https://github.com/tsinghua-fib-lab/Token_Signature)], 2025.06. ![](https://img.shields.io/badge/ICML2025-orange)
- **SynapseRoute: An Auto-Route Switching Framework on Dual-State Large Language Model**  
  *Wencheng Zhang, Shiqin Qiao, Lingjie Luo, Yinfeng Li, Chuanyang Zheng, Qian Xu, Meng Li, Yong Gui, Yijun He, Jianing Qiu, Jindong Hong, Jiankai Sun*. [[pdf](https://arxiv.org/pdf/2507.02822)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SynapseRoute-blue)
- **Large Reasoning Models Know How to Think Efficiently**  
  *Zeyu XING, Xing Li, Huiling Zhen, Xianzhi Yu, Mingxuan Yuan, Sinno Jialin Pan*. [[pdf](https://openreview.net/forum?id=pLKDeGm2t1)], 2025.07. ![](https://img.shields.io/badge/ESFoMoIII@ICML2025-orange) ![](https://img.shields.io/badge/SelfThink-blue)
- **Think in Blocks: Adaptive Reasoning from Direct Response to Deep Reasoning**  
  *Yekun Zhu, Guang Chen, Chengjun Mao*. [[pdf](https://arxiv.org/pdf/2508.15507)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange)

### Reasoning Shortcuts

- **Not All Neuro-Symbolic Concepts Are Created Equal: Analysis and Mitigation of Reasoning Shortcuts**  
  *Emanuele Marconato, Stefano Teso, Antonio Vergari, Andrea Passerini*. [[pdf](https://arxiv.org/pdf/2305.19951)], 2023.05. ![](https://img.shields.io/badge/NIPS2023-orange)
- **Break the Chain: Large Language Models Can be Shortcut Reasoners**  
  *Mengru Ding, Hanmeng Liu, Zhizhang Fu, Jian Song, Wenbo Xie, Yue Zhang*. [[pdf](https://arxiv.org/pdf/2406.06580)], 2024.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Break_the_Chain-blue)
- **Can Language Models Learn to Skip Steps?**  
  *Tengxiao Liu, Qipeng Guo, Xiangkun Hu, Cheng Jiayang, Yue Zhang, Xipeng Qiu, Zheng Zhang*. [[pdf](https://arxiv.org/pdf/2411.01855)], [[code](https://github.com/tengxiaoliu/LM_skip)], 2024.11. ![](https://img.shields.io/badge/NIPS2024-orange) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **TokenSkip: Controllable Chain-of-Thought Compression in LLMs**  
  *Heming Xia, Yongqi Li, Chak Tou Leong, Wenjie Wang, Wenjie Li*. [[pdf](https://arxiv.org/pdf/2502.12067)], [[code](https://github.com/hemingkx/TokenSkip)], 2025.02. ![](https://img.shields.io/badge/EMNLP2025-orange) ![](https://img.shields.io/badge/TokenSkip-blue) ![](https://img.shields.io/badge/Token_Shortcut-green)
- **Stepwise Perplexity-Guided Refinement for Efficient Chain-of-Thought Reasoning in Large Language Models**  
  *Yingqian Cui, Pengfei He, Jingying Zeng, Hui Liu, Xianfeng Tang, Zhenwei Dai, Yan Han, Chen Luo, Jing Huang, Zhen Li, Suhang Wang, Yue Xing, Jiliang Tang, Qi He*. [[pdf](https://arxiv.org/pdf/2502.13260)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **Accelerating Chain-of-Thought Reasoning: When Goal-Gradient Importance Meets Dynamic Skipping**  
  *Ren Zhuang, Ben Wang, Shuifa Sun*. [[pdf](https://arxiv.org/pdf/2505.08392)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Token_Shortcut-green)
- **DRP: Distilled Reasoning Pruning with Skill-aware Step Decomposition for Efficient Large Reasoning Models**  
  *Yuxuan Jiang, Dawei Li, Frank Ferraro*. [[pdf](https://arxiv.org/pdf/2505.13975)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DRP-blue) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **R1-Compress: Long Chain-of-Thought Compression via Chunk Compression and Search**  
  *Yibo Wang, Li Shen, Huanjin Yao, Tiansheng Huang, Rui Liu, Naiqiang Tan, Jiaxing Huang, Kai Zhang, Dacheng Tao*. [[pdf](https://arxiv.org/pdf/2505.16838)], [[code](https://github.com/w-yibo/R1-Compress)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/R1--Compress-blue) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **Not All Tokens Are What You Need In Thinking**  
  *Hang Yuan, Bin Yu, Haotian Li, Shijun Yang, Christina Dan Wang, Zhou Yu, Xueyin Xu, Weizhen Qi, Kai Chen*. [[pdf](https://arxiv.org/pdf/2505.17827)], [[code](https://github.com/Faustrazor/Not-All-Thinking-Tokens)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Token_Shortcut-green)
- **LIMOPro: Reasoning Refinement for Efficient and Effective Test-time Scaling**  
  *Yang Xiao, Jiashuo Wang, Ruifeng Yuan, Chunpu Xu, Kaishuai Xu, Wenjie Li, Pengfei Liu*. [[pdf](https://arxiv.org/pdf/2505.19187)], [[code](https://github.com/GAIR-NLP/LIMOPro)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/LIMOPro-blue) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **Don't Think Longer, Think Wisely: Optimizing Thinking Dynamics for Large Reasoning Models**  
  *Sohyun An, Ruochen Wang, Tianyi Zhou, Cho-Jui Hsieh*. [[pdf](https://arxiv.org/pdf/2505.21765)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DTO-blue) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **Compressing Chain-of-Thought in LLMs via Step Entropy**  
  *Zeju Li, Jianyuan Zhong, Ziyang Zheng, Xiangyu Wen, Zhijian Xu, Yingying Cheng, Fan Zhang, Qiang Xu*. [[pdf](https://arxiv.org/pdf/2508.03346)], [[code](https://github.com/staymylove/COT_Compresstion_via_Step_entropy)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Step_Shortcut-green)
- **Pruning the Unsurprising: Efficient Code Reasoning via First-Token Surprisal**  
  *Wenhao Zeng, Yaoning Wang, Chao Hu, Yuling Shi, Chengcheng Wan, Hongyu Zhang, Xiaodong Gu*. [[pdf](https://arxiv.org/pdf/2508.05988)], [[code](https://github.com/Zengwh02/ASAP)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Step_Shortcut-green)

### Reasoning Step Decomposition

- **Markov Chain of Thought for Efficient Mathematical Reasoning**  
  *Wen Yang, Minpeng Liao, Kai Fan*. [[pdf](https://arxiv.org/pdf/2410.17635)], [[code](https://github.com/james-yw/Markov-Chain-of-Thought)], 2024.10. ![](https://img.shields.io/badge/NAACL2025-orange) ![](https://img.shields.io/badge/MCoT-blue) ![](https://img.shields.io/badge/Intermediate_CoT_Summarization-green)
- **Atom of Thoughts for Markov LLM Test-Time Scaling**  
  *Fengwei Teng, Zhaoyang Yu, Quan Shi, Jiayi Zhang, Chenglin Wu, Yuyu Luo*. [[pdf](https://arxiv.org/pdf/2502.12018)], [[code](https://github.com/qixucen/atom)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/AoT-blue)
- **DISC: Dynamic Decomposition Improves LLM Inference Scaling**  
  *Jonathan Light, Wei Cheng, Wu Yue, Masafumi Oyamada, Mengdi Wang, Santiago Paternain, Haifeng Chen*. [[pdf](https://arxiv.org/pdf/2502.16706)], 2025.02. ![](https://img.shields.io/badge/ICLR2025_SSI--FM_workshop-orange) ![](https://img.shields.io/badge/DISC-blue)
- **Can Atomic Step Decomposition Enhance the Self-structured Reasoning of Multimodal Large Models?**  
  *Kun Xiang, Zhili Liu, Zihao Jiang, Yunshuang Nie, Kaixin Cai, Yiyang Yin, Runhui Huang, Haoxiang Fan, Hanhui Li, Weiran Huang, Yihan Zeng, Yu-Jie Yuan, Jianhua Han, Lanqing Hong, Hang Xu, Xiaodan Liang*. [[pdf](https://arxiv.org/pdf/2503.06252)], [[code](https://github.com/Quinn777/AtomThink)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SCoT-blue) ![](https://img.shields.io/badge/Multimodal-green)
- **From Chaos to Order: The Atomic Reasoner Framework for Fine-grained Reasoning in Large Language Models**  
  *Jinyi Liu, Yan Zheng, Rong Cheng, Qiyu Wu, Wei Guo, Fei Ni, Hebin Liang, Yifu Yuan, Hangyu Mao, Fuzheng Zhang, Jianye Hao*. [[pdf](https://arxiv.org/pdf/2503.15944)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/AR-blue)

### Small Reasoning Models & CoT Distillation

- **Teaching Small Language Models to Reason**  
  *Lucie Charlotte Magister, Jonathan Mallinson, Jakub Adamek, Eric Malmi, Aliaksei Severyn*. [[pdf](https://aclanthology.org/2023.acl-short.151.pdf)], 2022.12. ![](https://img.shields.io/badge/ACL2023--short-orange)
- **Mixed Distillation Helps Smaller Language Model Better Reasoning**  
  *Chenglin Li, Qianglong Chen, Liangyue Li, Caiyu Wang, Yicheng Li, Zulong Chen, Yin Zhang*. [[pdf](https://arxiv.org/pdf/2312.10730)], 2023.12. ![](https://img.shields.io/badge/EMNLP2024--findings-orange)
- **Small Language Models Need Strong Verifiers to Self-Correct Reasoning**  
  *Yunxiang Zhang, Muhammad Khalifa, Lajanugen Logeswaran, Jaekyeom Kim, Moontae Lee, Honglak Lee, Lu Wang*. [[pdf](https://arxiv.org/pdf/2404.17140)], [[code](https://github.com/yunx-z/SCORE)], 2024.04. ![](https://img.shields.io/badge/ACL2024--findings-orange)
- **Distilling Reasoning Ability from Large Language Models with Adaptive Thinking**  
  *Xiaoshu Chen, Sihang Zhou, Ke Liang, Xinwang Liu*. [[pdf](https://arxiv.org/pdf/2404.09170)], 2024.04. ![](https://img.shields.io/badge/Arxiv-orange)
- **Teaching Small Language Models Reasoning through Counterfactual Distillation**  
  *Tao Feng, Yicheng Li, Li Chenglin, Hao Chen, Fei Yu, Yin Zhang*. [[pdf](https://aclanthology.org/2024.emnlp-main.333.pdf)], 2024.11. ![](https://img.shields.io/badge/EMNLP2024-orange)
- **Improving Mathematical Reasoning Capabilities of Small Language Models via Feedback-Driven Distillation**  
  *Xunyu Zhu, Jian Li, Can Ma, Weiping Wang*. [[pdf](https://arxiv.org/pdf/2411.14698)], 2024.11. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/FDD-blue)
- **Thinking Slow, Fast: Scaling Inference Compute with Distilled Reasoners**  
  *Daniele Paliotta, Junxiong Wang, Matteo Pagliardini, Kevin Y. Li, Aviv Bick, J. Zico Kolter, Albert Gu, François Fleuret, Tri Dao*. [[pdf](https://arxiv.org/pdf/2502.20339)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange)
- **Unveiling the Key Factors for Distilling Chain-of-Thought Reasoning**  
  *Xinghao Chen, Zhijing Sun, Wenjin Guo, Miaoran Zhang, Yanjun Chen, Yirong Sun, Hui Su, Yijie Pan, Dietrich Klakow, Wenjie Li, Xiaoyu Shen*. [[pdf](https://arxiv.org/pdf/2502.18001)], [[code](https://github.com/EIT-NLP/Distilling-CoT-Reasoning)], 2025.02. ![](https://img.shields.io/badge/ACL2025--findings-orange)
- **Can 1B LLM Surpass 405B LLM? Rethinking Compute-Optimal Test-Time Scaling**  
  *Runze Liu, Junqi Gao, Jian Zhao, Kaiyan Zhang, Xiu Li, Biqing Qi, Wanli Ouyang, Bowen Zhou*. [[pdf](https://arxiv.org/pdf/2502.06703)], [[code](https://github.com/RyanLiu112/compute-optimal-tts)], [[homepage](https://ryanliu112.github.io/compute-optimal-tts/)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/TTS-blue)
- **Small Models Struggle to Learn from Strong Reasoners**  
  *Yuetai Li, Xiang Yue, Zhangchen Xu, Fengqing Jiang, Luyao Niu, Bill Yuchen Lin, Bhaskar Ramasubramanian, Radha Poovendran*. [[pdf](https://arxiv.org/pdf/2502.12143)], [[code](https://github.com/Small-Model-Gap/Small-Model-Learnability-Gap)], [[homepage](https://small-model-gap.github.io/)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange)
- **Towards Reasoning Ability of Small Language Models**  
  *Gaurav Srivastava, Shuxiang Cao, Xuan Wang*. [[pdf](https://arxiv.org/pdf/2502.11569)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange)
- **Deconstructing Long Chain-of-Thought: A Structured Reasoning Optimization Framework for Long CoT Distillation**  
  *Yijia Luo, Yulin Song, Xingyao Zhang, Jiaheng Liu, Weixun Wang, GengRu Chen, Wenbo Su, Bo Zheng*. [[pdf](https://arxiv.org/pdf/2503.16385)], [[code](https://github.com/elena-luo/SODE)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DLCoT-blue)
- **SimpleRL-Zoo: Investigating and Taming Zero Reinforcement Learning for Open Base Models in the Wild**  
  *Weihao Zeng, Yuzhen Huang, Qian Liu, Wei Liu, Keqing He, Zejun Ma, Junxian He*. [[pdf](https://arxiv.org/pdf/2503.18892)], [[code](https://github.com/hkust-nlp/simpleRL-reason)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SimpleRL--Zoo-blue) ![](https://img.shields.io/badge/Zero_RL_Training-green)
- **Reinforcement Learning for Reasoning in Small LLMs: What Works and What Doesn't**  
  *Quy-Anh Dang, Chris Ngo*. [[pdf](https://arxiv.org/pdf/2503.16219)], [[code](https://github.com/knoveleng/open-rs)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange)
- **TwT: Thinking without Tokens by Habitual Reasoning Distillation with Multi-Teachers' Guidance**  
  *Jingxian Xu, Mengyu Zhou, Weichang Liu, Hanbing Liu, Shi Han, Dongmei Zhang*. [[pdf](https://arxiv.org/pdf/2503.24198)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/TwT-blue)
- **When Reasoning Meets Compression: Benchmarking Compressed Large Reasoning Models on Complex Reasoning Tasks**  
  *Nan Zhang, Yusen Zhang, Prasenjit Mitra, Rui Zhang*. [[pdf](https://arxiv.org/pdf/2504.02010)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange)
- **A Short Survey on Small Reasoning Models: Training, Inference, Applications and Research Directions**  
  *Chengyu Wang, Taolin Zhang, Richang Hong, Jun Huang*. [[pdf](https://arxiv.org/pdf/2504.09100)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Survey-green)
- **Tina: Tiny Reasoning Models via LoRA**  
  *Shangshang Wang, Julian Asilis, Ömer Faruk Akgül, Enes Burak Bilgin, Ollie Liu, Willie Neiswanger*. [[pdf](https://arxiv.org/pdf/2504.15777)], [[code](https://github.com/shangshang-wang/Tina)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Tina-blue)
- **A Technical Study into Small Reasoning Language Models**  
  *Xialie Zhuang, Peixian Ma, Zhikai Jia, Zheng Cao, Shiwei Liu*. [[pdf](https://arxiv.org/pdf/2506.13404)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)

### Small & Large Reasoning Model Collaboration

- **Hawkeye: Efficient Reasoning with Model Collaboration**  
  *Jianshu She, Zhuohao Li, Zhemin Huang, Qi Li, Peiran Xu, Haonan Li, Qirong Ho*. [[pdf](https://arxiv.org/pdf/2504.00424)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Hawkeye-blue)
- **Guiding Reasoning in Small Language Models with LLM Assistance**  
  *Yujin Kim, Euiin Yi, Minu Kim, Se-Young Yun, Taehyeon Kim*. [[pdf](https://arxiv.org/pdf/2504.09923)], [[code](https://github.com/kimyuji/ScaffoldedReasoning)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SMART-blue)
- **Thought Manipulation: External Thought Can Be Efficient for Large Reasoning Models**  
  *Yule Liu, Jingyi Zheng, Zhen Sun, Zifan Peng, Wenhan Dong, Zeyang Sha, Shiwen Cui, Weiqiang Wang, Xinlei He*. [[pdf](https://arxiv.org/pdf/2504.13626)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Thought_Manipulation-blue) ![](https://img.shields.io/badge/CoTs_from_SRMs-green)
- **SplitReason: Learning To Offload Reasoning**  
  *Yash Akhauri, Anthony Fei, Chi-Chih Chang, Ahmed F. AbouElhamayed, Yueying Li, Mohamed S. Abdelfattah*. [[pdf](https://arxiv.org/pdf/2504.16379)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SplitReason-blue) ![](https://img.shields.io/badge/offloading_challenging_CoT_parts_to_LRMs-green)
- **ProxyThinker: Test-Time Guidance through Small Visual Reasoners**  
  *Zilin Xiao, Jaywon Koo, Siru Ouyang, Jefferson Hernandez, Yu Meng, Vicente Ordonez*. [[pdf](https://arxiv.org/pdf/2505.24872)], [[code](https://github.com/MrZilinXiao/ProxyThinker)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ProxyThinker-blue) ![](https://img.shields.io/badge/CoTs_from_Multimodal_SRMs-green)
- **What makes Reasoning Models Different? Follow the Reasoning Leader for Efficient Decoding**  
  *Ming Li, Zhengyuan Yang, Xiyao Wang, Dianqi Li, Kevin Lin, Tianyi Zhou, Lijuan Wang*. [[pdf](https://arxiv.org/pdf/2506.06998)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/FoReaL--Decoding-blue)
- **Collaborative LLM Inference via Planning for Efficient Reasoning**  
  *Byeongchan Lee, Jonghoon Lee, Dongyoung Kim, Jaehyung Kim, Jinwoo Shin*. [[pdf](https://arxiv.org/pdf/2506.11578)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **R-Stitch: Dynamic Trajectory Stitching for Efficient Reasoning**  
  *Zhuokun Chen, Zeren Chen, Jiahao He, Mingkui Tan, Jianfei Cai, Bohan Zhuang*. [[pdf](https://arxiv.org/pdf/2507.17307)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange)

### Speculative Decoding for CoT Efficiency

- **Reward-Guided Speculative Decoding for Efficient LLM Reasoning**  
  *Baohao Liao, Yuhui Xu, Hanze Dong, Junnan Li, Christof Monz, Silvio Savarese, Doyen Sahoo, Caiming Xiong*. [[pdf](https://arxiv.org/pdf/2501.19324)], [[code](https://github.com/BaohaoLiao/RSD)], 2025.01. ![](https://img.shields.io/badge/ICML2025-orange) ![](https://img.shields.io/badge/RSD-blue)
- **SpecReason: Fast and Accurate Inference-Time Compute via Speculative Reasoning**  
  *Rui Pan, Yinwei Dai, Zhihao Zhang, Gabriele Oliaro, Zhihao Jia, Ravi Netravali*. [[pdf](https://arxiv.org/pdf/2504.07891)], [[code](https://github.com/ruipeterpan/specreason)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SpecReason-blue)
- **Speculative Thinking: Enhancing Small-Model Reasoning with Large Model Guidance at Inference Time**  
  *Wang Yang, Xiang Yue, Vipin Chaudhary, Xiaotian Han*. [[pdf](https://arxiv.org/pdf/2504.12329)], [[code](https://github.com/uservan/speculative_thinking)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Speculative_Thinking-blue)
- **Efficient Reasoning for LLMs through Speculative Chain-of-Thought**  
  *Jikai Wang, Juntao Li, Lijun Wu, Min Zhang*. [[pdf](https://arxiv.org/pdf/2504.19095)], [[code](https://github.com/Jikai0Wang/Speculative_CoT)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SCoT-blue)
- **Accelerating Large Language Model Reasoning via Speculative Search**  
  *Zhihai Wang, Jie Wang, Jilai Pan, Xilin Xia, Huiling Zhen, Mingxuan Yuan, Jianye Hao, Feng Wu*. [[pdf](https://arxiv.org/pdf/2505.02865)], 2025.05. ![](https://img.shields.io/badge/ICML2025-orange) ![](https://img.shields.io/badge/SCoT-blue)
- **Accelerated Test-Time Scaling with Model-Free Speculative Sampling**  
  *Woomin Song, Saket Dingliwal, Sai Muralidhar Jayanthi, Bhavana Ganesh, Jinwoo Shin, Aram Galstyan, Sravan Babu Bodapati*. [[pdf](https://arxiv.org/abs/2506.04708)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/STAND-blue)

### Sparse Attention & KV Cache

- **R-KV: Redundancy-aware KV Cache Compression for Training-Free Reasoning Models Acceleration**  
  *Zefan Cai, Wen Xiao, Hanshi Sun, Cheng Luo, Yikai Zhang, Ke Wan, Yucheng Li, Yeyang Zhou, Li-Wen Chang, Jiuxiang Gu, Zhen Dong, Anima Anandkumar, Abedelkadir Asi, Junjie Hu*. [[pdf](https://arxiv.org/pdf/2505.24133)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/R--KV-blue)
- **SeerAttention-R: Sparse Attention Adaptation for Long Reasoning**  
  *Yizhao Gao, Shuming Guo, Shijie Cao, Yuqing Xia, Yu Cheng, Lei Wang, Lingxiao Ma, Yutao Sun, Tianzhu Ye, Li Dong, Hayden Kwok-Hay So, Yu Hua, Ting Cao, Fan Yang, Mao Yang*. [[pdf](https://arxiv.org/pdf/2506.08889)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SeerAttention--R-blue)
- **Think Clearly: Improving Reasoning via Redundant Token Pruning**  
  *Daewon Choi, Jimin Lee, Jihoon Tack, Woomin Song, Saket Dingliwal, Sai Muralidhar Jayanthi, Bhavana Ganesh, Jinwoo Shin, Aram Galstyan, Sravan Babu Bodapati*. [[pdf](https://arxiv.org/pdf/2507.08806)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange)
- **Less Is More: Training-Free Sparse Attention with Global Locality for Efficient Reasoning**  
  *Lijie Yang, Zhihao Zhang, Arti Jain, Shijie Cao, Baihong Yuan, Yiwei Chen, Zhihao Jia, Ravi Netravali*. [[pdf](https://arxiv.org/pdf/2508.07101)], [[code](https://github.com/DerrickYLJ/LessIsMore)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange)

### Optimal Test-Time Scaling

- **Scaling LLM Test-Time Compute Optimally Can be More Effective than Scaling Parameters for Reasoning**  
  *Charlie Snell, Jaehoon Lee, Kelvin Xu, Aviral Kumar*. [[pdf](https://openreview.net/pdf?id=4FWAwZtd2n)], 2024.08. ![](https://img.shields.io/badge/ICLR2025-orange)
- **Inference Scaling Laws: An Empirical Analysis of Compute-Optimal Inference for Problem-Solving with Language Models**  
  *Yangzhen Wu, Zhiqing Sun, Shanda Li, Sean Welleck, Yiming Yang*. [[pdf](https://arxiv.org/pdf/2408.00724)], [[code](https://github.com/thu-wyz/inference_scaling)], [[homepage](https://thu-wyz.github.io/inference-scaling/)], 2024.08. ![](https://img.shields.io/badge/Arxiv-orange)
- **Scaling Test-Time Compute Without Verification or RL is Suboptimal**  
  *Amrith Setlur, Nived Rajaraman, Sergey Levine, Aviral Kumar*. [[pdf](https://arxiv.org/pdf/2502.12118)], 2025.02. ![](https://img.shields.io/badge/ICML2025-orange)
- **Revisiting the Test-Time Scaling of o1-like Models: Do they Truly Possess Test-Time Scaling Capabilities?**  
  *Zhiyuan Zeng, Qinyuan Cheng, Zhangyue Yin, Yunhua Zhou, Xipeng Qiu*. [[pdf](https://arxiv.org/pdf/2502.12215)], [[code](https://github.com/ZhiYuanZeng/test-time-scaling-eval)], 2025.02. ![](https://img.shields.io/badge/ACL2025-orange) ![](https://img.shields.io/badge/Over--thinking-green)
- **Towards Thinking-Optimal Scaling of Test-Time Compute for LLM Reasoning**  
  *Wenkai Yang, Shuming Ma, Yankai Lin, Furu Wei*. [[pdf](https://arxiv.org/pdf/2502.18080)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Over--thinking-green)
- **Optimizing Test-Time Compute via Meta Reinforcement Fine-Tuning**  
  *Yuxiao Qu, Matthew Y. R. Yang, Amrith Setlur, Lewis Tunstall, Edward Emanuel Beeching, Ruslan Salakhutdinov, Aviral Kumar*. [[pdf](https://arxiv.org/pdf/2503.07572)], [[code](https://github.com/CMU-AIRe/MRT)], [[homepage](https://cohenqu.github.io/mrt.github.io/)], 2025.03. ![](https://img.shields.io/badge/ICML2025-orange) ![](https://img.shields.io/badge/MRT-blue)
- **Is Best-of-N the Best of Them? Coverage, Scaling, and Optimality in Inference-Time Alignment**  
  *Audrey Huang, Adam Block, Qinghua Liu, Nan Jiang, Dylan J. Foster, Akshay Krishnamurthy*. [[pdf](https://arxiv.org/pdf/2503.21878)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/InferenceTimePessimism-blue)
- **What, How, Where, and How Well? A Survey on Test-Time Scaling in Large Language Models**  
  *Qiyuan Zhang, Fuyuan Lyu, Zexu Sun, Lei Wang, Weixu Zhang, Zhihan Guo, Yufei Wang, Irwin King, Xue Liu, Chen Ma*. [[pdf](https://arxiv.org/pdf/2503.24235)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Survey-green)
- **When To Solve, When To Verify: Compute-Optimal Problem Solving and Generative Verification for LLM Reasoning**  
  *Nishad Singhi, Hritik Bansal, Arian Hosseini, Aditya Grover, Kai-Wei Chang, Marcus Rohrbach, Anna Rohrbach*. [[pdf](https://arxiv.org/pdf/2504.01005)], [[code](https://github.com/nishadsinghi/sc-genrm-scaling)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange)
- **Z1: Efficient Test-time Scaling with Code**  
  *Zhaojian Yu, Yinghao Wu, Yilun Zhao, Arman Cohan, Xiao-Ping Zhang*. [[pdf](https://arxiv.org/pdf/2504.00810)], [[code](https://github.com/efficientscaling/Z1)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Z1-blue)
- **Think Deep, Think Fast: Investigating Efficiency of Verifier-free Inference-time-scaling Methods**  
  *Junlin Wang, Shang Zhu, Jon Saad-Falcon, Ben Athiwaratkun, Qingyang Wu, Jue Wang, Shuaiwen Leon Song, Ce Zhang, Bhuwan Dhingra, James Zou*. [[pdf](https://arxiv.org/pdf/2504.14047)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange)
- **Putting the Value Back in RL: Better Test-Time Scaling by Unifying LLM Reasoners With Verifiers**  
  *Kusha Sareen, Morgane M Moss, Alessandro Sordoni, Rishabh Agarwal, Arian Hosseini*. [[pdf](https://arxiv.org/pdf/2505.04842)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange)
- **Guided by Gut: Efficient Test-Time Scaling with Reinforced Intrinsic Confidence**  
  *Amirhosein Ghasemabadi, Keith G. Mills, Baochun Li, Di Niu*. [[pdf](https://arxiv.org/abs/2505.20325)], [[code](https://github.com/Amirhosein-gh98/Guided-by-Gut)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange)
- **Value-Guided Search for Efficient Chain-of-Thought Reasoning**  
  *Kaiwen Wang, Jin Peng Zhou, Jonathan Chang, Zhaolin Gao, Nathan Kallus, Kianté Brantley, Wen Sun*. [[pdf](https://arxiv.org/pdf/2505.17373)], [[code](https://github.com/kaiwenw/value-guided-search)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange)
- **Don't Overthink it. Preferring Shorter Thinking Chains for Improved LLM Reasoning**  
  *Michael Hassid, Gabriel Synnaeve, Yossi Adi, Roy Schwartz*. [[pdf](https://arxiv.org/pdf/2505.17813)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Shortest_N-green)
- **First Finish Search: Efficient Test-Time Scaling in Large Language Models**  
  *Aradhye Agarwal, Ayan Sengupta, Tanmoy Chakraborty*. [[pdf](https://arxiv.org/pdf/2505.18149)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Shortest_N-green)
- **LLM-First Search: Self-Guided Exploration of the Solution Space**  
  *Nathan Herr, Tim Rocktäschel, Roberta Raileanu*. [[pdf](https://arxiv.org/pdf/2506.05213)], [[code](https://github.com/NathanHerr/LLM-First-Search)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/LFS-blue)
- **Every Rollout Counts: Optimal Resource Allocation for Efficient Test-Time Scaling**  
  *Xinglin Wang, Yiwei Li, Shaoxiong Feng, Peiwen Yuan, Yueqi Zhang, Jiayi Shi, Chuyi Tan, Boyuan Pan, Yao Hu, Kan Li*. [[pdf](https://arxiv.org/pdf/2506.15707)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DORA-blue)
- **𝚂𝙿𝙴𝙲𝚂: Faster Test-Time Scaling through Speculative Drafts**  
  *Mert Cemri, Nived Rajaraman, Rishabh Tiwari, Xiaoxuan Liu, Kurt Keutzer, Ion Stoica, Kannan Ramchandran, Ahmad Beirami, Ziteng Sun*. [[pdf](https://arxiv.org/pdf/2506.15733)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SPECS-blue)
- **BEST-Route: Adaptive LLM Routing with Test-Time Optimal Compute**  
  *Dujian Ding, Ankur Mallick, Shaokun Zhang, Chi Wang, Daniel Madrigal, Mirian Del Carmen Hipolito Garcia, Menglin Xia, Laks V.S. Lakshmanan, Qingyun Wu, Victor Rühle*. [[pdf](https://arxiv.org/pdf/2506.22716)], 2025.07. ![](https://img.shields.io/badge/ICML2025-orange) ![](https://img.shields.io/badge/BEST--Route-blue)
- **Deep Think with Confidence**  
  *Yichao Fu, Xuewei Wang, Yuandong Tian, Jiawei Zhao*. [[pdf](https://arxiv.org/pdf/2508.15260)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DeepConf-blue)
### Efficient Sampling

- **Fast Best-of-N Decoding via Speculative Rejection**  
  *Hanshi Sun, Momin Haider, Ruiqi Zhang, Huitao Yang, Jiahao Qiu, Ming Yin, Mengdi Wang, Peter Bartlett, Andrea Zanette*. [[pdf](https://openreview.net/pdf?id=348hfcprUs)], [[code](https://github.com/Zanette-Labs/SpeculativeRejection)], 2024.10. ![](https://img.shields.io/badge/NIPS2024-orange) ![](https://img.shields.io/badge/Speculative_Rejection-blue) ![](https://img.shields.io/badge/Best--of--N-green)
- **Non-myopic Generation of Language Models for Reasoning and Planning**  
  *Chang Ma, Haiteng Zhao, Junlei Zhang, Junxian He, Lingpeng Kong*. [[pdf](https://openreview.net/pdf?id=OoNazl6T7D)], [[code](https://github.com/chang-github-00/LLM-Predictive-Decoding)], 2024.10. ![](https://img.shields.io/badge/ICLR2025-orange) ![](https://img.shields.io/badge/Predictive--Decoding-blue)
- **FastMCTS: A Simple Sampling Strategy for Data Synthesis**  
  *Peiji Li, Kai Lv, Yunfan Shao, Yichuan Ma, Linyang Li, Xiaoqing Zheng, Xipeng Qiu, Qipeng Guo*. [[pdf](https://www.arxiv.org/pdf/2502.11476)], 2025.02. ![](https://img.shields.io/badge/ACL2025-orange) ![](https://img.shields.io/badge/FastMCTS-blue)
- **Dynamic Parallel Tree Search for Efficient LLM Reasoning**  
  *Yifu Ding, Wentao Jiang, Shunyu Liu, Yongcheng Jing, Jinyang Guo, Yingjie Wang, Jing Zhang, Zengmao Wang, Ziwei Liu, Bo Du, Xianglong Liu, Dacheng Tao*. [[pdf](https://arxiv.org/pdf/2502.16235)], 2025.02. ![](https://img.shields.io/badge/ACL2025-orange) ![](https://img.shields.io/badge/DPTS-blue)
- **Don't Get Lost in the Trees: Streamlining LLM Reasoning by Overcoming Tree Search Exploration Pitfalls**  
  *Ante Wang, Linfeng Song, Ye Tian, Dian Yu, Haitao Mi, Xiangyu Duan, Zhaopeng Tu, Jinsong Su, Dong Yu*. [[pdf](https://arxiv.org/pdf/2502.11183)], 2025.02. ![](https://img.shields.io/badge/ACL2025-orange) ![](https://img.shields.io/badge/FETCH-blue)
- **Sampling-Efficient Test-Time Scaling: Self-Estimating the Best-of-N Sampling in Early Decoding**  
  *Yiming Wang, Pei Zhang, Siyuan Huang, Baosong Yang, Zhuosheng Zhang, Fei Huang, Rui Wang*. [[pdf](https://arxiv.org/pdf/2503.01422)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ST--BoN-blue) ![](https://img.shields.io/badge/Best--of--N-green)
- **Language Models can Self-Improve at State-Value Estimation for Better Search**  
  *Ethan Mendes, Alan Ritter*. [[pdf](https://arxiv.org/pdf/2503.02878)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Self--taught_Lookahead-blue)
- **ϕ-Decoding: Adaptive Foresight Sampling for Balanced Inference-Time Exploration and Exploitation**  
  *Fangzhi Xu, Hang Yan, Chang Ma, Haiteng Zhao, Jun Liu, Qika Lin, Zhiyong Wu*. [[pdf](https://arxiv.org/pdf/2503.13288)], [[code](https://github.com/xufangzhi/phi-Decoding)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/ϕ--Decoding-blue)
- **Lost at the Beginning of Reasoning**  
  *Baohao Liao, Xinyi Chen, Sara Rajaee, Yuhui Xu, Christian Herold, Anders Søgaard, Maarten de Rijke, Christof Monz*. [[pdf](https://arxiv.org/pdf/2506.22058)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)
- **Adaptive Termination for Multi-round Parallel Reasoning: An Universal Semantic Entropy-Guided Framework**  
  *Zenan Xu, Zexuan Qiu, Guanhua Huang, Kun Li, Siheng Li, Chenchen Zhang, Kejiao Li, Qi Yi, Yuhao Jiang, Bo Zhou, Fengzong Lian, Zhanhui Kang*. [[pdf](https://arxiv.org/pdf/2507.06829)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange)
- **MUR: Momentum Uncertainty guided Reasoning for Large Language Models**  
  *Hang Yan, Fangzhi Xu, Rongman Xu, Yifei Li, Jian Zhang, Haoran Luo, Xiaobao Wu, Luu Anh Tuan, Haiteng Zhao, Qika Lin, Jun Liu*. [[pdf](https://arxiv.org/pdf/2507.14958)], [[code](https://github.com/yayayacc/MUR)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange)

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
  *Amir Taubenfeld, Tom Sheffer, Eran Ofek, Amir Feder, Ariel Goldstein, Zorik Gekhman, Gal Yona*. [[pdf](https://arxiv.org/pdf/2502.06233)], 2025.02. ![](https://img.shields.io/badge/ACL2025--findings-orange) ![](https://img.shields.io/badge/CISC-blue)
- **Bridging Internal Probability and Self-Consistency for Effective and Efficient LLM Reasoning**  
  *Zhi Zhou, Tan Yuhao, Zenan Li, Yuan Yao, Lan-Zhe Guo, Xiaoxing Ma, Yu-Feng Li*. [[pdf](https://arxiv.org/pdf/2502.00511)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/RPC-blue)

### Long-Context Reasoning Efficiency

- **OmniKV: Dynamic Context Selection for Efficient Long-Context LLMs**  
  *Jitai Hao, Yuke Zhu, Tian Wang, Jun Yu, Xin Xin, Bo Zheng, Zhaochun Ren, Sheng Guo*. [[pdf](https://openreview.net/pdf?id=ulCAPXYXfa)], 2024.10. ![](https://img.shields.io/badge/ICLR2025-orange) ![](https://img.shields.io/badge/OmniKV-blue)
- **InftyThink: Breaking the Length Limits of Long-Context Reasoning in Large Language Models**  
  *Yuchen Yan, Yongliang Shen, Yang Liu, Jin Jiang, Mengdi Zhang, Jian Shao, Yueting Zhuang*. [[pdf](https://arxiv.org/pdf/2503.06692)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/InftyThink-blue) ![](https://img.shields.io/badge/Intermediate_CoT_Summarization-green)

### Multimodal Reasoning Efficiency

- **PixelThink: Towards Efficient Chain-of-Pixel Reasoning**  
  *Song Wang, Gongfan Fang, Lingdong Kong, Xiangtai Li, Jianyun Xu, Sheng Yang, Qiang Li, Jianke Zhu, Xinchao Wang*. [[pdf](https://arxiv.org/pdf/2505.23727)], [[code](https://github.com/songw-zju/PixelThink)], [[homepage](https://pixelthink.github.io/)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/PixelThink-blue)
- **R-4B: Incentivizing General-Purpose Auto-Thinking Capability in MLLMs via Bi-Mode Annealing and Reinforce Learning**  
  *Jie Jiang, Qi Yang, Bolin Ni, Shiming Xiang, Han Hu, Houwen Peng*. [[pdf](https://arxiv.org/pdf/2508.21113)], [[code](https://github.com/yannqi/R-4B)], [[huggingface](https://huggingface.co/YannQi/R-4B)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/R--4B-blue)

### Other Work

- **Skeleton-of-Thought: Large Language Models Can Do Parallel Decoding**  
  *Xuefei Ning, Zinan Lin, Zixuan Zhou, Zifu Wang, Huazhong Yang, Yu Wang*. [[pdf](https://openreview.net/pdf?id=mqVgBbNCm9)], [[code](https://github.com/imagination-research/sot)], [[homepage](https://sites.google.com/view/sot-llm)], 2023.06. ![](https://img.shields.io/badge/ICLR2024-orange) ![](https://img.shields.io/badge/SoT-blue) ![](https://img.shields.io/badge/Parallel_CoT-green)
- **Adaptive Skeleton Graph Decoding**  
  *Shuowei Jin, Yongji Wu, Haizhong Zheng, Qingzhao Zhang, Matthew Lentz, Z. Morley Mao, Atul Prakash, Feng Qian, Danyang Zhuo*. [[pdf](https://arxiv.org/pdf/2402.12280)], 2024.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Parallel_CoT-green)
- **PENCIL: Long Thoughts with Short Memory**  
  *PENCIL: Long Thoughts with Short Memory*. [[pdf](https://arxiv.org/pdf/2503.14337)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/PENCIL-blue) ![](https://img.shields.io/badge/Intermediate_CoT_Reduction-green)
- **Accelerate Parallelizable Reasoning via Parallel Decoding within One Sequence**  
  *Yijiong Yu*. [[pdf](https://arxiv.org/pdf/2503.20533)], [[code](https://github.com/yuyijiong/parallel-decoding-in-one-sequence)], 2024.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Parallel_Decoding-green)
- **Fast-Slow-Thinking: Complex Task Solving with Large Language Models**  
  *Yiliu Sun, Yanfang Zhang, Zicheng Zhao, Sheng Wan, Dacheng Tao, Chen Gong*. [[pdf](https://arxiv.org/pdf/2504.08690)], 2024.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/System2-green)
- **Learning Adaptive Parallel Reasoning with Language Models**  
  *Jiayi Pan, Xiuyu Li, Long Lian, Charlie Snell, Yifei Zhou, Adam Yala, Trevor Darrell, Kurt Keutzer, Alane Suhr*. [[pdf](https://arxiv.org/pdf/2504.15466)], [[code](https://github.com/Parallel-Reasoning/APR)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/APR-blue) ![](https://img.shields.io/badge/Parallel_Computation-green)
- **M1: Towards Scalable Test-Time Compute with Mamba Reasoning Models**  
  *Junxiong Wang, Wen-Ding Li, Daniele Paliotta, Daniel Ritter, Alexander M. Rush, Tri Dao*. [[pdf](https://arxiv.org/pdf/2504.10449)], [[code](https://github.com/jxiw/M1)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/M1-blue) ![](https://img.shields.io/badge/Mamba-green)
- **Group Think: Multiple Concurrent Reasoning Agents Collaborating at Token Level Granularity**  
  *Chan-Jan Hsu, Davide Buffelli, Jamie McGowan, Feng-Ting Liao, Yi-Chang Chen, Sattar Vakili, Da-shan Shiu*. [[pdf](https://arxiv.org/pdf/2505.11107)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Parallel_CoT-green)
- **Thinker: Learning to Think Fast and Slow**  
  *Stephen Chung, Wenyu Du, Jie Fu*. [[pdf](https://arxiv.org/pdf/2505.21097)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/System2-green)
- **Multiverse: Your Language Models Secretly Decide How to Parallelize and Merge Generation**  
  *Xinyu Yang, Yuwei An, Hongyi Liu, Tianqi Chen, Beidi Chen*. [[pdf](https://arxiv.org/pdf/2506.09991)], [[homepage](https://multiverse4fm.github.io/)], [[code](https://github.com/Infini-AI-Lab/Multiverse)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Parallel_CoT-green)
- **SPRINT: Enabling Interleaved Planning and Parallelized Execution in Reasoning Models**  
  *Emil Biju, Shayan Talaei, Zhemin Huang, Mohammadreza Pourreza, Azalia Mirhoseini, Amin Saberi*. [[pdf](https://arxiv.org/pdf/2506.05745)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/SPRINT-blue) ![](https://img.shields.io/badge/Parallel_Execution-green)
- **Route-and-Reason: Scaling Large Language Model Reasoning with Reinforced Model Router**  
  *Chenyang Shao, Xinyang Liu, Yutang Lin, Fengli Xu, Yong Li*. [[pdf](https://arxiv.org/pdf/2506.05901)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/R2--Reasoner-blue) ![](https://img.shields.io/badge/Model_Router-green)
- **Accelerating LLM Reasoning via Early Rejection with Partial Reward Modeling**  
  *Seyyed Saeid Cheshmi, Azal Ahmad Khan, Xinran Wang, Zirui Liu, Ali Anwar*. [[pdf](https://arxiv.org/pdf/2508.01969)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange)

### Benchmarks

- **DNA Bench: When Silence is Smarter -- Benchmarking Over-Reasoning in Reasoning LLMs**  
  *Masoud Hashemi, Oluwanifemi Bamgbose, Sathwik Tejaswi Madhusudhan, Jishnu Sethumadhavan Nair, Aman Tiwari, Vikas Yadav*. [[pdf](https://arxiv.org/pdf/2503.15793)], 2024.12. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/DNA_Bench-blue)
- **S1-Bench: A Simple Benchmark for Evaluating System 1 Thinking Capability of Large Reasoning Models**  
  *Wenyuan Zhang, Shuaiyi Nie, Xinghua Zhang, Zefeng Zhang, Tingwen Liu*. [[pdf](https://arxiv.org/pdf/2504.10368)], [[code](https://github.com/WYRipple/S1_Bench)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/S1--Bench-blue)
- **THOUGHTTERMINATOR: Benchmarking, Calibrating, and Mitigating Overthinking in Reasoning Models**  
  *Xiao Pu, Michael Saxon, Wenyue Hua, William Yang Wang*. [[pdf](https://arxiv.org/pdf/2504.13367)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/THOUGHTTERMINATOR-blue)
- **THINK-Bench: Evaluating Thinking Efficiency and Chain-of-Thought Quality of Large Reasoning Models**  
  *Zhiyuan Li, Yi Chang, Yuan Wu*. [[pdf](https://arxiv.org/pdf/2505.22113)], [[homepage](https://think-bench.github.io/)], [[code](https://github.com/ZhiyuanLi218/Think-Bench)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/THINK--Bench-blue)
- **LLMThinkBench: Towards Basic Math Reasoning and Overthinking in Large Language Models**  
  *Gaurav Srivastava, Aafiya Hussain, Sriram Srinivasan, Xuan Wang*. [[pdf](https://arxiv.org/pdf/2507.04023)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/LLMThinkBench-blue)
- **OptimalThinkingBench: Evaluating Over and Underthinking in LLMs**  
  *Pranjal Aggarwal, Seungone Kim, Jack Lanchantin, Sean Welleck, Jason Weston, Ilia Kulikov, Swarnadeep Saha*. [[pdf](https://arxiv.org/pdf/2508.13141)], [[code](https://github.com/facebookresearch/RAM/tree/main/projects/otb)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/OptimalThinkingBench-blue)

### Analysis

- **The Impact of Reasoning Step Length on Large Language Models**  
  *Mingyu Jin, Qinkai Yu, Dong Shu, Haiyan Zhao, Wenyue Hua, Yanda Meng, Yongfeng Zhang, Mengnan Du*. [[pdf](https://aclanthology.org/2024.findings-acl.108.pdf)], [[code](https://github.com/MingyuJ666/The-Impact-of-Reasoning-Step-Length-on-Large-Language-Models)], 2024.01. ![](https://img.shields.io/badge/AC2024--findings-orange) ![](https://img.shields.io/badge/Reasoning_Step_Length-green)
- **Concise Thoughts: Impact of Output Length on LLM Reasoning and Cost**  
  *Sania Nayab, Giulio Rossolini, Marco Simoni, Andrea Saracino, Giorgio Buttazzo, Nicolamaria Manes, Fabrizio Giacomelli*. [[pdf](https://arxiv.org/pdf/2407.19825)], 2024.07. ![](https://img.shields.io/badge/Arxiv-orange)
- **Unlocking the Capabilities of Thought: A Reasoning Boundary Framework to Quantify and Optimize Chain-of-Thought**  
  *Qiguang Chen, Libo Qin, Jiaqi Wang, Jinxuan Zhou, Wanxiang Che*. [[pdf](https://arxiv.org/pdf/2410.05695)], [[code](https://github.com/LightChen233/reasoning-boundary)], 2024.10. ![](https://img.shields.io/badge/NIPS2024-orange) ![](https://img.shields.io/badge/Reasoning_Boundary-green)
- **Do NOT Think That Much for 2+3=? On the Overthinking of o1-Like LLMs**  
  *Xingyu Chen, Jiahao Xu, Tian Liang, Zhiwei He, Jianhui Pang, Dian Yu, Linfeng Song, Qiuzhi Liu, Mengfei Zhou, Zhuosheng Zhang, Rui Wang, Zhaopeng Tu, Haitao Mi, Dong Yu*. [[pdf](https://arxiv.org/pdf/2412.21187)], 2024.12. ![](https://img.shields.io/badge/ICML2025-orange) ![](https://img.shields.io/badge/Over--thinking-green)
- **When More is Less: Understanding Chain-of-Thought Length in LLMs**  
  *Yuyang Wu, Yifei Wang, Tianqi Du, Stefanie Jegelka, Yisen Wang*. [[pdf](https://arxiv.org/pdf/2502.07266)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Optimal_CoT_Length-green)
- **The Danger of Overthinking: Examining the Reasoning-Action Dilemma in Agentic Tasks**  
  *Alejandro Cuadron, Dacheng Li, Wenjie Ma, Xingyao Wang, Yichuan Wang, Siyuan Zhuang, Shu Liu, Luis Gaspar Schroeder, Tian Xia, Huanzhi Mao, Nicholas Thumiger, Aditya Desai, Ion Stoica, Ana Klimovic, Graham Neubig, Joseph E. Gonzalez*. [[pdf](https://arxiv.org/pdf/2502.08235)], [[code](https://github.com/AlexCuadron/ThinkingAgent)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Over--thinking-green)
- **Thoughts Are All Over the Place: On the Underthinking of o1-Like LLMs**  
  *Yue Wang, Qiuzhi Liu, Jiahao Xu, Tian Liang, Xingyu Chen, Zhiwei He, Linfeng Song, Dian Yu, Juntao Li, Zhuosheng Zhang, Rui Wang, Zhaopeng Tu, Haitao Mi, Dong Yu*. [[pdf](https://arxiv.org/pdf/2501.18585)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Under--thinking-green)
- **The Relationship Between Reasoning and Performance in Large Language Models -- o3 (mini) Thinks Harder, Not Longer**  
  *Marthe Ballon, Andres Algaba, Vincent Ginis*. [[pdf](https://arxiv.org/pdf/2502.15631)], 2025.02. ![](https://img.shields.io/badge/Arxiv-orange)
- **Long Is More Important Than Difficult for Training Reasoning Models**  
  *Si Shen, Fei Huang, Zhixiao Zhao, Chang Liu, Tiansheng Zheng, Danhao Zhu*. [[pdf](https://arxiv.org/pdf/2503.18069)], [[code](https://huggingface.co/ZTss/LONG1k-32B)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange)
- **Innate Reasoning is Not Enough: In-Context Learning Enhances Reasoning Large Language Models with Less Overthinking**  
  *Yuyao Ge, Shenghua Liu, Yiwei Wang, Lingrui Mei, Lizhe Chen, Baolong Bi, Xueqi Cheng*. [[pdf](https://arxiv.org/pdf/2503.19602)], 2025.03. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Over--thinking-green)
- **Reasoning Models Know When They're Right: Probing Hidden States for Self-Verification**  
  *Anqi Zhang, Yulin Chen, Jane Pan, Chen Zhao, Aurojit Panda, Jinyang Li, He He*. [[pdf](https://arxiv.org/pdf/2504.05419)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Over--thinking-green)
- **Missing Premise exacerbates Overthinking: Are Reasoning Models losing Critical Thinking Skill?**  
  *Chenrui Fan, Ming Li, Lichao Sun, Tianyi Zhou*. [[pdf](https://arxiv.org/pdf/2504.06514)], [[code](https://github.com/tianyi-lab/MiP-Overthinking)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Over--thinking-green)
- **Time's Up! An Empirical Study of LLM Reasoning Ability Under Output Length Constraint**  
  *Yi Sun, Han Wang, Jiaqiang Li, Jiacheng Liu, Xiangyu Li, Hao Wen, Huiwen Zheng, Yan Liang, Yuanchun Li, Yunxin Liu*. [[pdf](https://arxiv.org/pdf/2504.14350)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Length_Budget-green)
- **Between Underthinking and Overthinking: An Empirical Study of Reasoning Length and correctness in LLMs**  
  *Jinyan Su, Jennifer Healey, Preslav Nakov, Claire Cardie*. [[pdf](https://arxiv.org/pdf/2505.00127)], 2025.04. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Over--thinking-green)
- **When Can Large Reasoning Models Save Thinking? Mechanistic Analysis of Behavioral Divergence in Reasoning**  
  *Rongzhi Zhu, Yi Liu, Zequn Sun, Yiwei Wang, Wei Hu*. [[pdf](https://www.arxiv.org/pdf/2505.15276)], 2025.05. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Over--thinking-green)
- **On Reasoning Strength Planning in Large Reasoning Models**  
  *Leheng Sheng, An Zhang, Zijian Wu, Weixiang Zhao, Changshuo Shen, Yi Zhang, Xiang Wang, Tat-Seng Chua*. [[pdf](https://arxiv.org/pdf/2506.08390)], [[code](https://github.com/AlphaLab-USTC/LRM-plans-CoT)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Reasoning_Length-green)
- **Is Long-to-Short a Free Lunch? Investigating Inconsistency and Reasoning Efficiency in LRMs**  
  *Shu Yang, Junchao Wu, Xuansheng Wu, Derek Wong, Ninhao Liu, Di Wang*. [[pdf](https://arxiv.org/pdf/2506.19492)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Long2Short_Inconsistency-green)
- **Thought Anchors: Which LLM Reasoning Steps Matter?**  
  *Paul C. Bogdan, Uzay Macar, Neel Nanda, Arthur Conmy*. [[pdf](https://arxiv.org/pdf/2506.19143)], 2025.06. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Reasoning_Steps-green)
- **What Happened in LLMs Layers when Trained for Fast vs. Slow Thinking: A Gradient Perspective**  
  *Ming Li, Yanhong Li, Tianyi Zhou*. [[pdf](https://aclanthology.org/2025.acl-long.1545/)],  [[code](https://github.com/MingLiiii/Layer_Gradient?tab=readme-ov-file)], 2025.06. ![](https://img.shields.io/badge/ACL2025--Oral-orange)
- **Latent Chain-of-Thought? Decoding the Depth-Recurrent Transformer**  
  *Wenquan Lu, Yuechuan Yang, Kyle Lee, Yanshu Li, Enqi Liu*. [[pdf](https://arxiv.org/pdf/2507.02199)], [[code](https://github.com/wenquanlu/huginn-latent-cot)], 2025.07. ![](https://img.shields.io/badge/Arxiv-orange)

### Applications

- **Pruning the Unsurprising: Efficient Code Reasoning via First-Token Surprisal**  
  *Wenhao Zeng, Yaoning Wang, Chao Hu, Yuling Shi, Chengcheng Wan, Hongyu Zhang, Xiaodong Gu*. [[pdf](https://arxiv.org/pdf/2508.05988)], [[code](https://github.com/Zengwh02/ASAP)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Code-green)
- **Audio-Thinker: Guiding Audio Language Model When and How to Think via Reinforcement Learning**  
  *Shu Wu, Chenxing Li, Wenfu Wang, Hao Zhang, Hualei Wang, Meng Yu, Dong Yu*. [[pdf](https://arxiv.org/pdf/2508.08039)], 2025.08. ![](https://img.shields.io/badge/Arxiv-orange) ![](https://img.shields.io/badge/Audio-green)

## Blog & Project

**Optimizing LLM Test-Time Compute Involves Solving a Meta-RL Problem.** CMU, University of Toronto. [[blog](https://blog.ml.cmu.edu/2025/01/08/optimizing-llm-test-time-compute-involves-solving-a-meta-rl-problem/)], 2025.01.

**Understanding R1-Zero-Like Training: A Critical Perspective.** Sea AI Lab. [[paper](https://github.com/sail-sg/understand-r1-zero/blob/main/understand-r1-zero.pdf)], [[code](https://github.com/sail-sg/understand-r1-zero)], 2025.03.

## Talks

**The Key Ingredients for Scaling Test-Time Compute.** [Aviral Kumar](https://aviralkumar2907.github.io/). Carnegie Mellon University. [[homepage](https://www.cs.cmu.edu/calendar/181689023)], [[video](https://www.bilibili.com/video/BV1suAteHEXS)], 2025.03.

## Resources

**Reading lists related to Efficient Reasoning**

- [Eclipsess/Awesome-Efficient-Reasoning-LLMs](https://github.com/Eclipsess/Awesome-Efficient-Reasoning-LLMs)
- [XiaoYee/Awesome_Efficient_LRM_Reasoning](https://github.com/XiaoYee/Awesome_Efficient_LRM_Reasoning)
- [Blueyee/Efficient-CoT-LRMs](https://github.com/Blueyee/Efficient-CoT-LRMs)
- [yueliu1999/Awesome-Efficient-Inference-for-LRMs](https://github.com/yueliu1999/Awesome-Efficient-Inference-for-LRMs)
- [DevoAllen/Awesome-Reasoning-Economy-Papers](https://github.com/DevoAllen/Awesome-Reasoning-Economy-Papers)
- [Hongcheng-Gao/Awesome-Long2short-on-LRMs](https://github.com/Hongcheng-Gao/Awesome-Long2short-on-LRMs)
- [EIT-NLP/Awesome-Latent-CoT](https://github.com/EIT-NLP/Awesome-Latent-CoT)
- [yzhangchuck/awesome-llm-reasoning-long2short-papers](https://github.com/yzhangchuck/awesome-llm-reasoning-long2short-papers)
- [yuelinan/Awesome-Efficient-R1-style-LRMs](https://github.com/yuelinan/Awesome-Efficient-R1-style-LRMs)

## Contributors

<a href="https://github.com/hemingkx/Awesome-Efficient-Reasoning/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=hemingkx/Awesome-Efficient-Reasoning" />
</a>

## Contributing to this paper list

-  There are cases where we miss important works in this field, please feel free to contribute and promote your awesome work or other related works here! Thanks for the efforts in advance.

