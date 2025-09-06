# 简介
点云补全是计算机视觉和3D深度学习中的重要任务，旨在从不完整的点云数据中恢复完整的3D形状。本文档整理了从2017年开始的主要点云补全相关论文，包含可用的代码链接和发表期刊/会议信息。

# 2017年

### [PCN: Point Completion Network](https://arxiv.org/abs/1808.00671)
- **作者**: Wentao Yuan, Tejas Khot, David Held, Christoph Mertz, Martial Hebert
- **会议**: 3DV 2018
- **代码**: [https://github.com/wentaoyuan/pcn](https://github.com/wentaoyuan/pcn)
- **简介**: 首个端到端的点云补全网络，使用编码器-解码器架构；采用粗到细两阶段预测（coarse-to-fine），以Chamfer Distance等度量进行监督，兼顾全局形状与局部细节。

# 2018年

### [FoldingNet: Point Cloud Auto-encoder via Deep Grid Deformation](https://arxiv.org/abs/1712.07262)
- **作者**: Yaoqing Yang, Chen Feng, Yiru Shen, Dong Tian
- **会议**: CVPR 2018
- **代码**: [https://github.com/antao97/FoldingNet](https://github.com/antao97/FoldingNet)
- **简介**: 通过网格变形实现点云自编码器；将二维规则网格“折叠”到三维表面上，提供通用的点云生成先验，常作为补全任务的基础模块。

### [AtlasNet: A Papier-Mâché Approach to Learning 3D Surface Generation](https://arxiv.org/abs/1802.05384)
- **作者**: Thibault Groueix, Matthew Fisher, Vladimir G. Kim, Bryan C. Russell, Mathieu Aubry
- **会议**: CVPR 2018
- **代码**: [https://github.com/ThibaultGROUEIX/AtlasNet](https://github.com/ThibaultGROUEIX/AtlasNet)
- **简介**: 原文做的是三角网格的表面重建，但是也可用作点云补全。

# 2019年

### [TopNet: Structural Point Cloud Decoder](https://openaccess.thecvf.com/content_CVPR_2019/papers/Tchapmi_TopNet_Structural_Point_Cloud_Decoder_CVPR_2019_paper.pdf)
- **作者**: Lyne P. Tchapmi, Vineet Kosaraju, Hamid Rezatofighi, Ian Reid, Silvio Savarese
- **会议**: CVPR 2019
- **代码**: [https://github.com/lynetcha/completion3d](https://github.com/lynetcha/completion3d)
- **简介**: 基于层次结构的点云解码器；树形解码自上而下递归分裂生成点，使结构一致性更强，适合从稀疏到稠密的补全过程。

### [MSN: Morphing and Sampling Network for Dense Point Cloud Completion](https://arxiv.org/abs/1912.00280)
- **作者**: Minghua Liu, Lu Sheng, Sheng Yang, Jing Shao, Shi-Min Hu
- **会议**: AAAI 2020
- **代码**: [https://github.com/Colin97/MSN-Point-Cloud-Completion](https://github.com/Colin97/MSN-Point-Cloud-Completion)
- **简介**: 通过形变和采样生成密集点云；先形变初始点集逼近目标拓扑，再基于重要性采样进行致密化，兼顾全局结构与局部细节。

# 2020年

### [GRNet: Gridding Residual Network for Dense Point Cloud Completion](https://arxiv.org/abs/2006.03761)
- **作者**: Haozhe Xie, Hongxun Yao, Shangchen Zhou, Jiageng Mao, Shengping Zhang, Wenxiu Sun
- **会议**: ECCV 2020
- **代码**: [https://github.com/hzxie/GRNet](https://github.com/hzxie/GRNet)
- **简介**: 使用网格化残差网络进行密集点云补全；将点云栅格化到3D网格上进行卷积与残差学习，再反投影为点，鲁棒性较强。

### [CRN: Cascaded Refinement Network for Point Cloud Completion](https://arxiv.org/abs/2010.08719)
- **作者**: Xiaogang Wang, Marcelo H. Ang Jr, Gim Hee Lee
- **会议**: CVPR 2020
- **代码**: [https://github.com/xiaogangw/cascaded-point-completion](https://github.com/xiaogangw/cascaded-point-completion)
- **简介**: 级联细化网络逐步改善补全质量；采用多阶段上采样与残差修复，每阶段同时利用局部几何与全局上下文增强细节。

# 2021年

### [SnowflakeNet: Point Cloud Completion by Snowflake Point Deconvolution with Skip-Transformer](https://arxiv.org/abs/2108.04444)
- **作者**: Peng Xiang, Xin Wen, Yu-Shen Liu, Yan-Pei Cao, Pengfei Wan, Wen Zheng, Zhizhong Han
- **会议**: ICCV 2021
- **代码**: [https://github.com/AllenXiangX/SnowflakeNet](https://github.com/AllenXiangX/SnowflakeNet)
- **简介**: 通过雪花点反卷积进行点云补全；基于逐级点展开（snowflake deconv）与跳跃式Transformer融合，从粗到细生成结构化点簇。

### [VRCNet: Variational Relational Point Completion Network](https://arxiv.org/abs/2104.10154)
- **作者**: Liang Pan, Xinyi Chen, Zhongang Cai, Junzhe Zhang, Haiyu Zhao, Shuai Yi, Ziwei Liu
- **会议**: CVPR 2021
- **代码**: [https://github.com/paul007pl/VRCNet](https://github.com/paul007pl/VRCNet)
- **简介**: 变分关系点补全网络；引入变分推断建模形状先验，并通过关系推理捕获局部-全局依赖，提升多样性与不确定性建模。

### [PoinTr: Diverse Point Cloud Completion with Geometry-Aware Transformers](https://arxiv.org/abs/2108.08839)
- **作者**: Xumin Yu, Yongming Rao, Ziyi Wang, Zuyan Liu, Jiwen Lu, Jie Zhou
- **会议**: ICCV 2021
- **代码**: [https://github.com/yuxumin/PoinTr](https://github.com/yuxumin/PoinTr)
- **简介**: 几何感知Transformer的多样化点云补全；将补全视为点查询到几何记忆上的检索/生成，利用Transformer捕获长程依赖与形状先验，生成多样解。

# 2022年

### [SeedFormer: Patch Seeds based Point Cloud Completion with Upsample Transformer](https://arxiv.org/abs/2207.10315)
- **作者**: Haoran Zhou, Yun Cao, Wenqing Chu, Junwei Zhu, Tong Lu, Ying Tai, Chengjie Wang
- **会议**: ECCV 2022
- **代码**: [https://github.com/hrzhou2/SeedFormer](https://github.com/hrzhou2/SeedFormer)
- **简介**: 基于种子补丁和上采样Transformer的点云补全；先预测少量“种子”补丁，再用上采样Transformer逐步扩展到稠密点集，兼顾效率与质量。

# 2023年

### [ProxyFormer: Proxy Alignment Assisted Point Cloud Completion with Missing Part Sensitive Transformer](https://arxiv.org/abs/2302.14435)
- **作者**: Shanshan Zhao, Mingming Gong, Huan Fu, Dacheng Tao
- **会议**: CVPR 2023
- **简介**: 代理对齐辅助的缺失部分敏感Transformer；通过代理对齐在多尺度上融合可见与缺失区域的特征，并用对缺失部分更敏感的注意力机制聚焦难恢复区域，提升局部一致性与全局复原。

### [AdaPoinTr: Diverse Point Cloud Completion with Adaptive Geometry-Aware Transformers](https://arxiv.org/abs/2301.04545)
- **作者**: Xumin Yu, Yongming Rao, Ziyi Wang, Jiwen Lu, Jie Zhou
- **期刊**: TPAMI 2023
- **代码**: [https://github.com/yuxumin/PoinTr](https://github.com/yuxumin/PoinTr)
- **简介**: 自适应几何感知Transformer的多样化点云补全；在PoinTr基础上引入自适应查询与几何先验融合策略，提升跨类别泛化与结果多样性。

### [AnchorFormer: Point Cloud Completion from Discriminative Nodes](https://openaccess.thecvf.com/content/CVPR2023/papers/Chen_AnchorFormer_Point_Cloud_Completion_From_Discriminative_Nodes_CVPR_2023_paper.pdf)
- **作者**: Shanshan Zhao, Mingming Gong, Huan Fu, Dacheng Tao
- **会议**: CVPR 2023
- **简介**: 从辨别性节点（anchor）出发进行形状推断；以Transformer在锚点与上下文之间传播信息，先定位关键结构再扩展细节，兼顾全局骨架与局部精细度。

# 2024年

### [CRA-PCN: Point cloud completion with intra- and inter-level cross-resolution transformers](https://arxiv.org/abs/2401.01552)
- **作者**: Yi Rong, Haoran Zhou, Lixin Yuan, Cheng Mei, Jiahao Wang, Tong Lu
- **会议**: AAAI 2024
- **代码**: https://github.com/EasyRy/CRA-PCN
- **简介**: 提出层内与层间的跨分辨率Transformer交互机制；在多尺度特征之间进行高效信息流动，缓解尺度不匹配并增强细节修复能力。

### [GeoFormer: Learning point cloud completion with tri-plane integrated transformer](https://arxiv.org/abs/2408.06596)
- **作者**: Jinpeng Yu,Binbin Huang,Yuxuan Zhang,Huaxia Li,Xu Tang,Shenghua Gao
- **会议**: ACMM 2024
- **代码**: https://github.com/Jinpeng-Yu/GeoFormer
- **简介**: 将Tri-plane表示融入Transformer，将三维几何投影到三个正交平面以高效建模长程依赖；在保持效率的同时提升几何完整性与边界细节。

### [PointAttN: You only need attention for point cloud completion](https://ojs.aaai.org/index.php/AAAI/article/view/28356)
- **作者**: Jun Wang, Ying Cui, Dongyan Guo, Junxia Li, Qingshan Liu, Chunhua Shen
- **会议**: AAAI 2024 （arxiv上的为2022年版本）
- **代码**: https://github.com/ohhhyeahhh/PointAttN
- **简介**: 仅用注意力即可完成点云补全的范式；以多头注意力为核心进行全局-局部关系建模，结合坐标偏移预测实现从粗到细生成，结构简洁、性能强。

### [T-CorresNet: Template Guided 3D Point Cloud Completion with Correspondence Pooling Query Generation Strategy](https://arxiv.org/abs/2407.05008v1)
- **作者**: Fan Duan, Jiahao Yu, Li Chen
- **会议**: ECCV 2024
- **代码**: https://github.com/df-boy/T-CorresNet
- **简介**: 模板引导的点云补全方法；先以球面模板生成粗完整模板，再通过对应池化（Corres-Pooling）从输入与模板的点对应关系中动态生成查询tokens，驱动Transformer解码器从粗到细补全缺失区域，兼顾全局结构一致性与局部细节恢复。
# 2025年

### [PCDreamer: Point Cloud Completion Through Multi-view Diffusion Priors](https://cvpr.thecvf.com/virtual/2025/poster/35041)
- **作者**: Guangshun Wei, Yuan Feng, Long Ma, Chen Wang, Yuanfeng Zhou, Changjian Li
- **会议**: CVPR 2025
- **代码**: https://github.com/GSW-D/PCDreamerCode
- **简介**: 引入多视图扩散先验进行点云补全；将不完整形状映射到多视角空间，利用扩散模型对缺失区域进行生成与约束，再融合回三维，实现高保真与多样化补全。
