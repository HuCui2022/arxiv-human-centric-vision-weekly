# arXiv cs.CV 人体中心视觉周报（2026-10-26 至 2026-11-01）

> 来源：[arXiv cs.CV](https://arxiv.org/list/cs.CV/recent) 官方列表及论文摘要页；以首次提交日期（UTC）筛选，周范围按北京时间上一完整自然周确定。
> 范围：动作与活动理解、手势与手语、人体及手部姿态和运动、人—人及人—物交互、三维/四维人体与数字人、光照估计与重光照。
> ★ 表示已核验公开实现代码；☆ 表示论文宣称代码将发布或给出占位仓库，但实现尚不可核验。

本期共收录 **20 篇**，其中 **3 篇 ★**、**2 篇 ☆**。

## 一览

| 首次提交 | 方向 | 中文题目 | arXiv | 代码 |
|---|---|---|---|---|
| 2026-10-26 | 三维人体高斯重建 | 复杂度引导的正则化提升人体高斯泼溅的泛化能力 | [2610.35152](https://arxiv.org/abs/2610.35152) | ★ |
| 2026-10-26 | 时序动作定位 | 学习高质量伪标签以实现点监督时序动作定位 | [2610.35516](https://arxiv.org/abs/2610.35516) | ★ |
| 2026-10-26 | 三维人体网格恢复 | UT-HMR：不确定性引导的时序建模实现稳健三维人体网格恢复 | [2610.36203](https://arxiv.org/abs/2610.36203) | — |
| 2026-10-26 | 双人社会关系理解 | 用于双人关系识别的层级多模态交互推理 | [2610.36249](https://arxiv.org/abs/2610.36249) | ★ |
| 2026-10-26 | 第一视角人体行为与运动理解 | SOMA：细粒度第一视角行为和身体运动理解基准 | [2610.36384](https://arxiv.org/abs/2610.36384) | ☆ |
| 2026-10-27 | 第一视角体育动作预测 | 感知和预测动态体育：第一视角网球视频中的视觉模型时空智能 | [2610.37619](https://arxiv.org/abs/2610.37619) | — |
| 2026-10-28 | 人体运动生成 | StepControl：基于脚部接触时间表的长时程人体运动生成 | [2610.38153](https://arxiv.org/abs/2610.38153) | — |
| 2026-10-28 | 步态分析 | 基于人体剪影的步态特征用于老年人衰弱评估 | [2610.38223](https://arxiv.org/abs/2610.38223) | — |
| 2026-10-28 | 跨骨架运动生成 | ETA-Motion：通过稀疏关节学习实现高效且不依赖骨架拓扑的运动扩散 | [2610.38259](https://arxiv.org/abs/2610.38259) | — |
| 2026-10-28 | 足球动作与三维姿态 | 三维姿态能改善足球动作价值评估吗？姿态表示与学习目标的实证研究 | [2610.38308](https://arxiv.org/abs/2610.38308) | — |
| 2026-10-28 | 小样本动作识别 | GeoTRAM：用于小样本动作识别的几何感知轨迹状态建模 | [2610.38482](https://arxiv.org/abs/2610.38482) | — |
| 2026-10-28 | 三维光源生成 | LightGenBench：三维发光属性生成基准 | [2610.39038](https://arxiv.org/abs/2610.39038) | — |
| 2026-10-29 | 第一视角手—物接触预测 | EgoContact：用第一视角视频评估物理智能 | [2610.39167](https://arxiv.org/abs/2610.39167) | — |
| 2026-10-29 | 连续手语分割 | BEACON：通过起止感知的结构化解码与蒸馏实现连续手语分割 | [2610.39553](https://arxiv.org/abs/2610.39553) | — |
| 2026-10-29 | 手部接触与力估计 | TactoHand：从视频学习基于几何的稠密手部表面交互场 | [2610.39585](https://arxiv.org/abs/2610.39585) | ☆ |
| 2026-10-29 | 视频步态评估 | 视频步态评估中的置信度过滤：测量误差与样本选择偏移 | [2610.39704](https://arxiv.org/abs/2610.39704) | — |
| 2026-10-29 | 人体跟踪与机器人安全 | 用于自主机器人导航的单目 RGB 人体跟踪：决策级误差归因与深度感知安全评估 | [2610.40199](https://arxiv.org/abs/2610.40199) | — |
| 2026-10-29 | 婴儿姿态与形状估计 | InfantNet：用于婴儿身体姿态与形状估计的大规模数据集 | [2610.40467](https://arxiv.org/abs/2610.40467) | — |
| 2026-10-29 | 人物分割与跟踪 | AVPS-360：发声人物实例分割与跟踪的空间视听基准 | [2610.40480](https://arxiv.org/abs/2610.40480) | — |
| 2026-10-29 | 长时程动作预期 | SymAnt：以可调整的符号先验为长时程动作预期提供依据 | [2610.40632](https://arxiv.org/abs/2610.40632) | — |

## 论文详情

### 1. 复杂度引导的正则化提升人体高斯泼溅的泛化能力

- 原题：Complexity-guided Regularization for Generalizable Human Gaussian Splatting
- 作者：Gun Ryu , Gi-Mun Um , Won-Sik Cheong , Wonjun Kim
- 方向：三维人体高斯重建
- 首次提交：2026-10-26
- arXiv：[https://arxiv.org/abs/2610.35152](https://arxiv.org/abs/2610.35152)

**完整摘要译文：**近期可泛化人体高斯泼溅已能根据多视角图像为未见人物合成新视角，但对几何和纹理复杂的细节仍难以表现。此前方法不限制高斯点的放置密度，复杂区域往往渲染模糊。本文提出复杂度引导的正则化，以穿着衣物的人体几何与纹理特征的局部熵计算复杂度先验，避免在复杂区域过于稀疏地放置高斯点，从而忠实重建精细结构。模型还依此先验优先从复杂区域采样局部图块，让细节获得充分监督。基准实验显示，该方法在保持实时推理速度的同时达到最先进的可泛化人体高斯泼溅性能。作者已公开代码与模型。

### 2. 学习高质量伪标签以实现点监督时序动作定位

- 原题：Learning High-Quality Pseudo-Labels for Point-Supervised Temporal Action Localization
- 作者：Zhenying Fang
- 方向：时序动作定位
- 首次提交：2026-10-26
- arXiv：[https://arxiv.org/abs/2610.35516](https://arxiv.org/abs/2610.35516)

**完整摘要译文：**点监督时序动作定位仅凭点级标注识别并定位未剪辑视频中的动作实例。现有伪标签方法虽有进展，按置信度初始化却可能遗漏定位准确的候选；训练中固定伪标签，或更新时未充分利用原始候选池的其他边界证据，都会降低监督质量。本文提出结合先验引导初始化（PGI）与训练期间共识引导细化（CGR）的框架。PGI 将候选置信度与由标注点得出的先验结合，为每个实例的初始伪标签选择和候选保留建立可靠性分数。CGR 持续利用保留的原始候选构建边界目标，将候选共识与检测器不断变化的预测结合，在整个训练过程中细化伪标签。四个基准上的检测表现具有竞争力；在 THUMOS14 上，tIoU 0.1–0.7 的平均 mAP 为 68.5%，比 PseR 高 3.7 个百分点。

### 3. UT-HMR：不确定性引导的时序建模实现稳健三维人体网格恢复

- 原题：UT-HMR: Uncertainty-Guided Temporal Modeling for Robust 3D Human Mesh Recovery
- 作者：Zhibo Wang , Sirisha Rambhatla , Yuhao Chen , Maria Koshkina , David Clausi
- 方向：三维人体网格恢复
- 首次提交：2026-10-26
- arXiv：[https://arxiv.org/abs/2610.36203](https://arxiv.org/abs/2610.36203)

**完整摘要译文：**远距离拍摄、遮挡及运动模糊造成的弱观测，使单目三维人体网格恢复不可靠；在体育场景中，不同三维姿态还可能产生相似二维投影。无需人物裁剪或外部二维线索、直接从全图恢复网格的单阶段方法尤其容易受此歧义影响。UT-HMR 据作者所知首次在单阶段框架中建模跨关节相关的姿态不确定性。每个人物查询预测完整 SMPL 姿态的高斯分布，使用紧凑的低秩加对角协方差，将其转为逐关节精度权重用于异方差监督，同时保持确定性推理。时间早期融合在姿态解码前加入邻帧证据，帮助消除不确定性所反映的歧义。使用轻量 ViT-B 主干，UT-HMR 在冰球 VIP-HockeyPose-v2 和足球 WorldPose 上达到最先进水平，MPJPE、PA-MPJPE、PVE 分别最多降低 4.7%、3.8%、5.6%；与更大主干和更高输入分辨率的方法相比，在 3DPW 上仍具有竞争力。

### 4. 用于双人关系识别的层级多模态交互推理

- 原题：Hierarchical Multimodal Interaction Reasoning for Dyadic Relationship Recognition
- 作者：Wang Tang , Fethiye Irmak Dogan , Linbo Qing , Ce Zhu , Hatice Gunes
- 方向：双人社会关系理解
- 首次提交：2026-10-26
- arXiv：[https://arxiv.org/abs/2610.36249](https://arxiv.org/abs/2610.36249)

**完整摘要译文：**双人关系识别根据两人的多模态互动判断潜在社会关系。现有方法通常把异质线索投射到共同表示并用平坦分类目标优化，忽略不同关系依赖不同的交互模式：较疏远的关系可能由直接行为对应揭示，亲密关系则更多体现为情感、行为和跨模态反应的协调。HiRe-DRR 从特征层、交互类型和关系层级组织证据，将面部、身体、声音和文本线索拆成低层与高层表示，并构建两人之间的同质和异质交互。其混合交互 Transformer（MoI-Former）把交互视作专门专家，用感知关系的稀疏路由识别相关证据，同时保留上下文。层级条件损失以由粗到细的监督利用关系层级。三个双人关系基准上的实验优于近期图像、视频及多模态方法；路由分析发现，疏远关系更依赖低层同质交互，亲密关系更依赖高层异质交互。

### 5. SOMA：细粒度第一视角行为和身体运动理解基准

- 原题：SOMA: A Benchmark for Fine-Grained Egocentric Behavior and Body-Motion Understanding
- 作者：Matea Tashkovska , Naël Ouerghemi , Haozhe Qi , Alexander Mathis
- 方向：第一视角人体行为与运动理解
- 首次提交：2026-10-26
- arXiv：[https://arxiv.org/abs/2610.36384](https://arxiv.org/abs/2610.36384)

**完整摘要译文：**理解人体运动对辅助人的多模态系统至关重要，但现有多模态大语言模型评测多关注物体、场景和粗粒度动作，对身体本身的推理评估不足。第一视角尤其困难，因为身体只部分可见，运动线索可能被遮挡或分散在时间上。SOMA 提出含 1,632 道人工核验问题的基准，覆盖身体构型、运动动力学和时间推理三项能力。作者评估 37 个领先的闭源、开源及第一视角专用模型，并进行了广泛的人类评测。人类仅凭视频也觉得任务困难（准确率 68.5%），却明显超过最强模型 Qwen3.6-27B 的零样本 50.0%。错误分析显示，模型常误读佩戴者自身身体、误判事件时间，并偏向右手或低估重复次数。作者另提出视频、身体运动与语言对齐的训练数据及联合学习三种模态的基线，以缩小差距；基准、训练数据和代码计划公开。

### 6. 感知和预测动态体育：第一视角网球视频中的视觉模型时空智能

- 原题：Perceiving and Predicting Dynamic Sports: Spatiotemporal Intelligence in Vision Models for Egocentric Tennis Video
- 作者：Tudor Braicu , Joseph DelPreto , Jared Boyer , Mónika Farsang , Maximilian Stölzle , Tim Niklas Seyde , Daniela Rus
- 方向：第一视角体育动作预测
- 首次提交：2026-10-27
- arXiv：[https://arxiv.org/abs/2610.37619](https://arxiv.org/abs/2610.37619)

**完整摘要译文：**敏捷机器人需要理解场景、推理交互和预期未来事件的时空能力，但基础视觉模型在运动的第一视角相机下表现如何尚不清楚。作者采集带标注的网球数据集，同步记录第一视角及五个外部视角视频、估计的全局位置、触球时刻和击球类型，并训练视觉模型执行七项预测任务：第一视角球员二维定位、网球三维定位、双方未来轨迹、正手或反手预期、距下次触球的时间及触球时网球三维位置。比较图像、视频编码器与视觉语言模型的联合训练预测头后，最佳模型当前帧球员和球定位平均误差分别为 0.14 与 0.54 米；未来 1.1 秒球员和球轨迹误差为 0.34 与 0.91 米；触球时间误差 0.14 秒。辅助深度明显改善三维球定位，说明公制深度仍难推断；更长图像历史未改善球轨迹预测，表明表示更多利用场景上下文而非仅帧间运动。作者最后提出条件扩散模型，从第一视角视频的视觉预测以实时速度生成全身网球运动学动作，并随预测改善调整动作。

### 7. StepControl：基于脚部接触时间表的长时程人体运动生成

- 原题：StepControl: Long-Horizon Human Motion Generation from Foot-Contact Schedules
- 作者：Hojun Jang , Jinseok Bae , Donggeun Lim , Taesun Kim , Seungbin Jeong , Younghwan Lee , Yong Seok Kim , Young Min Kim
- 方向：人体运动生成
- 首次提交：2026-10-28
- arXiv：[https://arxiv.org/abs/2610.38153](https://arxiv.org/abs/2610.38153)

**完整摘要译文：**可控人体运动生成通常指定发生何种动作或身体移动到哪里。本文探讨仅指定左右脚何时接地，能否控制全身运动。StepControl 是以未来左右脚二值接触时间表为条件的自回归扩散模型，无需目标根部与身体姿态或语义提示。它把接触表示为显式时间事件，通过专门的交叉注意力和无分类器引导注入模型；随机混合噪声调度与预热策略使长时程自回归生成保持稳定。实验显示，相比把已有空间引导运动生成器改造成接触约束方法，StepControl 更准确遵循指定接触时序，在长时间连续生成中保持有效控制，并响应步频变化、走走停停、跛行和双脚跳跃等编辑。结果证明，简洁的脚部接触时间表可作为直观有效的时间控制接口。

### 8. 基于人体剪影的步态特征用于老年人衰弱评估

- 原题：Silhouette-Based Gaitomics for Frailty Assessment in Older Adults
- 作者：Laura McDaniel , Ryan Roemmich , Crystal Szczesny , Peter Abadir , Rama Chellappa , Basudha Pal
- 方向：步态分析
- 首次提交：2026-10-28
- arXiv：[https://arxiv.org/abs/2610.38223](https://arxiv.org/abs/2610.38223)

**完整摘要译文：**步行可反映身体功能，也可支持可解释的视频衰弱评估。作者提出基于剪影的“步态组学”，把衰弱预测与可测量的身体构型和运动模式关联。在按 Fried 衰弱表型评估的 66 名老年人中，标准化剪影与步态能量图形成 90 项形状、时间变化、运动和纹理描述符。基于互信息差的最小冗余最大相关特征选择优先保留信息量大的特征。每种分类器在参与者层面进行外层五折、内层三折的嵌套分层交叉验证，特征排名与数量选择仅在训练分区内完成；Shapley 加性解释分析留出预测。双侧剪影差异在三分类和两项涉及衰弱者的比较中均位居总体特征排名前列；不同任务的归因不同，三分类尤其依赖纹理和连续帧剪影差异。CatBoost 三分类平均 micro-AUC 最高，为 0.647±0.085；衰弱与非衰弱、衰弱与衰弱前期、衰弱前期与非衰弱的最佳两两 micro-AUC 分别为 0.833±0.249、0.765±0.168 和 0.554±0.129。该方法把预测与明确步态特征相连，同时揭示任务依赖的特征优先级及衰弱前期与非衰弱之间有限的区分度；仍需更大规模独立研究验证可靠性和临床意义。

### 9. ETA-Motion：通过稀疏关节学习实现高效且不依赖骨架拓扑的运动扩散

- 原题：ETA-Motion: Efficient Topology-Agnostic Motion Diffusion via Sparse Joint Learning
- 作者：Seoyoung Hwang , Tae-Kyun Kim
- 方向：跨骨架运动生成
- 首次提交：2026-10-28
- arXiv：[https://arxiv.org/abs/2610.38259](https://arxiv.org/abs/2610.38259)

**完整摘要译文：**不依赖骨架拓扑的运动生成，要为任意骨架的不同角色合成动作，须处理关节配置多样和语义不一致的问题。现有方法密集建模所有关节，计算成本高，也不利于学习可迁移的运动模式。ETA-Motion 基于稀疏关节学习，用紧凑关节子集减少冗余，并在得到的稀疏骨架上训练生成器。为建立跨拓扑对应，方法以文本和视觉线索构建语义关节嵌入，辅以保持骨架结构的拓扑感知训练目标。虽然仅用稀疏观测训练，推理时仍能生成完整骨架运动。实验显示，ETA-Motion 超过现有跨拓扑基线，并明显提高效率及对未见动作和未见拓扑的泛化能力。

### 10. 三维姿态能改善足球动作价值评估吗？姿态表示与学习目标的实证研究

- 原题：Does 3D Pose Improve Action Valuation in Football? An Empirical Study of Pose Representations and Learning Objectives
- 作者：Rikuhei Umemoto , Kenjiro Ide , Soham Majumder , Ulf Brefeld , Keisuke Fujii
- 方向：足球动作与三维姿态
- 首次提交：2026-10-28
- arXiv：[https://arxiv.org/abs/2610.38308](https://arxiv.org/abs/2610.38308)

**完整摘要译文：**足球动作价值评估估计球员对未来得分的贡献。现有多智能体深度强化学习模型使用二维位置和速度，忽略与即将发生的动作相关的姿态。本文检验在基于 SARSA 的模型中加入三维姿态，能否改善与进攻回报相关的已发生动作价值：回报包括进球、失球或最终预期控球价值。作者使用 2022/23 赛季欧冠事件、追踪和三维姿态数据，在五种学习设置和三个随机种子下比较六类表示，包括无姿态、原始关节、躯干与头部朝向，以及 ST-GCN 嵌入；设置调整时序差分目标与动作预测损失，并以蒙特卡洛回报回归作参照。50 项有球与无球比较中，姿态仅在三项稳定改善回报预测，且均使用躯干和头部朝向；十二项变差，多数采用 ST-GCN。训练选择影响更大：移除动作预测损失，使仅位置的有球动作价值能力从 0.003 升至 0.040，与预期进球的相关性由 0.23 升至 0.60；同等训练长度下回报预测收益仍存在。另一方面，原始关节姿态使未来 0.2 秒有球动作预测的宏 AUC 从 0.914 升至 0.934；传球执行时的传球者姿态使传球成功预测 AUC 从 0.844 升至 0.856。在该训练协议中，姿态有助于预测即将发生的动作，却很少改善已发生动作的价值评估。

### 11. GeoTRAM：用于小样本动作识别的几何感知轨迹状态建模

- 原题：Geometry-Aware Trajectory State Modeling for Few-Shot Action Recognition
- 作者：Zhiqi Miao , Marko Haralović , Stanislav Levendeev , Sarvesh Angadi , Jannatul Ferdous , Dan-Cristian Ploesteanu , Jiapan Guo , Estefanía Talavera
- 方向：小样本动作识别
- 首次提交：2026-10-28
- arXiv：[https://arxiv.org/abs/2610.38482](https://arxiv.org/abs/2610.38482)

**完整摘要译文：**小样本动作识别需要仅从少量有标注视频中提取具有判别性的运动动态。近期轨迹方法用长期点追踪建立显式时间对应，却常只把轨迹当作视觉特征载体，或用紧凑二维位移描述符概括运动。本文将动作视为 2.5 维轨迹状态及其局部几何交互的有序演化，提出 GeoTRAM。它把稀疏追踪提升为 2.5 维轨迹，StateMotion 建模单条轨迹内有序状态演化，RelMotion 利用随时间变化的相对几何和运动捕获带状态条件的局部交互。经质量过滤的谱采样使轨迹初始化更可靠；语义、运动、深度线索分别细化并保留用于联合时空建模；动作引导的重加权和 top-ρ 轨迹选择支持帧级与轨迹级互补匹配。在五个小样本动作基准上，方法显著改善运动主导的 Something-Something 结果，在外观主导基准上也保持竞争力，并兼顾准确率与效率。

### 12. LightGenBench：三维发光属性生成基准

- 原题：LightGenBench: A Benchmark for 3D Emission Generation
- 作者：Dongchen Yang , Xingguang Yan , Manolis Savva
- 方向：三维光源生成
- 首次提交：2026-10-28
- arXiv：[https://arxiv.org/abs/2610.39038](https://arxiv.org/abs/2610.39038)

**完整摘要译文：**近期方法能生成几何精细、纹理丰富的三维资产，但多数资产只反射光而不能自行发光。本文提出发光属性生成任务：根据三维资产的几何、非发光材料及渲染视图，预测其表面空间变化的 RGB 发光分布。LightGenBench 提供三方面支持：收集 3.7 万个艺术家制作、以 UV、体素和多视角形式表示的发光资产；建立 UV 域、稀疏体素、多视角及分割式生成四类基线；设计评估资产何处发光、如何发光的协议，并以不同发光强度的渲染图开展用户研究。四类方法中，稀疏体素基线 TRELLIS.2-Emission 最好，因为原生三维发光生成避开了 UV 空间断裂伪影和多视角方法看不到被遮挡发光区域等问题。但其 IoU 仅 0.271，说明任务仍远未解决。作者希望该基准使发光生成成为可系统评测的三维生成问题。

### 13. EgoContact：用第一视角视频评估物理智能

- 原题：EgoContact: Evaluating Physical Intelligence with Egocentric Video
- 作者：Adam Deryło , Alexey Gavryushin , Daniel Cremers , Marc Pollefeys , Xi Wang
- 方向：第一视角手—物接触预测
- 首次提交：2026-10-29
- arXiv：[https://arxiv.org/abs/2610.39167](https://arxiv.org/abs/2610.39167)

**完整摘要译文：**第一视角视频是学习可泛化操控先验的可扩展数据来源，但尽管广泛用于机器人策略预训练，在检验物理智能方面仍利用不足，其中一项关键能力是判断为达成交互意图应在物体何处接触。EgoContact 提出大规模第一视角基准，通过预测未来接触点评估学习到的操控先验的泛化性与精度。数据集含 2.25 万个人工核验的交互事件，每项提供接触前观测、语义意图及像素精度的接触位置。作者发现现有方法常难以准确预测接触点，有时即使允许多次预测，也无法在多样的野外场景中定位目标物体。标注交互对机器人操控也有用：仅把 EgoContact 用作现有可供性迁移策略的记忆库，抓取成功率就从仿真的 14.2% 升至 31.2%，真实机器人上从 16% 升至 58%。

### 14. BEACON：通过起止感知的结构化解码与蒸馏实现连续手语分割

- 原题：BEACON: Distilled Begin/End-Aware Structured Decoding for Continuous Sign Language Segmentation
- 作者：Guohou Zhang , Kalin Stefanov
- 方向：连续手语分割
- 首次提交：2026-10-29
- arXiv：[https://arxiv.org/abs/2610.39553](https://arxiv.org/abs/2610.39553)

**完整摘要译文：**基于分割的连续手语识别先把未剪辑视频切成词汇单元，因此分割最终服务于下游识别；然而分割器通常按局部边界检测评判，而非按词汇片段及其支持的识别质量。BEACON 将四类 Outside/Begin/Inside/End（BIOE）标注、对八种合法转移的约束 Viterbi 解码，以及从二分类教师蒸馏到共享学生的边界知识结合起来。在严格的无剪切评估及基于验证集选模下，相对 PHOENIX-14 和 BSL Corpus 各自的最先进方法，片段 F1 分别提高 14.58 和 14.59 点，边界 F1 分别提高 2.17 和 1.22 点，下游词错误率（WER）分别降低 9.10 和 4.15 点。评估五种不同架构后，片段 F1 与较低 WER 的相关性在两个语料上均比边界 F1 更一致：Spearman ρ 分别为 -1.0/-0.9，对比 -0.9/-0.8。结果支持按片段质量及下游识别效用，而非只按局部边界准确率评估手语分割。

### 15. TactoHand：从视频学习基于几何的稠密手部表面交互场

- 原题：TactoHand: Learning Geometry-Based Dense Hand-Surface Interaction Fields from Video
- 作者：Ziheng Xi , Weibo Li , Jiayi Yu , Sipeng Zheng , Wanpeng Zhang , Haiweng Xu , Hao Luo , Chuan Mao , Zongqing Lu
- 方向：手部接触与力估计
- 首次提交：2026-10-29
- arXiv：[https://arxiv.org/abs/2610.39585](https://arxiv.org/abs/2610.39585)

**完整摘要译文：**理解人与世界的交互，需要在手部表面表示物理作用。触觉传感可捕获这些信息，但规模化采集需要专门硬件。TactoHand 从单目视频预测接触、接近程度及三维作用力三个稠密手部表面交互场。作者从约 5000 万源视频帧组成的精选集合中，利用符合条件的训练数据，推导几何接触和接近标签，以及由运动得到的力标签。模型以时序 Transformer 汇聚跨帧视觉证据，再用三个学习得到的查询解码对应的表面场；可微物理层根据观测到的物体运动约束力预测。在同域和域外基准上，接触和接近估计均优于先前方法；物理监督降低运动展开中的位置和旋转误差，预测的接触与接近场也改善下游手—物重建。结果表明，无需采集触觉测量，也能以低成本、可扩展方式学习手部表面交互场。

### 16. 视频步态评估中的置信度过滤：测量误差与样本选择偏移

- 原题：Confidence Filtering in Video-Based Gait Assessment: Measurement Error versus Selection Shift
- 作者：David Regev , Eran Beeri Bamani
- 方向：视频步态评估
- 首次提交：2026-10-29
- arXiv：[https://arxiv.org/abs/2610.39704](https://arxiv.org/abs/2610.39704)

**完整摘要译文：**视频步态评估常只保留高置信度姿态观测，这可能降低测量误差，却改变实际被评估的动作。作者在帕金森相关队列（96 人）及 NF2 相关复现队列（18 人）中，将置信度选择与相同预算的随机选择比较。帕金森相关队列的置信度选择使观测运动汇总略有但一致的偏移（+0.05 标准差，95% 置信区间 0.03–0.07），留出 Mini-BESTest 误差基本不变（-0.04 分，-0.13 至 0.05）；保持运动分组比例的策略减少偏移。NF2 队列未见偏移，且预测器未优于常数基线。由于这一影响混合测量误差与样本选择偏移，作者按队列时间窗口结构分解并模拟两者：若误差与置信度相关，过滤可降低局部误差；若置信度更多跟随运动而非误差，则会使终点指标有偏。帕金森数据中，置信度与运动仅弱相关（ρ=0.14）；若高质量窗口无偏，过滤无害；若系统误差只在参与者内部重新分布，过滤可引入最多 0.58 度误差。因此，小队列预测器临床误差不变，并不能证明质量过滤保持了原本被评估的动作。

### 17. 用于自主机器人导航的单目 RGB 人体跟踪：决策级误差归因与深度感知安全评估

- 原题：Decision-Level Error Attribution and Depth-Aware Safety Evaluation of Monocular RGB Human Tracking for Autonomous Robot Navigation
- 作者：Abdulahi Taiwo , Chijioke Cyriacus Ekechi
- 方向：人体跟踪与机器人安全
- 首次提交：2026-10-29
- arXiv：[https://arxiv.org/abs/2610.40199](https://arxiv.org/abs/2610.40199)

**完整摘要译文：**机器人在人附近运行时，单目 RGB 跟踪有用，但感知错误会影响“停止或继续”的二元决策，而几何准确率指标不足以体现这种影响。本文区分安全规则与感知各自造成的决策错误。作者证明，仅用横向距离是平面距离的下界：若位置准确，它不会漏掉平面规则发现的危险，但会造成不必要停车。方法用双因素 Shapley 归因拆分规则和感知贡献，并进一步区分漏检与定位误差。实验使用 ETH 和 UCY 行人视频、模拟静止机器人、互不重叠的校准与评估行人，以及按时间块自助采样的区间。三个场景 898 名行人中，横向规则在标注位置上未漏掉危险，但停车精确率只有 5.6%–31.9%。在两个 RGB 感知场景中，校准后的地面定位平面 RMSE 为 0.59 和 0.51 米，优于几何基线的 1.72 和 1.39 米及校准 Depth Anything V2 的 0.81 和 0.68 米。0.43 和 0.26 的检测召回率使漏检成为危险漏判的主要来源。使用地面定位和两个标准差安全裕度，在全部八种场景—阈值设置中达到或改善横向规则的漏危险率，并在其中七种减少不必要停车。全部机器人交互均为模拟，结果是离线决策分类，并非实际避撞演示。

### 18. InfantNet：用于婴儿身体姿态与形状估计的大规模数据集

- 原题：InfantNet: A Large Scale Dataset for Infant Body Pose and Shape Estimation
- 作者：Zhipeng Hui , Jiahao Wang , Xun Dong , Guofeng Zhang , Xingrui Wang , Jiawei Peng , Qihao Liu , Xiaoding Yuan , Yi Zhang , Junjie Oscar Yin , Wufei Ma , Qinfan Lyu , Sara N. Lupolt , Keeve Edward Nachman , Adam Kortylewski , Alan Yuille
- 方向：婴儿姿态与形状估计
- 首次提交：2026-10-29
- arXiv：[https://arxiv.org/abs/2610.40467](https://arxiv.org/abs/2610.40467)

**完整摘要译文：**婴儿姿态和形状估计可用于护理、发育监测和医学诊断，但现有方法及数据集主要面向成年人；由于身体比例、关节活动范围和频繁自遮挡存在显著差异，直接迁移效果不佳。InfantNet 是迄今最大的真实图像婴儿数据集，包含 6–18 个月婴儿的 108,902 张 RGB 图像，全部有二维关键点标注；精选的 11,642 张还含完整 SMIL 参数的三维姿态与形状标注，并通过多视角渲染和重投影误差过滤核验。迭代标注流程保证二维及三维标签质量。数据集建立大规模婴儿二维关键点与三维姿态形状恢复基准。基线实验显示，最先进成人姿态估计器难以泛化至婴儿，在 InfantNet 上微调则稳定改善表现；三维姿态与形状的收益更明显，基于 SMIL 的估计精度可与已报道的 SMPL 方法结果相当。作者发布数据集和基准，为婴儿姿态分析及相关健康应用提供资源。

### 19. AVPS-360：发声人物实例分割与跟踪的空间视听基准

- 原题：AVPS-360: A Spatial Audio-Visual Benchmark for Instance Segmentation and Tracking of Sound-Producing Persons
- 作者：Yifu Sun , Parthasaarathy Sudarsanam , Tuomas Virtanen , Archontis Politis
- 方向：人物分割与跟踪
- 首次提交：2026-10-29
- arXiv：[https://arxiv.org/abs/2610.40480](https://arxiv.org/abs/2610.40480)

**完整摘要译文：**视听实例分割要在视频中分割、跟踪各个发声物体。现有基准主要使用单声道音频，缺乏空间区分同时发声源的跨声道线索。AVPS-360 将视听实例分割与声音事件定位检测连接起来，基于 STARSS23 配对一阶 Ambisonics 音频及同步 360 度视频，含 230 段录制、共 10.5 小时，平均每段 164.0 秒。数据捕获现实互动中间歇出现的语音，以及笑声、拍手和脚步，提供与发声者身份及事件标签关联的 31,678 张人工审核实例掩码。作者还提出融合空间音频与视觉特征的基线，用于逐帧分割和跨帧身份关联。实验发现，已有视听实例分割方法在长时、间歇发声的录制中难以检测和关联身份，而新基线在两方面均明显改善。

### 20. SymAnt：以可调整的符号先验为长时程动作预期提供依据

- 原题：SymAnt: Grounding Long-Horizon Action Anticipation with Adaptable Symbolic Priors
- 作者：Fnu Aryan , Yaqi Xie , Joseph Campbell , Woojun Kim , Kwonjoon Lee , Hossein Nourkhiz Mahjoub , Ehsan Moradi-Pari , Katia Sycara , Simon Stepputtis
- 方向：长时程动作预期
- 首次提交：2026-10-29
- arXiv：[https://arxiv.org/abs/2610.40632](https://arxiv.org/abs/2610.40632)

**完整摘要译文：**随着机器人和智能系统越来越多地与人互动，它们需要从短暂观测预期较长的未来动作序列。纯神经模型通常需要大量观测，且难解释或调整；符号先验可提供结构化替代。SymAnt 提出神经符号方法，结合神经网络表达能力与场景图、知识图的结构推理。给定短视频，方法联合搜索两类图以构建符号上下文，统一推理空间关系、物体属性、可供性及关联动作；该上下文作为迭代细化的先验，逐步生成并改善未来动作序列。符号约束使其能以较少参数从短观测窗口预测长时程动作，用户还可直接编辑底层知识调整预测而无需再训练。在 Breakfast、50 Salads、EPIC-KITCHENS、EGTEA Gaze+ 和 Assembly101 五个数据集上，实验验证了方法有效性，短观测场景尤其明显。

## 筛选与代码核验说明

- 从官方 cs.CV 列表筛选候选，并逐篇查看摘要页的完整摘要及首次提交历史；排除首次提交于 10 月 25 日或更早、仅在本周公告或交叉列出的论文。
- 本期未发现直接估计场景光源参数的论文；纳入与光照建模相关的三维发光属性生成基准 LightGenBench。
- 未将仅发布数据集、模型权重或与论文实现无关的网站源码计为 ★。

### 已核验公开实现（★，3 篇）

- [2610.35152](https://arxiv.org/abs/2610.35152)：[仓库](https://github.com/DCVL-3D/CGR-GS_release) 含 src、config、scripts 与数据准备代码。
- [2610.35516](https://arxiv.org/abs/2610.35516)：[仓库](https://github.com/zhenyingfang/LHQP) 含 src、OpenTAD、configs 和训练脚本。
- [2610.36249](https://arxiv.org/abs/2610.36249)：[仓库](https://github.com/tw-repository/HiRe-DRR) 含 network.py、train.py 和 dataset.py。

### 代码声明或占位项目（☆，2 篇）

- [2610.36384](https://arxiv.org/abs/2610.36384)：摘要承诺公开完整基准、训练数据与代码，当前未核验到实现仓库。
- [2610.39585](https://arxiv.org/abs/2610.39585)：[仓库](https://github.com/zhenqis123/Tactohand) 当前仅有 README；摘要称代码将发布。
