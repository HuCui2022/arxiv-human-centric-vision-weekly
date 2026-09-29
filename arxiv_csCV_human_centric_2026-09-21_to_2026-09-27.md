# arXiv cs.CV 人体中心视觉周报（2026-09-21 至 2026-09-27）

> 数据源：[arXiv cs.CV recent](https://arxiv.org/list/cs.CV/recent)、官方 API 与摘要页。按首次提交时间（UTC）筛选 2026-09-21 00:00 至 2026-09-27 23:59，且分类包含 `cs.CV`。★ 表示已核验公开仓库含实际实现代码；☆ 表示论文宣布或链接代码/项目，但当前实现尚不可核验。数据集或演示本身不作为代码标记。

## 概览

| 日期 | 主题 | 中文题目 |
|---|---|---|
| 09-26 | 人—物交互 | [TRACE：利用耦合流补全建模人—物交互](https://arxiv.org/abs/2609.32551) |
| 09-26 | 骨架动作识别 | ★ [利用凸包自适应平移消除骨架动作识别偏差](https://arxiv.org/abs/2609.32454) |
| 09-26 | 手语生成 | [RoboSTAR：面向人形机器人的下一尺度自回归手语翻译](https://arxiv.org/abs/2609.32250) |
| 09-26 | 步态识别 | [带重嵌入网络的两阶段多视图步态识别](https://arxiv.org/abs/2609.32244) |
| 09-26 | 人体运动预测 | [流中的骨架：面向人体运动预测的图结构流匹配](https://arxiv.org/abs/2609.32231) |
| 09-25 | 手语视频分割 | [观察语义变化：差分感知的句子级手语视频时序分割](https://arxiv.org/abs/2609.31148) |
| 09-25 | 流式数字人 | [何处、何时施加强制：用于流式化身的路由强制](https://arxiv.org/abs/2609.30963) |
| 09-25 | 人体运动生成 | [运动风格滑块：端点监督的人体运动扩散连续风格控制](https://arxiv.org/abs/2609.30795) |
| 09-25 | 人体运动生成 | ☆ [Timo：驯服用于人体运动生成的多模态扩散 Transformer](https://arxiv.org/abs/2609.30761) |
| 09-24 | 三维服装重建 | ☆ [OmniFabric：面向三维服装重建的连贯 UV 空间纹理合成](https://arxiv.org/abs/2609.30234) |
| 09-24 | 四维人体重建 | ☆ [Ego-Exo4D Human Meshes：面向第一/第三视角采集的四维人体运动重建数据集](https://arxiv.org/abs/2609.30187) |
| 09-24 | 手语数字人 | ☆ [PHOSA：照片级真实三维手语化身建模与基准](https://arxiv.org/abs/2609.29292) |
| 09-23 | 临床步态分析 | [DrGait：生物力学约束的可解释临床步态视觉推理](https://arxiv.org/abs/2609.28796) |
| 09-23 | 化身动作理解 | [视觉质量何时产生误导：渲染化身失真下的意图识别](https://arxiv.org/abs/2609.27560) |
| 09-23 | 人体中心视频 | [视觉语言模型能否分析人体中心视频？模型能力与人机协作流程图谱](https://arxiv.org/abs/2609.27327) |
| 09-22 | 可重光照数字人 | [Heartian：生理感知的可重光照高斯头部化身](https://arxiv.org/abs/2609.28539) |
| 09-22 | 人体运动预测 | [面向人体运动预测的潜空间数据集蒸馏](https://arxiv.org/abs/2609.26430) |
| 09-22 | 手势控制 | ☆ [身份门控无人机手势控制的部署研究](https://arxiv.org/abs/2609.25511) |
| 09-21 | 三维人体姿态 | ☆ [STA-TFM：跨视角时空聚合 Transformer 姿态估计](https://arxiv.org/abs/2609.24482) |
| 09-21 | 三维手部姿态 | ★ [利用视觉 Transformer 在相机空间精确估计手部姿态](https://arxiv.org/abs/2609.24424) |
| 09-21 | 步态分析 | [DiaSeg：从 DTW 路径提取对角片段以实现可解释步态分析](https://arxiv.org/abs/2609.24223) |
| 09-21 | 行人意图线索 | [面向安全人车交互的轻量行人头部朝向识别网络](https://arxiv.org/abs/2609.24193) |
| 09-21 | 重光照数字人 | [具有语义自适应运动—光照响应的可重光照三维化身重建](https://arxiv.org/abs/2609.24158) |

## 论文详情

### 1. TRACE：利用耦合流补全建模人—物交互

**原标题：** Harnessing Coupled Stream Completion For Human-Object Interaction Modeling<br>
**作者：** Dawei Guan, Di Yang, Jiangtao Wang<br>
**主题：** 人—物交互、文本条件生成、流匹配<br>
**arXiv：** [2609.32551](https://arxiv.org/abs/2609.32551)

**摘要翻译：** 文本条件人—物交互生成要求身体运动、物体轨迹与旋转以及手部动作保持协调。这些分量的尺度和动力学不同，却必须在接触、相对姿态和时间上保持一致。共享表示可能限制各流的独特结构，独立生成又使各流无法响应其他流的变化；只监督潜表示也不能直接约束解码后的接触。本文提出连续潜空间框架 TRACE，保持身体、物体和手部状态相互独立，同时耦合其更新。它将三类运动编码成不同潜变量，并根据完整的当前交互状态预测每个流的速度；解码运动上的几何损失进一步约束接触和随时间变化的物体相对运动。同一模型可根据其余两流补全任意一个缺失流，冻结的流特征还可输入语言模型用于交互理解。在 InterAct、OMOMO 和 BEHAVE 上，联合补全训练改善生成，冻结流特征也优于原始运动编码；TRACE 在 InterAct 的接触精确率、召回率和 F1 上均为比较方法最佳。

### 2. ★ 利用凸包自适应平移消除骨架动作识别偏差

**原标题：** De-biasing Skeleton-based Action Recognition with Convex Hull Adaptive Shift<br>
**作者：** Mengyuan Liu, Yuhang Wen, Yi Zhang, Songtao Wu, Hong Liu, Junsong Yuan, Beichen Ding<br>
**主题：** 骨架动作识别、多实体交互、归一化<br>
**arXiv：** [2609.32454](https://arxiv.org/abs/2609.32454)

**摘要翻译：** 骨架序列可表示单人动作和多人、多物体或机器人交互。现有方法常用后期融合，假设各实体独立同分布，以训练共享权重的稳健实体编码器；但各类骨架数据中观察到的实体偏差违反这一假设，并可能造成错误识别。偏差源于世界坐标系的初始设置，尤其是原点选择。本文提出基于凸包自适应平移的归一化方法 CHASE，以减小实体偏差。一个即插即用的参数化网络为输入骨架自适应施加合理平移，并保证新世界原点落在骨架凸包内，以约束搜索空间、避免不收敛；辅助目标利用成对分布距离进一步引导优化。子实体策略统一处理单实体和多实体动作，方法也兼容骨骼、速度等骨架内模态。本质上，CHASE 是降低实体偏差的归一化模块，使后续分类器在不同设置下表现更好。七个数据集上的实验表明，它可无缝集成多种骨干并显著提升性能。

### 3. RoboSTAR：面向人形机器人的下一尺度自回归手语翻译

**原标题：** RoboSTAR: Next-Scale Autoregressive Sign Language Translation for Humanoid Robots<br>
**作者：** Yujia Zeng, Chensheng Peng, Yuxin Chen, Alex Shao, Nathan Jew, Masayoshi Tomizuka<br>
**主题：** 手语生成、人体动作、人形机器人重定向<br>
**arXiv：** [2609.32250](https://arxiv.org/abs/2609.32250)

**摘要翻译：** 公共交流中的手语口译依赖合格专业译员，难以大规模部署，因此机器人手语可作为辅助无障碍界面。本文提出 RoBoSTAR，一种文本条件的手语生成框架，产生以人为中心、可重定向至机器人执行的手语运动，并可通过外部自动语音识别前端支持语音输入。传统自回归方法把运动展平成单一全分辨率 token 序列，迫使长程和局部依赖在同一时间粒度建模。RoBoSTAR 结合分部有限标量量化和下一尺度自回归，在逐渐细化的时间分辨率上生成运动，同时于每一步并行预测同步身体与手部 token。粗到细结构先提供紧凑长程上下文，再逐步细化动作；自条件和上下文扰动增强对跨尺度预测误差的稳健性。生成动作随后被重定向到真实人形机器人执行。广泛的定性和定量实验验证了方法有效性。

### 4. 带重嵌入网络的两阶段多视图步态识别

**原标题：** Two-Stage Multi-View Gait Recognition with a Re-Embedding Network<br>
**作者：** Long Hoang Le, Trung Thanh Ngo<br>
**主题：** 步态识别、多视图、重嵌入<br>
**arXiv：** [2609.32244](https://arxiv.org/abs/2609.32244)

**摘要翻译：** 单阶段步态识别容易严重过拟合且受固定视角约束。本文提出“先转换、再推理”的两阶段框架 TFTR。第一阶段用带三元组损失的浅层孪生卷积网络，将步态能量图映射到 128 维视角特定嵌入；第二阶段把各视角嵌入作为 token，交给 12 层 Transformer 编码器重新投影到余弦可分性更强的空间。推理时可灵活融合任意数量视角，突破既有方法的固定输入限制。模型在含 6,000 名受试者的 OU-MVLP 上训练，并在未见过的 CASIA-B 正常、携包和穿外套条件下测试：OU-MVLP 单视角和三视角准确率分别为 96.91% 与 99.49%，CASIA-B 三视角准确率达到 100%。

### 5. 流中的骨架：面向人体运动预测的图结构流匹配

**原标题：** Skeletons in Flow: Graph Structured Flow Matching for Human Motion Prediction<br>
**作者：** Yixuan Wang, Brandon C. Fallin, Warren E. Dixon<br>
**主题：** 人体运动预测、骨架图、流匹配<br>
**arXiv：** [2609.32231](https://arxiv.org/abs/2609.32231)

**摘要翻译：** 人体运动预测需要产生多样未来轨迹，同时与已观察运动和人体关节物理结构一致。骨架约束限制单帧姿态，协调运动还依赖相连关节间的空间交互和时间点间的时序交互。本文提出图结构流匹配 GSFM，通过单个条件速度场运输完整未来骨架轨迹。轨迹形成时空骨架图，空间与时间注意力按骨架关系和物理时间偏移耦合其演化。相对根关节的骨骼方向位于单位球面，切空间演化在生成中保持输入骨长。模型通过条件流匹配学习速度场，沿连接“以最后观测姿态为中心的随机轨迹”和真实未来轨迹的测地路径训练。AMASS 实验评估预测准确率、多样性校准和运动统计，并通过消融验证空间与时间消息传递的作用。在 AMASS 训练的 GSFM 无需更新或重训即可在未见的 Human3.6M 骨架上取得有竞争力表现。

### 6. 观察语义变化：差分感知的句子级手语视频时序分割

**原标题：** Seeing Semantic Shift: Difference-Aware Sentence-Level Temporal Segmentation of Sign Language Videos<br>
**作者：** Bowen Guo, Shiwei Gan, Yafeng Yin, Xiao Liu, Kuizhuang Liu, Zhiwei Jiang, Lei Xie<br>
**主题：** 手语视频、句子分割、时序差分<br>
**arXiv：** [2609.31148](https://arxiv.org/abs/2609.31148)

**摘要翻译：** 手语理解在短单句视频上已取得显著进展，但面对长连续视频性能明显下降。本文研究仅视觉的句子级手语分割 Vis-SSLS，在无字幕辅助下把连续手语视频划分为互不重叠的句子片段，为后续识别和翻译提供基础。手语句间过渡通常平滑且视觉上模糊，没有明确停顿或姿态复位，静态帧表示因此难以捕获边界处细微时间变化。作者提出差分感知框架 SignShift，显式把帧间特征变化作为句子边界线索。时间差分模块融合全帧、面部和手部信息，用帧间差分学习多尺度时间变化，既捕捉细粒度局部运动，也捕捉全局语义转换；片段数量预测模块估计句子数，以指导边界选择并减少过分割和欠分割。基准实验显示 SignShift 显著优于现有方法。

### 7. 何处、何时施加强制：用于流式化身的路由强制

**原标题：** Where and When to Force: Routed Forcing for Streaming Avatars<br>
**作者：** Zihan Su, Siwen Lu, Junhao Zhuang, Zeyue Xue, Haoyang Huang, Guanghao Li, Xiaofeng Tan, Chun Yuan, Nan Duan<br>
**主题：** 流式化身、音频驱动视频、扩散蒸馏<br>
**arXiv：** [2609.30963](https://arxiv.org/abs/2609.30963)

**摘要翻译：** 音频驱动流式化身需要实时合成与语音同步、动态且多样的视频。Self Forcing 用分布匹配蒸馏 DMD 把双向视频扩散模型压缩为因果少步生成器，但 DMD 最小化反向 KL 散度，天然偏向寻找模式，导致学生丢弃高动态模式、坍缩到静态输出，压缩动作动态性与多样性。作者发现坍缩具有区域差异：姿态和手势变化所在人物区域损失最大，音频驱动嘴部较小，背景基本稳定。基于此，Routed Forcing 按语义区域和噪声阶段路由蒸馏目标。空间上，对坍缩严重的人物区域采用真实视频监督的数据强制蒸馏 DFD，嘴部和背景仍用 DMD 保持唇音同步和场景稳定；时间上，高噪声阶段启用 DFD 注入多样动态模式，低噪声阶段用 DMD 细化细节，避免真实视频与学生输出空间差异造成模糊和伪影。实验相对 Self Forcing 将动态性最多提高 45%、多样性提高 7%–25%，同时保持画质和唇音同步。

### 8. 运动风格滑块：端点监督的人体运动扩散连续风格控制

**原标题：** Motion Style Slider: Endpoint-Supervised Continuous Style Control for Human Motion Diffusion<br>
**作者：** Chen-Chieh Liao, Yichen Peng, Yiyi Cai, Yûi Ono, Hiroki Hanaoka, Erwin Wu, Hideki Koike, Shuichi Kurabayashi<br>
**主题：** 人体运动扩散、风格迁移、连续控制<br>
**arXiv：** [2609.30795](https://arxiv.org/abs/2609.30795)

**摘要翻译：** 现有人体运动扩散方法生成质量较高，风格迁移模型也能注入目标风格，但对风格强度的细粒度连续控制研究不足。制作中不同艺术家和导演对强度理解主观，实用需求不是统一绝对单位，而是可靠的单调控制轴。本文提出 Motion Style Slider，一种仅以端点监督、连续控制强度的运动到运动风格迁移框架。给定内容运动和风格运动，模型在学习到的运动风格嵌入空间构造风格方向，并用标量强度控制扩散生成。训练目标结合扩散去噪和潜空间强度正则，无需中间强度真值即可鼓励平滑、单调缩放。框架兼容预训练运动扩散骨干和异构风格数据集。作者还增加小规模真实采集的“过度反应”扩展，在未见目标上测试范围外强度，评估可控性、内插/外推、内容保持与运动真实性，并消融方向构造和损失设计。

### 9. ☆ Timo：驯服用于人体运动生成的多模态扩散 Transformer

**原标题：** Timo: Taming Multimodal Diffusion Transformer for Human Motion Generation<br>
**作者：** Zhao Wang, Jiangtao Hu, Jack Yu, Tao Yu<br>
**主题：** 人体运动生成、文本到运动、扩散 Transformer<br>
**arXiv：** [2609.30761](https://arxiv.org/abs/2609.30761)

**摘要翻译：** 现有人体运动生成方法多用交叉注意力注入文本语义，却忽略运动与文本 token 的双向建模，限制文本理解。将视觉生成中有效的多模态扩散 Transformer 直接用于该任务时，人体关节运动虽时间连贯、关节间相关性却较弱，结合流匹配会生成协调性差且抖动的动作。本文提出运动学感知的多模态扩散 Transformer Timo：使用完全共享的多模态注意力双向建模文本与运动，结合流匹配；用比较真实旋转及其时间变化的几何和旋转运动学监督；再采用从广泛运动学习到细致字幕对齐的两阶段课程。作者还从六个公开数据集构建含 40,025 个留出片段的基准，在统一评测器和协议下考察六个互补维度。Timo 在定量与定性评测中显著优于先进方法，在六项中的五项超过 Kimodo，平均基准分数相对提高 40.8%。论文提供项目与演示页面，但未核验到实现仓库。

### 10. ☆ OmniFabric：面向三维服装重建的连贯 UV 空间纹理合成

**原标题：** OmniFabric: Coherent UV Space Texture Synthesis for 3D Garment Reconstruction<br>
**作者：** Ding-Jiun Huang, Yuanhao Wang, Cheng Zhang, Hugo Bertiche, Alexandru-Eugen Ichim, Thabo Beeler, Fernando De la Torre<br>
**主题：** 三维服装、UV 纹理、重光照资产<br>
**arXiv：** [2609.30234](https://arxiv.org/abs/2609.30234)

**摘要翻译：** 从单张图像自动生成可直接用于制作的三维服装资产是数字内容创作中的核心挑战。生成模型已显著推进三维几何重建，但高质量纹理仍是瓶颈：现有方法常把环境光照和阴影烘焙进纹理，或无法保持全局结构一致，使资产不适合物理模拟与重光照。本文提出 OmniFabric，直接在二维缝纫纸样空间合成全局连贯纹理。给定参考图像，流水线利用估计三维网格和强视觉语言模型的生成先验，在展开纸样上建立完整但粗糙的纹理初始化；随后，专用扩散 Transformer 通过自动合成数据引擎训练，以三维位置特征为条件，在标准 UV 域细化纹理。这能去除畸变与烘焙伪影，提取保留原始服装设计的干净、归一化纹理。大量实验显示 OmniFabric 明显优于先进基线，生成具有高质量纹理的照片级三维服装。当前仅核验到项目页。

### 11. ☆ Ego-Exo4D Human Meshes：面向第一/第三视角采集的四维人体运动重建数据集

**原标题：** Ego-Exo4D Human Meshes Dataset: 4D Human Motion Reconstruction for Ego-Exo Captures<br>
**作者：** Abhiram Maddukuri, Georgios Pavlakos<br>
**主题：** 四维人体运动、人体网格、第一与第三视角<br>
**arXiv：** [2609.30187](https://arxiv.org/abs/2609.30187)

**摘要翻译：** Ego-Exo4D 是提供同步第一视角和多视图第三视角视频的大规模数据集，可用于技能学习与评估、程序性活动理解和具身智能。然而，它只附带稀疏三维人体姿态标注，从多视图采集中恢复稠密人体运动并不容易。本文提出 Ego-Exo4D-HM，为 Ego-Exo4D 采集提供大规模四维人体运动重建，并发布配套重建流水线。论文给出包含代码、数据和文档的项目网站；核验时未能确认独立公开实现仓库，因此标为 ☆。

### 12. ☆ PHOSA：照片级真实三维手语化身建模与基准

**原标题：** PHOSA: Photorealistic 3D Sign Avatar Modeling and Benchmark<br>
**作者：** Haodong Wang, Hezhen Hu, Wengang Zhou, Houqiang Li<br>
**主题：** 手语化身、SMPL-X、多视图数据集<br>
**arXiv：** [2609.29292](https://arxiv.org/abs/2609.29292)

**摘要翻译：** 照片级真实手语化身对于与聋人群体有效交流十分重要，其难点是复杂手势和细微面部表情。本文提出与聋人专家共同设计的首个多视图中国手语数据集 MVSign，包含多样手势和丰富标注。为获得精确 SMPL-X 标注，作者开发混合拟合流水线，产生准确的身体、手部和面部参数，并可用于单目场景。基于 MVSign，论文提出解耦式手语化身表示，将身体、头部和手部分离以捕捉复杂关节动作，并设计运动感知采样以处理运动模糊、平衡手势多样性。实验表明，该方法在 MVSign 上获得高保真视觉效果，尤其能还原细致手部和面部区域，并可泛化到野外单目手语视频。论文仅提供项目页，未核验到实现仓库。

### 13. DrGait：生物力学约束的可解释临床步态视觉推理

**原标题：** DrGait: Biomechanically Grounded Visual Reasoning for Interpretable Clinical Gait Analysis<br>
**作者：** Xiangyu Yin, Shiqi Wang, Abrar Alamri, Yasir Aljohani, Weichen Liu, Goeran Fiedler, Wei Gao<br>
**主题：** 临床步态、生物力学、视觉语言模型<br>
**arXiv：** [2609.28796](https://arxiv.org/abs/2609.28796)

**摘要翻译：** 临床自动步态分析通常依赖不可解释的黑盒分类器。视觉语言模型推理能力强，但直接分析步态视频时难以测量原始视觉上下文中的细微几何偏差，容易产生幻觉。本文提出无需训练的智能体框架 DrGait，把视觉语言模型从直接视觉推理器转变为临床规划器。其“分诊—验证—综合”流程将语义推理与几何感知解耦：给定视频和基础时空指标，智能体先用启发式分诊提出诊断假设，再自主调用确定性生物力学工具，在重建的三维网格轨迹、分割的二维姿态轨迹和事件中心视频证据上验证；闭环机制根据反馈递归更新推理上下文。把模型推理锚定在可验证几何与时间测量上可减少幻觉，在获得有竞争力诊断准确率的同时生成透明、可审计的临床报告。

### 14. 视觉质量何时产生误导：渲染化身失真下的意图识别

**原标题：** When Visual Quality Misleads: Intent Recognition under Rendered Avatar Distortions<br>
**作者：** Ning-Hsuan Chang, Kai-Siang Ma, Yu-Chih Chen<br>
**主题：** 三维化身、动作意图识别、视频质量<br>
**arXiv：** [2609.27560](https://arxiv.org/abs/2609.27560)

**摘要翻译：** 化身流媒体通常用图像和视频质量指标评估，隐含地把视觉保真度当作交流成功的代理。本文通过受控行为研究检验该假设，比较无失真条件与十四种几何、光度、时间及组合失真下的三维渲染化身。59 名参与者给出 2,688 次动作感知、响应置信度和视觉质量判断。作者把感知质量高于平均、但动作识别准确率低于平均的渲染定义为“误导性质量”，并构造结合识别正确性和置信度的意图质量分数 IQS，作为客观指标的行为目标。126 个内容—条件单元中有 31 个（24.6%）出现误导性质量；时间和几何失真的比例最高，分别为 50.0% 和 31.1%。不同失真族对外观和交流的影响不同，揭示质量与准确率脱钩。在 24 个直接评分质量指标和三个监督特征回归基线中，与 IQS 的一致性仍有限；λ=0.5 时，最佳留一内容基线 PLCC 为 0.4435。结果说明视觉保真度不足以衡量化身交流，需要面向意图的质量评估与流媒体目标。

### 15. 视觉语言模型能否分析人体中心视频？模型能力与人机协作流程图谱

**原标题：** Can Vision-Language Models Analyze Human-Centered Video? Mapping Model Capabilities and Human-AI Collaborative Workflows<br>
**作者：** Xiyuan Shen, Jiuyang Lyu, Seokhyun Hwang, Huanfen Yao, Shwetak Patel, Zhihan Zhang, Jacob O. Wobbrock<br>
**主题：** 人体行为视频、视觉语言模型、人机协作<br>
**arXiv：** [2609.27327](https://arxiv.org/abs/2609.27327)

**摘要翻译：** 视频记录人体行为、交互和情境，是理解人和开展人体中心研究的重要证据。视觉语言模型日益具备视频分析能力，有望自动化这一原本高度依赖人的过程，但何时可独立分析、何时仍需人工参与尚不清楚。作者系统分析 CHI 2026 的全部 1,702 篇长文，找出 125 篇进行视频标注的论文，并通过迭代编码形成涵盖分析目的、视角、现象、推理需求与标注权威的五维分类体系。基于其中反复出现的任务，论文从开放数据集构建 15 项代表性基准，刻画通用视觉语言模型的能力和限制。研究比较模型单独、人工单独、人工验证模型输出三种流程。模型单独标注平均接近人类准确率（HNS=97.0，以人工单独为 100）；人工验证模型输出准确率最高（HNS=121.5），且相对纯人工把标注时间降低 48.9%、成本降低 31.3%–44.5%。结果连接了真实人体中心视频任务与当前模型能力，并阐明可靠高效的人机协作方式。

### 16. Heartian：生理感知的可重光照高斯头部化身

**原标题：** Heartian: Physiology-Aware Relightable Gaussian Head Avatar<br>
**作者：** Xiaoyue Fan, Jose Echevarria, Akshay Paruchuri, Kaan Akşit<br>
**主题：** 可重光照头部化身、远程光电容积描记、生理信号<br>
**arXiv：** [2609.28539](https://arxiv.org/abs/2609.28539)

**摘要翻译：** 高斯头部化身通常把内在面部外观视为时间静态，忽略心搏引起的细微肤色变化。本文提出生理感知调制框架 Heartian，在可重光照头部化身中学习面部皮肤区域高斯随心动周期变化的逐帧反照率调制，以编码远程光电容积描记 rPPG 信号。借助同步接触式 PPG 监督，Heartian 把指定心动波形建模为两个高斯函数之和，并用轻量 MLP 学习逐帧空间残差。在 UBFC-rPPG、PURE 和 MMPD 的 152 段静态记录上，属性空间恢复输入信号的汇总记录级心率 MAE 为 0.29 bpm、MAPE 为 0.38%。渲染后信号仍可被基准 rPPG 方法检测；最佳配置是在 UBFC-rPPG 预训练、加入运动增强的 TS-CAN 解码器，在渲染 MMPD 化身上获得 0.97 bpm MAE 和 1.21% MAPE。重建质量与基线相当，平均 PSNR 仅下降 0.005 dB。该方法把可恢复 rPPG 信号作为可控材质属性嵌入特定人物的高斯头部化身。

### 17. 面向人体运动预测的潜空间数据集蒸馏

**原标题：** Latent Dataset Distillation for Human Motion Prediction<br>
**作者：** Ge Tian, Guang Li, Takahiro Ogawa, Miki Haseyama<br>
**主题：** 人体运动预测、数据集蒸馏、运动先验<br>
**arXiv：** [2609.26430](https://arxiv.org/abs/2609.26430)

**摘要翻译：** 数据集蒸馏把大型训练集压缩成紧凑合成集，同时保留下游训练效用；它已广泛用于图像并扩展到时间序列预测，但在人体运动预测中仍少有研究。人体运动高维且结构耦合，在原始运动空间进行梯度匹配会优化大量相关变量，又缺少姿态合理性和时间动力学先验，因而经常产生不可信、不稳定的合成运动。本文提出用学习运动先验正则蒸馏的潜空间框架。运动先经残差量化变分自编码器 RVQ-VAE 压缩，随后只通过冻结量化器和解码器更新可学习潜变量库。预训练解码器把合成动作限制在其输出空间内，残差量化则通过多个码本逐步细化潜近似，缓解单阶段向量量化瓶颈。在 Human3.6M、CMU 和 3DPW 上，结合两个预测骨干，方法在 30 个设置中的 27 个优于直接梯度匹配，并在全部设置优于随机子集；定性结果也显示合成运动更可信。

### 18. ☆ 身份门控无人机手势控制的部署研究

**原标题：** A Deployment Study of Identity-Gated Drone Gesture Control<br>
**作者：** Diyari Mohammed Salih, Ilyes Chaabeni, Naima Ait Oufroukh<br>
**主题：** 手势识别、身份验证、人机交互<br>
**arXiv：** [2609.25511](https://arxiv.org/abs/2609.25511)

**摘要翻译：** 视觉手势控制会接受相机视场内任意手的命令，在共享室内空间不安全。本文提出 IGate，把手势控制和人脸跟踪结合，只有确认已登记操作者身份后才接受命令。系统用最初 20 帧人脸进行少样本注册，无需事先针对用户训练；验证时以余弦相似度比较当前人脸裁剪的嵌入与登记模板，人脸跟踪采用比例校正。手势控制使用自建数据集训练的 RBF-SVM 对提取的手部标志分类，层次有限状态机处理模式选择、默认和回退行为。系统部署于 DJI Tello EDU，各组件经过离线与飞行测试，共 270 次试验，其中 149 次实际飞行。人脸验证离线等错误率为 0.32%，飞行中为 19.3%；在锁定悬停条件下，RBF-SVM 的手势准确率 0.850，高于几何规则的 0.651，其中 82% 的差距来自深度通道。作者承诺发布全部日志和复现脚本，当前尚未提供可核验仓库。

### 19. ☆ STA-TFM：跨视角时空聚合 Transformer 姿态估计

**原标题：** STA-TFM: Spatio-Temporal Aggregation Across Views TransForMer for Pose Estimation<br>
**作者：** Mena Kamel, Natalie Won, Amrut Sarangi, Sven Jager, Albert Pla Planas<br>
**主题：** 多视图三维人体姿态、时空聚合、Transformer<br>
**arXiv：** [2609.24482](https://arxiv.org/abs/2609.24482)

**摘要翻译：** 单目三维人体姿态估计受深度歧义、遮挡和时间一致性影响；多视图方法更准确，但常需复杂设置。本文提出 STA-TFM，以 Transformer 融合多视图空间与时间信息。DSTformer 作为单目特征提取器捕捉每个视角中的长程姿态依赖，融合 Transformer 再跨视角聚合，输出连贯三维估计。为缓解训练数据不足，作者设计数据生成流水线，可用可控参数把任意现有三维姿态数据集转换为多视图设置。实验显示 STA-TFM 优于无需相机参数的现有多视图方法：在 DHP19 上 MPJPE 与 MPJVE 分别降低 50.9% 和 49.5%，在 HAA4D 上分别降低 6.7% 和 7.7%，在 TotalCapture 上 MPJPE 降低 15.2%。它还能处理有噪或缺失的二维输入，适用于健康监测、运动评估和沉浸式技术。论文称代码、检查点和数据已上传 Zenodo，但本次未核验其实际实现内容。

### 20. ★ 利用视觉 Transformer 在相机空间精确估计手部姿态

**原标题：** Estimating Accurate Hand Pose in Camera Space with Vision Transformer<br>
**作者：** Kaiwen Ren, Yiran Jiang, Yongjing Ye, Shihong Xia<br>
**主题：** 三维手部姿态、相机坐标、视觉 Transformer<br>
**arXiv：** [2609.24424](https://arxiv.org/abs/2609.24424)

**摘要翻译：** 基于单目 RGB 的手部姿态估计是计算机视觉的重要前沿。局部方法预测相对手腕的姿态，全局方法还需估计手腕在相机坐标系中的位置，因此面临单目深度歧义，以及透视投影中局部手姿态与全局手腕位置耦合两项根本挑战；投影由局部姿态、手腕位置和相机内参共同决定。本文在主流编码器—解码器架构中引入两项创新：用变换同构监督提取手部深度信息，用透视信息嵌入解除局部姿态与手腕位置耦合；另提出感知帧率的多数据集训练策略，细化序列姿态。完整方法在 HO3D 的相机空间平均关节误差 CS-MJE 上相对先进方法最高提升 37.1%。公开 GitHub 仓库包含模型包、脚本、测试和检查点。

### 21. DiaSeg：从 DTW 路径提取对角片段以实现可解释步态分析

**原标题：** DiaSeg: Diagonal Segment Extraction from DTW Paths for Interpretable Gait Analysis<br>
**作者：** Tresor Y. Koffi, Amel Hidouri, Corentin Legrand, Aurélie Bertaux<br>
**主题：** 步态分析、动态时间规整、临床解释<br>
**arXiv：** [2609.24223](https://arxiv.org/abs/2609.24223)

**摘要翻译：** 动态时间规整 DTW 是时间序列相似度的主流方法，但标准做法算出单一距离后丢弃最佳规整路径，损失对临床诊断最有价值的局部对齐信息。本文提出 DiaSeg，从允许受控中断的 DTW 路径提取对角片段，并以有效长度、中断次数、代价变化、时间位置和路径上下文五个几何特征描述每个片段，无需领域特征工程即可发现无监督模式。在健康老化、帕金森病、亨廷顿病、肌萎缩侧索硬化、脑肿瘤和卒中六类临床状况的 91 名受试者上，片段形成与生物力学阶段标注一致的稳定无监督模式（轮廓系数 0.33），标签验证对健康与病理步态几乎完全分离（ARI 最高 0.986）。片段以 69% 的监督准确率和 75% 的患者级聚类准确率区分病理，病理表现为片段长度分布变化；结合片段与步态周期特征后分类达到 91.7%。周期方法准确率更高（91%），但对角片段能定位步态周期内协调失效位置，提供全局表示不具备的阶段级解释。

### 22. 面向安全人车交互的轻量行人头部朝向识别网络

**原标题：** Lightweight Pedestrian Head-Orientation Recognition Network for Safe Pedestrian-Vehicle Interaction<br>
**作者：** Yuanzhe Li, Yidi Huang, Xiaotong Chang, Hounian Liu<br>
**主题：** 行人头部朝向、过街意图、人车交互<br>
**arXiv：** [2609.24193](https://arxiv.org/abs/2609.24193)

**摘要翻译：** 行人头部朝向能反映其注意力并辅助预测过街行为，对自动驾驶很重要；但真实交通场景中头部区域常分辨率很低，可靠识别仍有困难。本文提出轻量低分辨率头部朝向卷积网络 LRHO-CNN。作者从多个公开数据集提取行人头部图像，人工标注为八个方向类别，并系统预处理和增强，以增加数据多样性、覆盖光照和图像质量变化。实验把 LRHO-CNN 与微调的 ResNet-18、ResNet-34 和 VGG-16 比较，前者取得最高分类准确率。在 JAAD 和 PIE 上的进一步评估也表明，它可在真实交通场景有效识别头部朝向，为下游行人行为和意图预测提供信息线索。

### 23. 具有语义自适应运动—光照响应的可重光照三维化身重建

**原标题：** Relightable 3D Avatar Reconstruction with Semantic-Adaptive Motion-Illumination Responses<br>
**作者：** Jiankuo Zhao, Xiangyu Zhu, Jijie Li, Baiqin Wang, Shukai Chen, Zhen Lei<br>
**主题：** 可重光照头部化身、高斯表示、语义材质响应<br>
**arXiv：** [2609.24158](https://arxiv.org/abs/2609.24158)

**摘要翻译：** 从单目视频重建富表现力且可重光照的三维头部化身，需要同时准确建模非刚性面部运动和依赖光照的外观。现有高斯化身常使用全局耦合表示，让所有高斯共享统一运动或光照响应，忽视不同面部语义区域的运动模式、材质和反射属性差异，限制细粒度动画精度和重光照可信度。本文提出语义自适应运动—光照响应高斯化身框架 SAMIRA。运动响应模块把当前到参考网格的位移栅格化到拓扑一致的 UV 空间，再依据面部语义将位移特征路由到区域专用调制器，预测粗网格绑定之外的局部高斯几何残差。光照响应模块为各面部区域学习紧凑的漫反射与镜面响应因子，使不同区域高斯适应新环境光；这些因子纳入延迟式物理着色，轻量近似依赖语义的光照效应。自重演、跨主体重演与重光照实验表明，SAMIRA 比现有方法更好地重建细微表情并提升重光照真实感。

## 筛选说明

- 最终纳入 23 篇，按首次提交时间去重并复核日期；排除了以道路多智能体活动或机器人动力学执行为主要贡献、人体中心视觉关联不足的候选，以及相机/物体姿态任务。
- 本周光照相关工作包括 SAMIRA 和 Heartian 两项可重光照头部化身研究；未发现以通用场景光照方向或环境光照估计为主要任务的论文。OmniFabric 通过去除烘焙光照生成可重光照服装资产，也作为邻近工作纳入。
- ★ 核验依据：[CS-ViT](https://github.com/Mine268/CS-ViT) 仓库含模型代码、脚本、测试与检查点；[CHASE](https://github.com/Necolizer/CHASE) 仓库含期刊版本实现目录、配置及运行说明。
- ☆ 核验依据：Timo、OmniFabric、PHOSA 目前仅核验到项目/演示页；Ego-Exo4D-HM 声称发布重建代码但本次未确认独立实现仓库；IGate 仅承诺未来发布日志与复现脚本；STA-TFM 声称在 Zenodo 发布代码、检查点和数据，但本次未核验归档中的实际实现内容。
