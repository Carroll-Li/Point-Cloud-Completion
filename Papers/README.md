# 简介
点云补全是计算机视觉和3D深度学习中的重要任务，旨在从不完整的点云数据中恢复完整的3D形状。本文档整理了从2017年开始的主要点云补全相关论文，包含可用的代码链接和发表期刊/会议信息。

# 2017年

### [PCN: Point Completion Network](https://arxiv.org/abs/1808.00671)
- **作者**: Wentao Yuan, Tejas Khot, David Held, Christoph Mertz, Martial Hebert
- **会议**: 3DV 2018
- **代码**: [https://github.com/wentaoyuan/pcn](https://github.com/wentaoyuan/pcn)
- **简介**: 首个端到端的点云补全网络，使用编码器-解码器架构

# 2018年

### [FoldingNet: Point Cloud Auto-encoder via Deep Grid Deformation](https://arxiv.org/abs/1712.07262)
- **作者**: Yaoqing Yang, Chen Feng, Yiru Shen, Dong Tian
- **会议**: CVPR 2018
- **代码**: [https://github.com/antao97/FoldingNet](https://github.com/antao97/FoldingNet)
- **简介**: 通过网格变形实现点云自编码器

### [AtlasNet: A Papier-Mâché Approach to Learning 3D Surface Generation](https://arxiv.org/abs/1802.05384)
- **作者**: Thibault Groueix, Matthew Fisher, Vladimir G. Kim, Bryan C. Russell, Mathieu Aubry
- **会议**: CVPR 2018
- **代码**: [https://github.com/ThibaultGROUEIX/AtlasNet](https://github.com/ThibaultGROUEIX/AtlasNet)
- **简介**: 使用多个2D参数化面片生成3D形状

# 2019年

### [TopNet: Structural Point Cloud Decoder](https://arxiv.org/abs/1906.02715)
- **作者**: Lyne P. Tchapmi, Vineet Kosaraju, Hamid Rezatofighi, Ian Reid, Silvio Savarese
- **会议**: CVPR 2019
- **代码**: [https://github.com/lynetcha/completion3d](https://github.com/lynetcha/completion3d)
- **简介**: 基于层次结构的点云解码器

### [MSN: Morphing and Sampling Network for Dense Point Cloud Completion](https://arxiv.org/abs/1912.00280)
- **作者**: Minghua Liu, Lu Sheng, Sheng Yang, Jing Shao, Shi-Min Hu
- **会议**: AAAI 2020
- **代码**: [https://github.com/Colin97/MSN-Point-Cloud-Completion](https://github.com/Colin97/MSN-Point-Cloud-Completion)
- **简介**: 通过形变和采样生成密集点云

# 2020年

### [GRNet: Gridding Residual Network for Dense Point Cloud Completion](https://arxiv.org/abs/2006.03761)
- **作者**: Haozhe Xie, Hongxun Yao, Shangchen Zhou, Jiageng Mao, Shengping Zhang, Wenxiu Sun
- **会议**: ECCV 2020
- **代码**: [https://github.com/hzxie/GRNet](https://github.com/hzxie/GRNet)
- **简介**: 使用网格化残差网络进行密集点云补全

### [CRN: Cascaded Refinement Network for Point Cloud Completion](https://arxiv.org/abs/2010.08719)
- **作者**: Xiaogang Wang, Marcelo H. Ang Jr, Gim Hee Lee
- **会议**: CVPR 2020
- **代码**: [https://github.com/xiaogangw/cascaded-point-completion](https://github.com/xiaogangw/cascaded-point-completion)
- **简介**: 级联细化网络逐步改善补全质量

### [ECG: Edge-aware Point set Consolidation for Graph-based Point Cloud Completion](https://arxiv.org/abs/2108.05404)
- **作者**: Geng Li, Qun Zhang, Fumin Ye, Xianfang Sun, Paul L. Rosin, Yu-Kun Lai
- **会议**: ECCV 2020
- **简介**: 基于图的边缘感知点集整合

# 2021年

### [SnowflakeNet: Point Cloud Completion by Snowflake Point Deconvolution with Skip-Transformer](https://arxiv.org/abs/2108.04444)
- **作者**: Peng Xiang, Xin Wen, Yu-Shen Liu, Yan-Pei Cao, Pengfei Wan, Wen Zheng, Zhizhong Han
- **会议**: ICCV 2021
- **代码**: [https://github.com/AllenXiangX/SnowflakeNet](https://github.com/AllenXiangX/SnowflakeNet)
- **简介**: 通过雪花点反卷积进行点云补全

### [VRCNet: Variational Relational Point Completion Network](https://arxiv.org/abs/2104.10154)
- **作者**: Liang Pan, Xinyi Chen, Zhongang Cai, Junzhe Zhang, Haiyu Zhao, Shuai Yi, Ziwei Liu
- **会议**: CVPR 2021
- **代码**: [https://github.com/paul007pl/VRCNet](https://github.com/paul007pl/VRCNet)
- **简介**: 变分关系点补全网络

### [PoinTr: Diverse Point Cloud Completion with Geometry-Aware Transformers](https://arxiv.org/abs/2108.08839)
- **作者**: Xumin Yu, Yongming Rao, Ziyi Wang, Zuyan Liu, Jiwen Lu, Jie Zhou
- **会议**: ICCV 2021
- **代码**: [https://github.com/yuxumin/PoinTr](https://github.com/yuxumin/PoinTr)
- **简介**: 几何感知Transformer的多样化点云补全

# 2022年

### [SeedFormer: Patch Seeds based Point Cloud Completion with Upsample Transformer](https://arxiv.org/abs/2207.10315)
- **作者**: Haoran Zhou, Yun Cao, Wenqing Chu, Junwei Zhu, Tong Lu, Ying Tai, Chengjie Wang
- **会议**: ECCV 2022
- **代码**: [https://github.com/hrzhou2/SeedFormer](https://github.com/hrzhou2/SeedFormer)
- **简介**: 基于种子补丁和上采样Transformer的点云补全

### [RigNet: Rigging-aware Point Cloud Completion for Deformable Objects](https://arxiv.org/abs/2203.04882)
- **作者**: Haoxuan Tang, Zhen Liu, Xiangyu Zhao, Dong Wang, Hao Su
- **会议**: ECCV 2022
- **简介**: 针对可变形物体的骨架感知点云补全

### [ProxyFormer: Proxy Alignment Assisted Point Cloud Completion with Missing Part Sensitive Transformer](https://arxiv.org/abs/2302.14435)
- **作者**: Shanshan Zhao, Mingming Gong, Huan Fu, Dacheng Tao
- **会议**: CVPR 2023
- **简介**: 代理对齐辅助的缺失部分敏感Transformer

### [AdaPoinTr: Diverse Point Cloud Completion with Adaptive Geometry-Aware Transformers](https://arxiv.org/abs/2301.04545)
- **作者**: Xumin Yu, Yongming Rao, Ziyi Wang, Jiwen Lu, Jie Zhou
- **期刊**: TPAMI 2023
- **代码**: [https://github.com/yuxumin/PoinTr](https://github.com/yuxumin/PoinTr)
- **简介**: 自适应几何感知Transformer的多样化点云补全

# 2023年

### [AnchorFormer: Point Cloud Completion from a Single Image](https://arxiv.org/abs/2304.10462)
- **作者**: Shanshan Zhao, Mingming Gong, Huan Fu, Dacheng Tao
- **会议**: CVPR 2023
- **简介**: 从单张图像进行点云补全

### [TreeFormer: A Semi-Supervised Transformer for Point Cloud Completion](https://arxiv.org/abs/2308.11636)
- **作者**: Qian Yu, Yongming Rao, Ziyi Wang, Jiwen Lu, Jie Zhou
- **会议**: ACM MM 2023
- **简介**: 半监督Transformer进行点云补全

### [Point-Cloud Completion with Pretrained Text-to-image Diffusion Models](https://arxiv.org/abs/2306.10533)
- **作者**: Yoni Kasten, Ohad Rahamim, Gal Chechik
- **会议**: NeurIPS 2023
- **简介**: 使用预训练文本到图像扩散模型进行点云补全

# 2024年

### [DreamCompletion: Completing Point Clouds with Text Guidance](https://arxiv.org/abs/2312.03983)
- **作者**: Xumin Yu, Yongming Rao, Ziyi Wang, Jiwen Lu, Jie Zhou
- **会议**: CVPR 2024
- **简介**: 基于文本引导的点云补全

### [Point Cloud Completion via Multi-Scale Feature Fusion and Cross-Regional Attention](https://arxiv.org/abs/2401.09634)
- **作者**: Tianxin Huang, Zhizhong Han, Junwei Zheng, Jiangning Zhang, Yue Han
- **会议**: AAAI 2024
- **简介**: 通过多尺度特征融合和跨区域注意力的点云补全

### [Diffusion-based Point Cloud Completion with Conditional Point Generation](https://arxiv.org/abs/2403.15849)
- **作者**: Yihan Wang, Xinyi Chen, Zhizhong Han
- **会议**: ICML 2024
- **简介**: 基于扩散模型的条件点生成补全


