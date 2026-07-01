# AI Governance 论文总结

## 1. How Adaptable Are American Workers to AI-Induced Job Displacement?
**作者：** Sam J. Manning, Tomás Aguirre (GovAI, NBER Working Paper 34705, Jan 2026)

构建了一个职业层面的adaptive capacity index（适应能力指数），衡量工人在被AI替代后应对job transition的能力。指数包含四个维度：净流动财富、增长加权技能可转移性、地理密度、年龄（55+比例）。覆盖356个职业，代表美国95.9%的劳动力。

核心发现：AI exposure和adaptive capacity正相关（r=0.502）。高exposure职业中，2650万工人同时拥有较高的适应能力（主要是专业和管理岗位），但610万工人（占样本4.2%）处于高exposure低adaptive capacity的困境，集中在文秘和行政岗位。地理上，这些脆弱岗位集中在大学城和州府。

关键局限：exposure不等于displacement。该指标使用Eloundou et al. (2024)的方法，衡量的是"AI能不能做这个任务"，而非"企业会不会替掉做这个任务的人"。无法区分displacement和augmentation。

## 2. Understanding AI's Labor Market Impacts (FAI Policy Brief)
**作者：** Sam Manning (Foundation for American Innovation, Dec 2025)

政策简报，提出美国劳工部（DOL）应建立AI Workforce Research Hub的四部分方案：
1. 与AI开发商（OpenAI、Anthropic、Google等）建立数据共享合作
2. 与薪资/招聘平台（ADP、LinkedIn、Revelio Labs）合作获取实时劳动力市场数据
3. 增强联邦调查（CPS增加AI补充问卷、AIES、BTOS）
4. 建立自愿性专家委员会进行季度分析

核心论点：现有联邦数据基础设施无法追踪AI对劳动力市场的影响速度，需要公私合作的新数据渠道。

## 3. Delays to Frontier AI in the EU and UK
**作者：** Lidiard, Vereschak, Gibbs, Anderljung (GovAI Technical Report, June 2026)

建立了375个LLM发布的数据集（2018年6月至2026年5月），追踪Meta、Google、OpenAI、Anthropic四家公司在EU和UK的发布延迟情况。

核心发现：11%的模型在EU延迟或未发布，7%在UK。Meta最差（约26%在EU延迟），Anthropic最好（UK无延迟）。GDPR是唯一已确认的监管障碍（个人数据训练、多模态涉及的特殊类别数据、合规文档不足）；EU AI Act目前没有证据显示造成了延迟。2026年新趋势：美国出口管制（而非欧洲监管）正成为更大的障碍。

## 4. Beyond Model Governance (arXiv 2606.00047v1)
**作者：** Goemans et al. (Google DeepMind + GovAI, June 2026, Position Paper)

核心论点：仅在模型层面进行治理是不够的，因为存在大量"非模型增益"（non-model gains）。

当前三种非模型增益向量：
- 推理增益（inference gain）：测试时计算扩展
- 系统增益（systems gain）：脚手架/编排、工具调用、多agent系统
- 资产增益（asset gain）：受限数据、专业知识

未来三种向量：具身化（embodiment）、持续学习（continual learning）、扩散效应（diffusion effects）

治理替代方案：系统治理、实体治理、agent治理、云治理，以及社会韧性建设。关键信息是AI能力增长不只来自更大的模型，治理框架需要覆盖整个AI系统栈。

## 5. Labeling of AI Agent Activity in Article 50 of the EU AI Act
**作者：** Alan Chan (GovAI Research Fellow, Policy Brief, Nov 2025)

讨论EU AI Act第50条是否要求标注AI agent的在线行为（点赞、发帖、购物等）。

核心论点：
- AI agent的行为属于AI系统的"输出"（outputs），因此应被标注
- 标注可通过元数据（metadata）实现：Web请求加"AI_generated: True"字段，浏览器操作通过可检测指示器
- 标注必须可验证：真实性（谁创建的）和完整性（是否被篡改），可用数字签名实现

局限性：元数据极易被删除；文本水印在短请求上效果差；当AI生成内容成为主流时，"AI generated"标签本身变成噪音；Art. 50只要求标注是否AI生成，不要求披露是谁的AI。

附录直接起草了Code of Practice的建议条文。

## 6. How Congress Is Approaching AI's Labor Market Impacts
**作者：** GovAI Policy Brief

分析美国国会6项与AI劳动力市场影响相关的法案，梳理立法层面的政策响应方向。
