# 信源白名单 / 黑名单

这是 `ai-learning-plan` 给用户挑资料时的信源纪律。**找资料时只从白名单里挑，主动避开黑名单。** 拿不准的来源，宁可不给。

用户可以随时让你往里加/删信源——这个文件就是用来被维护的。

---

## 白名单（优先级从高到低，但以"哪个最契合当前阶段"为准）

核心理念：**有出处、第一手、作者有公信力**。以 GitHub / YouTube / X 优质博主为主，官方博客与 arXiv 兜底权威性。

### GitHub 仓库（动手 / 实现 / 代码阅读）
- 作者本人或官方维护的实现：`karpathy/nanoGPT`、`karpathy/llm.c`、`karpathy/micrograd`、`karpathy/minGPT`
- 官方框架与模型仓库：`huggingface/transformers`、`huggingface/diffusers`、`pytorch/pytorch`、`google-research/*`、`facebookresearch/*`、`openai/*`
- 高质量推断/训练工程：`ggml-org/llama.cpp`、`vllm-project/vllm`、`unslothai/unsloth`、`Dao-AILab/flash-attention`
- 经过筛选的 awesome / 论文清单（看 star 数和维护活跃度，别用陈年失修的）：如 `Hannibal046/Awesome-LLM`、`mlabonne/llm-course`
- 优质教学仓库：`rasbt/LLMs-from-scratch`(Sebastian Raschka)、`mlabonne/llm-course`

判断标准：作者可信、近期有维护、README 清楚、有实际可跑的代码或扎实的整理，而不是攒星营销。

### YouTube 频道（讲解 / 视频课 / 论文精读）
- Andrej Karpathy —— "Neural Networks: Zero to Hero" 系列，第一手、极高质量
- 3Blue1Brown —— 神经网络/数学直觉可视化
- StatQuest with Josh Starmer —— 机器学习基础，循序渐进
- DeepLearning.AI / Andrew Ng —— 系统课程
- Yannic Kilcher —— 论文精读与评论
- Umar Jamil —— 从零实现 Transformer / LLM 等，代码级深度
- Sebastian Raschka、Two Minute Papers（前沿速览，作辅助）

判断标准：作者是领域内的研究者/工程师/公认教育者，讲的是原理与实现，不是"AI 赚钱"营销号。

### X（Twitter）优质博主（前沿动态 / 作者一手解读 / 资料线索）
用于追踪最新进展、找一手解读和资料线索（顺着他们贴的链接去原始出处）：
- @karpathy (Andrej Karpathy)、@ylecun (Yann LeCun)、@AndrewYNg (Andrew Ng)
- @rasbt (Sebastian Raschka)、@lilianweng (Lilian Weng)、@giffmana (Lucas Beyer)
- @_jasonwei (Jason Wei)、@DrJimFan (Jim Fan)、@hardmaru (David Ha)
- @cwolferesearch (Cameron Wolfe)、@_philschmid (Philipp Schmid)

注意：X 上即使是优质博主，也优先顺着他们指向的**原始论文/仓库/博客**，而不是把一条推文当作终点资料。

### 官方博客 / 研究站（权威解读 / 系统文章）
- Anthropic、OpenAI、Google DeepMind、Google AI、Meta AI 的官方研究博客
- Hugging Face Blog
- Lilian Weng 的 Lil'Log (lilianweng.github.io)
- Sebastian Raschka 的 Ahead of AI / Magazine
- Distill.pub（可视化解释，虽更新少但经典）
- The Batch (DeepLearning.AI 新闻周报)

### 论文 / 一手来源
- arXiv（优先原始论文）、各会议官方页（NeurIPS/ICML/ICLR/ACL 等）
- 论文作者的官方项目主页 / 官方代码仓库

### 中文信源（B站 / 知乎 / 社区 / 课程）
中文场景的优质一手内容。原则同上：**按"人/号"白名单，不按平台**——B站、知乎本身鱼龙混杂，只认下面这些可信作者；遇到搬运优先回到原作者的官方频道。

- **B站**：
  - **跟李沐学AI**（李沐）—— 《动手学深度学习》+ 论文精读系列，一手、顶级，适合从基础到读论文。
  - **李宏毅**（台大）—— 中文机器学习/深度学习系统课的标杆，适合打基础。
  - **王木头学科学** —— 数学/ML 直觉可视化。
  - 3Blue1Brown 官方中文号。
- **知乎 / 中文博客（按作者）**：
  - **苏剑林《科学空间》(kexue.fm)** —— 一手、高质量的数学/模型推导，圈内公认。
  - **张俊林** —— NLP / 大模型方向资深研究者的专栏。
- **GitHub 中文社区 / 教程**：
  - **Datawhale (datawhalechina)** —— 开源中文教程（李宏毅课程笔记、大模型入门等），质量稳。
  - **动手学深度学习 d2l-zh** (d2l-ai/d2l-zh)。
- **系统课**：吴恩达 / DeepLearning.AI 中文、各高校公开课的官方授权版本。

### 中文动态 / 线索（谨慎·仅作线索，落到学习要回原文）
这些是新闻、二手解读或社区讨论，**适合追前沿、找论文/项目线索，但不要把它当作终点学习资料**——顺着它指向的原始论文/仓库/官方博客去拿一手内容。
- 公众号：**机器之心、量子位、PaperWeekly**（仅这几个相对可信；其余公众号默认按黑名单处理）。
- **即刻 App** 的 AI 圈 —— 从业者一手讨论，适合"看全貌"和追动态。

---

## 黑名单（不要从这些地方拿资料）

- **内容农场 / SEO 水文**：为搜索引擎堆关键词、无作者署名、无出处、互相抄的"X 详解/X 入门"站点。
- **营销号 / 蹭热点**：标题党、"一文看懂""震惊体"、卖课引流、夸大其词的公众号/博客/视频。
- **无出处的二手解读**：把别人的论文/博客洗一遍、不给原文链接、无法溯源的转述。
- **AI 批量生成的低质博客**：一眼能看出是套模板量产、没有独到信息的页面。
- **过时且失修的内容**：几年前的、且领域已大幅演进的教程（除非是讲不变的基础原理）。
- **盗传 / 侵权搬运**：把付费课程、书籍盗录重传的资源。
- **纯广告页 / 落地页**：本质是卖产品，技术内容是噱头。
- **小红书**：技术学习场景信噪比过低——卖课、"AI 搞钱"、标题党、无出处的笔记占主流，不可溯源，不作为规划资料来源。（极个别求职/体验贴可当背景参考，但不进白名单。）
- **未列入"谨慎"名单的公众号**：默认按营销号/标题党处理，不取用。

判断口诀：**问得出"作者是谁、原始出处在哪、可信吗"三连，答不上来就别给。**

---

## 给资料前的自检清单

1. 来源在白名单，或虽未列出但明显符合白名单标准（一手、有署名、作者可信）？
2. 不是黑名单那几类？
3. 链接指向**原始出处**，不是二手搬运？
4. 内容契合用户当前所在的学习阶段（不太浅也不太难）？

四项都过，再给。
