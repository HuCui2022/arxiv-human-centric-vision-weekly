# arXiv cs.CV 人体中心视觉论文周报（2026-08-24—2026-08-30）

> 数据源：[arXiv cs.CV recent](https://arxiv.org/list/cs.CV/recent) 与 arXiv 官方 API。筛选范围为首次提交时间（UTC）在 2026-08-24 00:00 至 2026-08-30 23:59、分类包含 `cs.CV` 的论文。题目与摘要均译为中文，并保留英文原标题。★ 表示已确认论文明确提供当前公开的源代码入口；仅有项目主页、演示、数据集或“未来开源”承诺的不标记。

## 一览

| 日期 | 主题 | 论文 |
|---|---|---|
| 08-24 | 动作识别 | [ByteAction：字节空间动作识别基础模型](https://arxiv.org/abs/2608.22760) |
| 08-24 | 人体运动生成 | [时空解耦的自回归扩散人体运动生成模型](https://arxiv.org/abs/2608.23279) |
| 08-24 | 三维人脸 | [使用下一尺度 Transformer 的照片级真人脸新视角合成](https://arxiv.org/abs/2608.23410) |
| 08-25 | 重光照 | [Luce：用于三维资产生成的可重光照高斯表示](https://arxiv.org/abs/2608.23943) |
| 08-25 | 时序动作分割 | [ConsensusTAS：长时程施工视频的自监督时序动作分割](https://arxiv.org/abs/2608.24043) |
| 08-25 | 动作/手势表征 | [用于四维点云视频自监督学习的掩码点管联合嵌入预测](https://arxiv.org/abs/2608.24093) |
| 08-25 | 重光照 | [ExMesh++：从多视图图像到可重光照 UV-PBR 网格资产](https://arxiv.org/abs/2608.24109) |
| 08-25 | 人体姿态 | [用于抗阻训练技术评估的无标记姿态估计](https://arxiv.org/abs/2608.24384) |
| 08-25 | 动作理解 | [MoTE：面向多任务视频理解的任务专家混合模型](https://arxiv.org/abs/2608.24763) |
| 08-26 | 手语识别 | [SMART：统一手语识别与定位的 MLLM 引导时间对齐](https://arxiv.org/abs/2608.25493) |
| 08-26 | 动作预判 | [面向低延迟人体动作预判的姿态锚定光流](https://arxiv.org/abs/2608.25495) |
| 08-26 | 手势生成 | [InteractGesture：连续流式伴语手势控制的渐进分块引导](https://arxiv.org/abs/2608.25734) |
| 08-27 | 手势生成 | [RoboGesture：用于人形机器人交互的实时语义对齐伴语手势生成](https://arxiv.org/abs/2608.28693) |
| 08-27 | 人体运动预测 | [复杂场景中的多人运动预测](https://arxiv.org/abs/2608.27039) |
| 08-27 | 三维人体—物体交互 | ★ [利用大型重建模型重建交互中的人与物](https://arxiv.org/abs/2608.27407) |
| 08-27 | 第一视角动作理解 | [VidParse：像专家一样在线解析第一视角操作流程](https://arxiv.org/abs/2608.27562) |
| 08-27 | 极低照姿态感知 | [将量子感知建模为概率事件](https://arxiv.org/abs/2608.27584) |
| 08-28 | 暴力/交互识别 | [交互表示究竟测量了什么？弱监督暴力检测中的事件前可分性](https://arxiv.org/abs/2608.27879) |
| 08-28 | 指示手势 | [DeicticVLA：在单一 VLA 中统一语言与指示手势指令模式](https://arxiv.org/abs/2608.28108) |
| 08-28 | 三维人体—物体交互 | [GraspHOI：从单张自然图像重建含手指级抓握的全身三维人—物交互](https://arxiv.org/abs/2608.28386) |
| 08-28 | 手语生成 | [SignRR：检索并精炼真实运动以生成手语](https://arxiv.org/abs/2608.28568) |
| 08-28 | 人体姿态与光照 | [文本驱动的艺术舞台编排：从绘画生成姿态、光照和相机参考](https://arxiv.org/abs/2608.28823) |
| 08-29 | 动作识别 | [用于联邦视频域适应的多尺度时间域对齐](https://arxiv.org/abs/2608.29186) |
| 08-29 | 重光照 | [LightFuse：通过多次扫描融合与二维高斯光线追踪实现可重光照交互场景重建](https://arxiv.org/abs/2608.29269) |

## 论文详情

### 1. ByteAction：字节空间动作识别基础模型

**原标题：** ByteAction: Byte-space Action Recognition Foundation Model  
**作者：** Fangcheng Li, Zhen Yu, Kejun Wu, Qiong Liu, You Yang  
**主题：** 动作识别、压缩码流、鲁棒性  
**arXiv：** https://arxiv.org/abs/2608.22760

**摘要翻译：** 字节空间动作识别（BAR）无需像素解码，直接从压缩图像码流识别人类动作，因此不依赖文件完整性和像素重建，天然适用于隐私敏感场景且能抵抗码流损坏。本文提出 ByteAction 基础模型，采用双视图字节级识别框架：通过码流模式增强构造弱损坏和强损坏视图，再由共享 ByteFormer 编码。模型同时优化分类和损坏一致性目标。码流模式增强将一维字节序列重排为二维字节矩阵并进行区域擦除，以学习跨区域字节依赖；损坏一致性训练则借助双向 KL 散度约束不同损坏程度下的预测稳定性。在 Stanford40、PPMI 和 PASCAL VOC 2012 Action 的图像码流上，该模型在所有损坏场景中达到先进鲁棒性，同时保持有竞争力的完整码流性能。

### 2. 时空解耦的自回归扩散人体运动生成模型

**原标题：** Spatiotemporally Decoupled Autoregressive Diffusion Model for Human Motion Generation  
**作者：** Chengqun Yang, Liang Xu, Yanping Li, Fulong Liu, Jingnan Gao, Weili Zeng, Yichao Yan  
**主题：** 文本驱动人体运动生成、可控编辑  
**arXiv：** https://arxiv.org/abs/2608.23279

**摘要翻译：** 文本驱动人体运动合成依赖运动表示和生成架构。VQ 表示存在信息损失，连续表示若把全身压入整体潜空间又会限制身体部位级灵活性；扩散与自回归扩散同样缺少细粒度部位控制。作者提出时空解耦框架 DeMoDiff，同时重构表示和架构。时空 VAE 不再压缩整体运动，而是逐关节编码；自回归扩散生成器加入时空掩码与注意力，从而兼顾生成和可控编辑。在 HumanML3D 与 KIT-ML 上，模型取得先进重建性能和有竞争力的运动生成结果，并展示出强时间与空间编辑能力。

### 3. 使用下一尺度 Transformer 的照片级真人脸新视角合成

**原标题：** Photorealistic Novel View Synthesis of Human Faces using Next-Scale Transformers  
**作者：** Federico Stella, Fei Jiang, Zhongshi Jiang, Zohar Barzelay, Emanuel Garbin, Amin Jourabloo, Liuhao Ge  
**主题：** 人体中心新视角合成、三维人脸  
**arXiv：** https://arxiv.org/abs/2608.23410

**摘要翻译：** 高分辨率、多目标相机条件下的人物新视角合成，需要同时保持身份、细节与几何一致性。本文把下一尺度自回归范式扩展到人体中心视图合成，在一次前向传播中支持更高分辨率、多视图输出和更强跨视图一致性，并在涵盖多样身份和服装的合成人脸数据上训练。该范式无需二维预训练，可利用低分辨率通用预训练，只在最后阶段使用完整高分辨率专用图像，因此能以更少的专用数据收敛。模型生成清晰真实的视图，并可同步产生多个目标视角。与像素对齐三维高斯提升模型组合后，还能从多视图人脸输入得到准确、照片级真实的三维人脸模型。

### 4. Luce：用于三维资产生成的可重光照高斯表示

**原标题：** Luce: Relightable Gaussians for 3D Asset Generation  
**作者：** Mayank Singh 等  
**主题：** 单图三维生成、PBR、重光照  
**arXiv：** https://arxiv.org/abs/2608.23943

**摘要翻译：** 高保真图像到三维生成需要同时捕获几何和外观；若要支持重光照及标准渲染流程，还需反照率、金属度—粗糙度和表面法线等 PBR 模态。Luce 在体素化多模态高斯云中统一几何与 PBR 材质，并为每种模态设置专用高斯基元。VAE 将其压缩到统一的材质感知潜空间，整流流 Transformer 再从单张图像生成该潜变量，并用预训练图像编码器的多层特征保留语义和空间细节。潜变量可解码为可重光照 PBR 高斯及可选纹理网格。在 Toys4K 上，Luce 相比最强基线将 FID 改善 28%；在 AI 生成图像基准上，CLIP 对齐分数由 0.8299 提高到 0.8519。

### 5. ConsensusTAS：长时程施工视频的自监督时序动作分割

**原标题：** ConsensusTAS: Self-Supervised Temporal Action Segmentation for Long-Horizon Construction Videos  
**作者：** Xiaoshan Zhou, Yafei Sun  
**主题：** 时序动作分割、自监督学习  
**arXiv：** https://arxiv.org/abs/2608.24043

**摘要翻译：** 顺序施工活动识别可帮助协作机器人理解工人的当前与后续动作，但既有研究多停留在攀爬、搬运、行走等类别分类，缺少对长视频中细粒度动作转变的识别，而标注时间边界成本很高。ConsensusTAS 是无标签自监督方法，利用多个候选分割之间的内部共识，把连续视频划分为不同活动阶段。在 GTEA、Breakfast 和 Assembly101 静态相机视频上，F1@10/F1@50 分别达到 73.08、64.33 和 33.50，优于先进方法。真实施工视频的事后评估显示，它能识别砌砖复合活动中的涂砂浆、放砖、按压和对齐等动作。模型无需计算昂贵的大型视觉语言模型，可在 CPU 上运行。

### 6. 用于四维点云视频自监督学习的掩码点管联合嵌入预测

**原标题：** Joint-Embedding Prediction of Masked Point Tubes for Self-Supervised Learning on 4D Point Cloud Videos  
**作者：** Jheng-Ling Lee, Shang-Tse Chen  
**主题：** 四维点云、动作与手势识别、自监督学习  
**arXiv：** https://arxiv.org/abs/2608.24093

**摘要翻译：** 四维点云视频的标注昂贵，而基于重建的预训练容易过度关注低层几何。本文提出 JEPA 风格框架，通过潜在点管预测从无标注时空点云学习：模型掩盖时空区域，不重建原始坐标，而是在特征空间利用可见上下文预测目标表示。作者加入草图化各向同性高斯正则化，在无需显式重建目标的情况下防止嵌入坍塌。该目标同时捕获空间结构和时间动态，并与下游语义识别对齐。动作和手势识别实验表明，所学表示可改善完整微调、少标签学习和跨数据集迁移。

### 7. ExMesh++：从多视图图像到可重光照 UV-PBR 网格资产

**原标题：** ExMesh++: From Multi-View Images to Relightable UV-PBR Mesh Assets via Topology-Adaptive Reconstruction and Decomposition  
**作者：** Chuanjin Fan, Lifan Wu, Wenjie Chang, Hanzhi Chang, Wenfei Yang, Tianzhu Zhang  
**主题：** 多视图重建、材质分解、重光照  
**arXiv：** https://arxiv.org/abs/2608.24109

**摘要翻译：** 可编辑、可重光照的网格资产需要良好拓扑、有效 UV 参数化和显式 PBR 材质贴图。现有重建通常先优化隐式场或高斯，再进行表面提取和纹理烘焙；逆渲染得到的材质与光照也常绑定在中间表示中，几何、材质和光照联合优化还可能相互补偿而产生歧义。ExMesh++ 采用分阶段方案：首先通过自适应顶点拆分和合并优化显式网格几何与拓扑，同时维持 UV 一致性；随后固定网格—UV 载体，共同优化 UV 空间 PBR 贴图和环境光照，并用共享材质的二次射线追踪建模一次漫反射间接光。实验显示其几何精度有竞争力、重光照效果强，且导出资产可直接用于标准 DCC 流程。

### 8. 用于抗阻训练技术评估的无标记姿态估计

**原标题：** Markerless Pose Estimation for Resistance Training Technique Assessment  
**作者：** Joseph Turner, Jeff Clark, Nawid Keshtmand  
**主题：** 人体姿态估计、运动生物力学  
**arXiv：** https://arxiv.org/abs/2608.24384

**摘要翻译：** 抗阻训练风险较高，而实验室动作分析虽能量化技术却不易普及。本文提出从普通视频评估抗阻训练技术的无标记姿态框架。使用 BlazePose 从深蹲、卧推和硬拉视频提取解剖标志并转换为关节角轨迹，以深蹲为主要案例，再用均方根误差与参考重复动作比较。结果表明，框架能恢复深蹲和硬拉的有意义运动学模式，量化不同重复动作并识别组内技术变化。性能明显受相机朝向和遮挡影响，非矢状面视角会扭曲二维关节角估计，但总体显示无标记姿态估计可支持实验室外的可及生物力学评估。

### 9. MoTE：面向多任务视频理解的任务专家混合模型

**原标题：** MoTE: Mixture of Task Experts for Multi-Task Video Understanding  
**作者：** Muhammad Asad Ali, Umar Khan, Nadia Robertini, Didier Stricker  
**主题：** 动作识别、动作预测、程序视频理解  
**arXiv：** https://arxiv.org/abs/2608.24763

**摘要翻译：** 程序视频语言模型需从相同视觉证据完成动作识别、预测和流程预测等异质任务。密集 Transformer 解码器在任务间共享前馈网络，容易纠缠任务行为；稀疏 MoE 的令牌级路由又不自然匹配任务级目标。MoTE 把大语言模型前馈网络转换为任务专属专家，同时共享多模态骨干；每个样本只走一条任务路由，因此激活计算量不随存储专家数量增长。VideoLLM-MoTE 在五个 COIN 基准上使用显式任务路由，五专家模型每样本激活约 20 亿 LLM 参数，平均 Top-1 准确率超过近期 VideoLLM，并优于相同专家拓扑下的密集全专家激活和学习式稀疏路由。

### 10. SMART：统一手语识别与定位的 MLLM 引导时间对齐

**原标题：** SMART: MLLM-guided Temporal Alignment for Unifying Sign Language Recognition and Spotting  
**作者：** Eunjee Choi, JungHoon Sung, Seongwhan Cho, Chu Xin, Younggeun Choi  
**主题：** 连续手语识别、手语定位  
**arXiv：** https://arxiv.org/abs/2608.25493

**摘要翻译：** 连续手语识别从未分割视频中在弱序列监督下预测 gloss 序列，但句子级标注难以提供细粒度时间和语义指导，传统视频—文本对齐还依赖大批量训练。SMART 使用多模态大模型生成的运动描述作为辅助语义线索，在小批量下稳定进行视频—文本对齐。多尺度时间适配器在 Transformer 编码期间建模时间交互；CSFormer 定位模块则把识别得到的 gloss 证据注入边界感知网络。由此识别特征帮助定位，定位监督也补充基于 CTC 的弱监督识别。在 PHOENIX14-T、CSL-Daily、大规模韩国手语及灾害安全韩国手语四个基准上，SMART 在识别和定位任务中均表现有效。

### 11. 面向低延迟人体动作预判的姿态锚定光流

**原标题：** Pose-Anchored Optical Flow for Low-Latency Human Action Anticipation in Human-Robot Teaming  
**作者：** Lewis de Zoete Grundy, Chris McCarthy, Christopher Fluke  
**主题：** 动作预判、人体姿态、人机协作  
**arXiv：** https://arxiv.org/abs/2608.25495

**摘要翻译：** 人机交互要求机器人在动作早期理解人的意图。稀疏骨架缺少细微运动线索，而密集光流计算昂贵。PoseOFF 以人体关节为锚点，在关节附近提取局部光流，将运动动态对齐到有语义意义的身体位置。多个基准和骨干架构上的动作预判实验表明，PoseOFF 持续提高识别准确率，尤其在早期观察比例下；模型观看更少动作序列即可达到相当或更佳性能。由于无需处理全帧运动，它适合实时和资源受限环境，可帮助交互机器人更早推断人体动作。

### 12. InteractGesture：连续流式伴语手势控制的渐进分块引导

**原标题：** InteractGesture: Progressive Chunk Guidance for Continuous Streaming Co-Speech Gesture Control  
**作者：** Ekkasit Pinyoanuntapong, Ajinkya Deogade, Paul Streli, Wenjing Zhang, Joanna Materzynska, Pu Wang, Vittorio Ferrari, Jie Shen  
**主题：** 伴语手势生成、流式运动控制  
**arXiv：** https://arxiv.org/abs/2608.25734

**摘要翻译：** 伴语手势生成已能从音频产生真实全身运动，但缺少单关节级空间控制。InteractGesture 是与模型无关的推理时方法，通过可微 RVQ-VAE 解码器引导扩散采样器的目标潜变量，并反向传播空间控制梯度。流式生成中，标准顺序推理会冻结先前分块，使未来约束无法修正早期轨迹并造成边界不连续。作者提出渐进分块引导，维护一组带交错延迟的可编辑分块潜变量，使空间约束可跨边界反向传播。在 BEAT2 上，该方法提高多关节空间控制同时保持手势质量，并支持稀疏关节定位、密集轨迹控制和方向指示。

### 13. RoboGesture：用于人形机器人交互的实时语义对齐伴语手势生成

**原标题：** RoboGesture: Real-Time Semantic-aligned Co-Speech Gestures Generation for Humanoid Interaction  
**作者：** Zifan Wang 等  
**主题：** 伴语手势、人形机器人、实时运动生成  
**arXiv：** https://arxiv.org/abs/2608.28693

**摘要翻译：** 让人形机器人针对人类语音实时生成同步且语义相关的手势，面临语义丰富数据稀缺、模型忽略音频而依赖运动惯性的“模态遮蔽”，以及实体安全的仿真到现实差距。RoboGesture 从数据、模型和控制联合设计完整交互系统。作者建立含 300 多类手势的数据集和自动化无碰撞机器人音频—运动合成流程；分层语义—声学对齐器从原始音频令牌提取多粒度韵律与语义线索，驱动基于条件流匹配扩散 Transformer 的流式运动生成器。抗惯性 CFG 掩码迫使模型使用音频控制信号，MPC 安全过滤器保证实体硬件上的实时无碰撞执行。Unitree G1 实验显示其安全性、节奏和语义适切性均优于基线。

### 14. 复杂场景中的多人运动预测

**原标题：** Multi-Person Human Motion Forecasting in Complex Scenes  
**作者：** Serdar Ozsoy, Lars Doorenbos, Juergen Gall  
**主题：** 多人运动预测、社会交互、人—物交互  
**arXiv：** https://arxiv.org/abs/2608.27039

**摘要翻译：** 复杂场景中的人体运动预测需要理解整个环境的过去与当前状态，并统一利用物体信息和社会交互。作者提出物体条件社会扩散模型 OCSD，将运动历史、多人交互和物体线索整合到一个条件扩散框架中。物体条件机制在每个去噪时间步调制过程，实现细粒度人—物推理；社会编码器则建模场景中所有人的交互。模型可自然处理变化的群体规模和复杂社会关系，并采样多个合理未来。在 Humans in Kitchens 与 HOI-M3 上达到先进结果，相较既有方法，两秒路径误差分别降低 121.5 mm（31.3%）和 130.5 mm（33.2%），长期预测也更真实。

### 15. ★ 利用大型重建模型重建交互中的人与物

**原标题：** Reconstructing Humans and Objects in Interaction using Large Reconstruction Models  
**作者：** Agniv Chatterjee, Georgios Pavlakos  
**主题：** 单图三维人体—物体交互重建  
**arXiv：** https://arxiv.org/abs/2608.27407

**摘要翻译：** 三维人—物交互重建受深度歧义、遮挡和物体形状变化影响。传统方法主要围绕重投影和接触约束，把参数人体模型与物体模板拟合到二维图像。MILO 转而利用大型重建模型的视觉能力，从单图恢复细致三维人—物交互。关键观察是，大型重建模型可提供保留人—物相对布局和邻近关系的几何支架，使任务转化为解释 LRM 网格：把网格分成人与物体部分，对人体拟合参数身体模型，并在有模板时选择性对齐物体模板。MILO 在多个基准和交互场景中取得强重建精度并超过既有基线。论文项目页明确提供 Code 入口。

### 16. VidParse：像专家一样在线解析第一视角操作流程

**原标题：** VidParse: Online Parsing of Egocentric Procedures Like a Pro  
**作者：** Anubhav Gupta, Archit Kambhamettu, Vatsal Agarwal, Pulkit Kumar, Abhinav Shrivastava  
**主题：** 第一视角动作理解、在线流程解析  
**arXiv：** https://arxiv.org/abs/2608.27562

**摘要翻译：** 把连续、嘈杂的第一视角视频转换为离散且有序的动作步骤，受到强烈自运动、短暂遮挡及非脚本化人—物交互类内差异的影响，帧级在线模型容易过分割并发生结构坍塌。VidParse 是无需训练的在线框架，把活动理解视为图约束推理。它利用操控锚定特征的时间相似度矩阵动态发现语义转变；特征来自冻结基础模型并强调前景手—物交互。束搜索解码器再使用诱导出的流程任务图约束合法动作转移并剪除不可能轨迹。该方法把稳健视觉片段绑定到硬流程约束，在复杂多步骤解析中相对强基线最高提升 10 倍，且无需梯度更新。

### 17. 将量子感知建模为概率事件

**原标题：** Quanta Perception as Probabilistic Events  
**作者：** Varun Sundar, Pavan Thodima, Sacha Jungerman, Mohit Gupta  
**主题：** 极低照视觉、人体姿态估计、量子传感  
**arXiv：** https://arxiv.org/abs/2608.27584

**摘要翻译：** 固定曝光的传统传感器在光子稀少或快速动态下存在灵敏度、动态范围和时间分辨率权衡；量子传感器虽检测单光子，其数据流却远超实时计算预算。本文提出“概率事件”计算原语：计算距上次强度变化时间的后验，把光子流表示为递归信念状态。不同于固定阈值事件相机，该贝叶斯递归产生运动自适应场景通量、高保真活动图和基于熵的感知不确定性。在约 0.05 lux 下，它无需重训视觉模型即可估计奔跑者姿态。方法可在普通 GPU 上处理每秒超过 5 万量子帧，输出达千赫兹，比先进量子重建基线最高快四个数量级。

### 18. 交互表示究竟测量了什么？弱监督暴力检测中的事件前可分性

**原标题：** What Do Interaction Representations Actually Measure? Pre-Event Separability in Weakly-Supervised Violence Detection  
**作者：** Parishruthi Ganesh  
**主题：** 暴力行为检测、人体姿态、基准偏差  
**arXiv：** https://arxiv.org/abs/2608.27879

**摘要翻译：** 本文在保持跟踪器、时间头、监督、划分和评测一致的情况下，比较从粗粒度框几何到手工姿态、增强姿态描述及原始关节学习编码器的五种交互表示。姿态表示均未超过粗几何，但小规模异常样本无法排除微小效应。扩展到冻结视觉编码器并在更大的 XD-Violence 上复现后，人物裁剪外观和全帧上下文都远胜几何，但全帧上下文不弱于、甚至优于人物裁剪。仅使用异常事件发生前帧评分，排除序列长度线索后，仍保留 39%–91% 的高于随机可分性。检查发现标题卡和平台水印等来源伪迹。由此，视频级 AUC 混合了事件证据与事件前来源线索，可能掩盖表示差异。

### 19. DeicticVLA：在单一 VLA 中统一语言与指示手势指令模式

**原标题：** DeicticVLA: Unifying Instruction Modes Based on Language and Deictic Gestures in a Single VLA  
**作者：** Kango Yanagida, Tatsuya Aoki, Yuichiro Yoshikawa, Takato Horii  
**主题：** 指示手势、视觉语言动作模型、人机交互  
**arXiv：** https://arxiv.org/abs/2608.28108

**摘要翻译：** 当多个物体类别相同或外观相似时，纯语言难以可靠指定操作目标。DeicticVLA 通过文本提示补全和指示手势定位，把语言指令、视觉—语言指令及视觉指令统一为文本提示与指示掩码，使一个预训练 VLA 支持三种模式。在共享骨干、演示和训练步数下，作者比较两种 RGB 视觉提示、两种独立通道掩码提示和三种训练策略。两阶段训练提高模型在未见布局中使用指示掩码的能力，第二阶段保留语言数据可减轻遗忘。三个真实任务中，同一策略支持全部模式；在未见表达、外观变化和新物体下，视觉—语言与视觉指令优于纯语言，对未见类别成功率均为 100%，联合训练纯语言仅 16.7%。

### 20. GraspHOI：从单张自然图像重建含手指级抓握的全身三维人—物交互

**原标题：** GraspHOI: Full-Body 3D Human-Object Reconstruction with Finger-Level Grasps from a Single In-the-Wild Image  
**作者：** Semin Kim, Haechan Shin, Jongyoo Kim  
**主题：** 全身三维 HOI、手部抓握、单图重建  
**arXiv：** https://arxiv.org/abs/2608.28386

**摘要翻译：** 现有单目全身三维 HOI 方法没有把显式手指级抓握优化与类别无关物体重建结合，手指即使在整体人—物布局合理时仍可能悬空或穿透物体。GraspHOI 首次从单张自然图像重建全身三维 HOI，并针对重建物体显式优化手指关节。它无需预定义网格或固定类别词表，分别重建身体、双手和物体，通过深度注册和图像空间对齐放入度量相机空间；遮挡感知的掌面对应把物体安置到抓握手中，接触感知优化再调整手臂和手指，使其形成表面接触且避免过度穿透。四个基准、六种基线的结果显示，人—物相对位置、手部精度和接触合理性均得到改善。作者仅承诺未来发布完整代码，因此不标 ★。

### 21. SignRR：检索并精炼真实运动以生成手语

**原标题：** SignRR: Retrieve and Refine Real Motion for Sign Language Production  
**作者：** Fidel Omar Tito Cruz, Angie Sanchez Marquina, Summy Farfan, Gissella Bejarano  
**主题：** 手语生成、运动检索与精炼  
**arXiv：** https://arxiv.org/abs/2608.28568

**摘要翻译：** 手语生成通常从口语经 gloss 生成连续姿态。纯生成模型从先验或噪声合成，难以保存罕见手形和手语者特有发音；检索方法复用真实清晰片段，但混合不同手语者和协同发音上下文会在全序列造成节奏与风格不一致。SignRR 提出“检索—精炼”范式：从真实检索运动出发，而非从头生成，再把它精炼为全局一致序列。系统以真实手语片段字典初始化运动，并用部位感知残差 VQ-VAE 精炼整个序列；残差量化保留精细手部关节，时间长度差异则在潜空间处理。在 PHOENIX14T 和 CSL-Daily 上，SignRR 的反向翻译性能达到先进水平，同时保持有竞争力的姿态质量。

### 22. 文本驱动的艺术舞台编排：从绘画生成姿态、光照和相机参考

**原标题：** Text-Driven Artistic Staging: Pose, Lighting, and Camera References from Paintings  
**作者：** Yunge Wen  
**主题：** 人体姿态生成、光照估计、三维舞台编排  
**arXiv：** https://arxiv.org/abs/2608.28823

**摘要翻译：** 艺术家协调人体姿态、照明和相机位置传达叙事与情感，但生成方法通常独立建模这些因素。本文提出“文本到可编辑三维舞台”任务，从情感描述联合生成人体姿态、主光源和相机配置。作者从 2,328 幅人物画中重建 SMPL 身体、估计低频光照、恢复相机参数，并与 ArtEmis 描述配对，构建 11,911 个文本—舞台样本。流匹配 Transformer 支持数量可变的人物，并为每个提示生成多个舞台方案。在留出描述上，模型检索 R@1 达 32.2%，而 CLIP 最近邻为 16.6%，同时大致保持语料级多样性，说明可从文本生成可编辑、情感条件化的三维舞台参考。

### 23. 用于联邦视频域适应的多尺度时间域对齐

**原标题：** Multi-Scale Temporal Domain Alignment for Federated Video Domain Adaptation  
**作者：** Lee En-Yi Hannah, Haozhi Cao, Yuecong Xu  
**主题：** 跨域动作识别、联邦学习  
**arXiv：** https://arxiv.org/abs/2608.29186

**摘要翻译：** 联邦视频域适应可在保护隐私的同时协同学习分布式非独立同分布视频，但时间信息对齐研究不足。METAL 在多个时间分辨率利用时序信息，仅交换模型参数以改善跨域动作识别。源客户端按尺度训练 Transformer 编码器，目标服务器在每个尺度独立进行知识投票以生成稳健伪标签；新的 L2 方差惩罚在尺度知识蒸馏中约束跨尺度一致性，防止单一尺度支配。后期融合聚合各尺度特征，融合头通过置信度加权尺度预测进行蒸馏。在 Epic-Kitchens-55 和 Daily-DA 上达到先进性能，相比现有联邦域适应最高提升 28.47%。论文仅称未来开源，因此不标 ★。

### 24. LightFuse：通过多次扫描融合与二维高斯光线追踪实现可重光照交互场景重建

**原标题：** LightFuse: Relightable Interactive Gaussian Scene Reconstruction via Multi-Scan Fusion and 2D Gaussian Ray Tracing  
**作者：** Haonan Zhou, Gaoxiang Linghu, Youlin Jia, Hongyu Cui, Kewei Wei, Kaiyue Zhou, Bruce X. B. Yu, Gaoang Wang  
**主题：** 交互场景重建、材质—光照分解、重光照  
**arXiv：** https://arxiv.org/abs/2608.29269

**摘要翻译：** 可重光照交互场景重建希望从不同物体布局的扫描构建可编辑三维模型，并在新光照下渲染新布局。既有方法或把光照烘焙到外观中，或仅针对固定场景恢复材质和照明，编辑布局后阴影与间接光会不一致。LightFuse 是二维高斯框架，通过显式材质—光照分解和物理重光照扩展交互场景重建。它先跨状态融合观察，重建共享背景和可移动物体，再进行面向光线追踪的几何细化；随后利用可微一次反弹光线追踪分阶段训练，把共享金属度—粗糙度材质与状态专属环境光分离。所得场景支持重排物体、编辑材质和重光照。合成场景上相对最强基线平均提高 9.74 dB PSNR 和 0.121 SSIM。

## 筛选说明

- 本周共纳入 24 篇。与相机/物体六自由度姿态估计、点云配准、标志板定位等有关但不以人体为中心的论文已排除。
- 本周未发现以传统单一光源颜色估计或计算色恒常为核心的论文；光照方向纳入了 Luce、ExMesh++、艺术舞台编排和 LightFuse 等直接涉及光照估计、材质—光照分解或重光照的工作。
- 仅 MILO 明确提供了当前可访问的代码入口，因此标记 ★；“代码将在录用后/未来发布”的论文不标记。
- arXiv 是预印本平台；本文“发表日期”指首次提交日期，不等同于正式同行评审发表时间。
