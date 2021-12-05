# Transformer-101-questions
Transformer 101 interview questions

<b>
  <pre>
  
序号:  分类 : 深度等级(L0最深) : 问题描述
1 第一性,数理 L0 请阐述Transformer能够进行训练来表达和生成信息背后的数学假设，什么数学模型或者公式支持了Transformer模型的训练目标？请展示至少一个相关数学公式的具体推导过程。（贝叶斯公式、极大似然估计、KL散度、交叉熵、矩阵空间转换等）
2 第一性 L0 Transformer中的神经网络为何能够很好的表示信息？请从数学和工程实践的角度展开具体的分析
3 第一性,架构 L0 请从Data Science的角度分析为何Transformer是目前最generic的AI模型？
4 第一性 L0 请分析一下是什么能够从根本上限制Transformer的能力？
5 原理，数理 L0 Transformer在通用语言领域(例如，整个英语语言领域)能否实现Word Analogy功能，请分析具体的工程原因和数学原因
6 第一性 L0 为何说Transformer是一种理想的Bayesian模型实现？请阐述数学原理及具体的场景案例
7 第一性,Naive Bayes L0 为何说Transformer是目前人工智能领域工程落地实践Bayesian理论的典型？请从数学的的角度进行完整的证明（至少包含Encoder-Decoder、Training、Inference等对Bayesian Theory的具体实现）
8 第一性 L0 在Gavin看来，“Transformer赋予机器思想。Transformer是实现多模态目前最佳的底层引擎，是人工智能、贝叶斯理论、认知模型演进的统一架构，是学术界（无意间）基于Bayesian理论通过神经网络实现的（计算机）认知模型持续的Evolving的理想架构体系”，你怎么看？
9 数理，架构 L1 请从数学和架构的角度分析一下Transformer是如何通过使用Bayesian理论中的marginal probability来完成信息更丰富和立体的表达的？
10 架构 L1 请描述一下你认为的把self-attention复杂度从O(n2) 降低到 O(n)有效方案
11 原理,Tokenization L1 使用BPE (Byte-Pair Encoding) 进行Tokenization对于Cross-lingual语言模型的意义是什么？是否会有问题及如何改进？
12 架构 L1 如果使用Transformer对不同类别的数据进行训练，数据集有些类别的数据量很大(例如有10亿条)，而大多数类别的数据量特别小(例如可能只有100条)，此时如何训练出一个相对理想的Transformer模型来对处理不同类别的任务？
13 架构,工程,数理 L1 如何使用使用多种类小样本对Transformer训练而取得很好的分类效果，请详述背后的架构设计和数学机制
14 架构 L1 更深更宽的Transformer网络是否意味着能够获得更强的预训练模型？请至少从3个角度，例如架构的工程化落地、参数的信息表达能力、训练任务等，来展开具体的分析
15 架构 L1 为什么说Transformer的注意力机制是相对廉价的？注意力机制相对更对于RNN系列及Convolution系列算法而言在计算上（尤其是计算复杂度）有什么优势？
16 BERT,架构,数理 L1 为何训练后的BERT模型不能够很容易的实现模型泛化？请从架构机制和数学原理部分进行分析
17 架构 L1 GPT的auto-regressive语言模型架构在信息表示方面有什么架构上的缺陷？具体如何改进？
18 Decoder, 架构 L1 请描述Transformer中Decoder的Embedding layers架构设计、运行流程和数学原理
19 原理 L1 为何Transformer的Matrix Dimensions是3D的？每个Dimension大小的改变是如何影响整个Transformer训练过程的？请详述其具体的流程和数学原理
20 原理 L1 请描述Transformer的Training Loss具体工作流程和背后的数学公式
21 原理 L1 请阐述Transformer中所有能够trainable的操作及其功能
22 原理 L1 如何解决Self-attention和Word和自己的Attention最大的问题？
23 原理 L1 为什么Transformer能够对NLP、CV等具有“set of units”的任何AI领域的信息进行更加有效表示？
24 原理 L1 为何通过Ground Truth就能够训练Transformer使其具有泛化能力? 请从数学原理的角度具体分析
25 原理 L1 相比于RNN等，为何Transformer论文作者声称“Attention is all you need”？请重点从数学的角度阐述其原因
26 原理,数理 L1 请具体谈一下Teacher forcing的数学原理及其在Transformer中的至少两个地方的应用
27 Encoder/Decoder,数理 L1 在Transformer的架构中Decoder在进行Inferencer的时候同时接收来自Encoder和Decoder的输入信息，以NLP为例，这两种类型的输入在词法、语法、语义上是否有所不同？背后的数学原理是是什么？
28 原理 L1 Transformer的Input长度为何受限？请阐明数学原因并提供至少一种可能的解决方案
29 代码,Pytorch L1 如果使用Pytorch实现Transformer，如何巧妙的使用或者停用 optimizer.zero_grad()来训练大模型，例如内存只允许一次只能训练一个Instance？
30 原理 L1 请描述Transformer训练时候的Label Smoothing核心功能、运行机制和数学原理
31 工程 L1 如果由你使用Transformer来实现一个对话系统，如何判定用户当前的交流的内容是否离题，例如在办理一项业务过程中突然对话机器人今天天气怎么？请阐述架构思路及数学原理
32 原理 L1 请描述Transformer使用动态Batch Size进行训练的原理、流程和数学证明
33 原理,数理 L1 使用Transformer实现NLU的时候需要使用Masking机制吗？请解释工程原因及数学原理
34 架构,数理 L0 如何使用Transformer来实现具有上下文的多轮对话系统？尤其重点考虑对话的状态管理。请描述工程架构和数学原理
35 原理,工程 L1 请问使用手动实现Tranformer和使用BERT哪个做Intent识别效果更好？请阐述具体的原因和工程实践过程
36 原理 L1 为何Transformer比RNN、LSTM等传统神经网络具有更高性价比且能够更有效的使用内存和计算资源？
37 原理 L1 Transformer为何只使用Attention机制就解决了CNN、LSTM、RNN等能解决的一切问题及这些传统网络解决不了的问题？
38 工程 L1 如何分类语料库中的有些Label标注是错误的，如何使用Transformer来发现分类语料库中的Bad Label？请描述具体的工程过程
39 架构,数理 L1 为什么一般情况下Transformer的训练不会完全使用Bayesian模型而是更倾向于采用Naive Bayes？请具体阐述其架构和背后的数学原理
40 原理 L1 请从Bayesian模型的角度分析Transformer中代表模型例如GPT3为何是模型越宽越深越好？
41 代码,工程,LDA L1 如何使用Transformer和LDA结合完成信息的多分类模型？请实现示例代码
42 原理,算法细节 L1 Transformer 编码器-解码器模型调优层面，压缩网络结构，对编码器及解码器的前馈层进行了模型改进，去掉Residual网络模块，将正则层LayerNorm从三层网络简化为一层网络，预测效果与基线Transformer模型相差无几，那么，Transformer模型的编码器及解码器的基本网络单元究竟在训练什么？到底发挥了什么作用？什么因素是Transformer 终极的的智慧预测法门？
43 数理 L2 在给Transformer输入Embeddings的时候是否可以使用多方来源的词嵌入训练模型？请阐述背后的数学原理及工程上的具体实现机制
44 数理,工程 L2 如何大规模降低Transformer中Embedding中的参数数量？请至少具体分析一种具体方法背后的数学原理和工程实践
45 数理 L2 请描述Trasnformer不同的Layer之间的FeedForward神经网络之间的联系，例如在Bert中不同Layer之间的CLS 有什么关系、对角矩阵随着Layer的加深有何变化等
46 数理,工程 L2 Transformer的Layer深度过深，例如512个Layer，会可能导致什么现象？请详述背后的数学机制。如何降低Transformer的Feedforward层的参数数量？请详述背后的数学原理和工程实践。
47 BERT,数理 L2 Bert中NSP可能的问题有些哪些？这些问题背后的数学原理是什么？如何改进？可以去掉NSP训练任务吗？
48 数理 L2 请详解分析Transformer的Batch大小与训练的信息困惑度Perplexity的关系并阐明背后的数学原理
49 工程 L2 请从数学的角度分析一下为何在对Transformer进行参数的 Quantization的时候工业界最终选择了INT8？包括压缩的具体过程、KL散度、长尾分布等。如何处理Quantization后模型质量降低度情况？
50 数理 L2 以Transformer为代表的的Neuron Network逐渐主导了人工智能各领域，例如NLP, CV等的信息表示。请从数学的角度阐述为什么Neuron Network能够代表任意人复杂度的信息？使用神经网络表达信息具体有什么优势？
51 数理 L2 请描述至少三种判断Transformer中神经元Neuron相对重要程度的具体方法及其背后的数学原理
52 数理 L2 请用具体例子阐述使用Multi-head的物理机制和并从数学的视角来推导其有效性的原因
53 数理,工程 L2 请分享一下至少三种提升Transformer预测速度的具体的方法及其数学原理
54 BERT,原理 L2 请分别描述Bert的MLM和NSP技术(例如Sampling) 的问题及具体改进方式
55 数理 L2 请阐述使用Transformer实现Zero-shot Learning数学原理和具体实现流程
56 工程 L2 请至少描述2种对来自不同训练模型训练出来的Embeddings进行相似度比较的方法的具体实现
57 工程，数理 L2 如何使得一个小模型，例如LSTM，具有一个大模型，例如Bert的能力？转过来讲，如何使得一个通用的大模型，例如Bert，能够汇聚小模型的能力？请阐述工程实践和数学原理
58 BERT L2 请描述BERT中MLM实现中的至少5个缺陷及可能的解决方案
59 数理 L2 请从数学的角度阐明对Transformer任意位置和长度进行Masking的具体实现方式
60 Encoder/Decoder,比较,数理 L2 请描述Encoder和Decoder中Attention机制的三点不同之处并阐述其数学原理
61 Decoder, 数理 L2 Transformer进行Training的全生命周期的在Decoder中是如何进行Embedding的呢？请阐述其流程和数学原理
62 Decoder, 数理 L2 Transformer进行Inference的全生命周期的在Decoder中是如何进行Embedding的呢？请阐述其流程和数学原理
63 数理 L2 Transformer如果采用和Inference同样的流程来进行Training，会有什么问题？请至少指出3点问题并说明背后的数学原理
64 原理 L2 请分别描述当进行Training和Inference的时候Masking在Transformer三大不同类型使用Attention机制的地方的具体功能和数学实现
65 QKV,原理,比较 L2 请阐述Multi-head Attention机制中通过Linear layer的Matrices计算Query、Key、Value时候进行logical partition和physical partition的异同及背后的数学原理
66 算法，优化 L2 Transformer的一种优化机制之一是共享不同Layer中的attention-feedforward操作中的参数，请分析这种优化方式可行性的神经网络内部支撑机制和数学原理
67 数理 L2 为什么Transformer中的Attention Score能够衡量不同Words之间Relevance的不同程序呢？请说明背后的物理机制和数学原理
68 数理 L2 Transformer是如何知道什么样的Weights能够使得其更好的表达不同信息部分的不同程度的注意力的？请描述其运行机制和背后的数学假设
69 原理,数理 L2 为什么在Transformer的Attention计算的时候需要进行Scaling操作，请从神经网络和数学原理的角度进行解释
70 原理 L2 在Transformer中，一个输入文本词汇的顺序是由position encoding来表达还是由multi-head attention来具体实现的？请阐述运行机制和数学原理
71 原理,代码 L2 请描述multi-head attention的至少三种实现方式并提供相应的示例实现代码
72 数理,算法细节 L2 请描述Transformer中三种类型的non-linear操作、具体功能，并阐述请数学原理
73 BERT,Tokenization L2 请描述BERT的Tokenization机制的优势和不足，及针对不足的解决方案
74 工程 L2 训练Transformer时候，如果因为内存大小限制导致连一个Instance的训练都无法容纳，该如何完成所有Instance的训练，请描述详细的工程过程
75 数理 L2 请描述Beam Search算法在Transformer中的具体应用并阐述其有效性的数学假设和数学公式
76 工程 L2 如何使用Transformer实现一个能够同时预测Intent和Entity的信息系统？使用一个Transformer模型同时预测Intent和Entity有什么弊端？请分析该弊端的产生的原因并提出具体的解决方案
77 工程,比较 L2 请问使用Transformer和CRF做NER哪个更好？请提出至少3个工程落地的最佳实践。
78 工程 L2 当有新的数据的来训练Transformer模型的时候，如何实现模型的增量训练？
79 工程,数理 L2 请分析如何使用Transformer探测Toxic语言，Toxic语言能够通过Tansformer移除吗？请分析工程实践和数学原理
80 工程,Naive Bayes L2 为什么说Transformer基于对Bayesian的时候极大的降级了训练时候的overfitting？请阐述工程工程和数学原理
81 数理,算法细节 L2 请详解描述使用Transformer进行Transfer Learning中具体Prior和Posterior地方及其具体的功能和数学原理
82 数理,算法细节 L2 请描述Transformer在Training和Inference对MLE(maximum likelihood estimation)模型具体应用
83 数理 L2 请描述Transformer在Training的时候具体使用MAP(Maximum A Posteriori) estimation 模型的地方并描述其流程机制和数学原理
84 数理 L2 请描述Transformer在训练的过程中什么情况下使用MLE和MAP是基本没有区别的，其背后的数学原理是什么？
85 数理,Naive Bayes L2 请描述Naive Bayes在Transformer的Auto-encoding模型训练时候的具体应用及其有效性的数学证明
86 数理,Naive Bayes L2 请描述Naive Bayes在Transformer的Auto-regressive模型训练时候的具体应用，这样能够在小样本数据的时候帮助取得优质德训练效果？其有效性的数学证明是什么？
87 数理,Naive Bayes L2 请描述Naive Bayes在Transformer的Generative Process的具体流程和有效性的数学证明
88 工程,数理,Naive Bayes L2 使用Naive Bayes来完成Transformer的Generative Process会有什么问题？问题背后工程实现限制和数学原因是什么？
89 算法细节 L2 生产环境中的数据呈现非线性及不稳特征，原始时序数据波动较大，少数异常点偏离中心阈值，Transformer 能较好的拟合生产中的非线性时序特征分布吗？如不能完全拟合，那么是产生了欠拟合吗？ 相对于Transformer模型，深度学习时序模型预测值跟训练集数据基本一致，是产生过拟合现象吗？完全拟合训练数据中的噪声和正常数据，效果就一定最好吗？Transformer模型拟合了数据的平稳长时间序列特征，预测就一定是表面感知的不准吗？Transformer模型预测的优势到底在哪里？
90 工程 L2 Transformer 模型训练中涵盖数十个超参数，包括不限于d_model、n_heads、e_layers、d_layers、dim_fcn、factor、dropout、attn、epochs、batch_size、learning_rate、seq_len、label_len、pred_len，在生产环境应用中，在少则几百万动辄上万亿的模型参数面前，如何调整超参数达到Transformer模型最佳预测效果， 超参数需调整到什么程度？
91 算法细节 L2 请分析如何使用Transformer来有效的对Knowledge Graph中的Edge进行Encoding？
92 QKV,算法细节 L3 Transformer中的可训练Queries、Keys和Values矩阵从哪儿来？Transformer中为何需要使用Queries、Keys和Values矩阵，而不是仅仅通过线性变换后的Values矩阵本身来求Attention？
93 FF,算法细节 L3 Transformer的Feed Forward层在训练的时候到底在训练什么？请具体阐述内部机制并使用具体的视觉识别或者NLP领域的实例来说明
94 FF,算法细节 L3 请具体分析一下Transformer的Attention层和Feedforward层的复杂度并与CNN、RNN等进行比较
95 Positional Encoding,算法细节 L3 Transformer的Positional Encoding是如何表达相对位置关系的，位置信息在不同的Encoder的之间传递会丢失吗？
96 Layer Norm,算法细节 L3请描述Naive Bayes在Transformer的Auto-regressive模型训练时候的具体应用，这样能够在小样本数据的时候帮助取得优质的训练效果？其有效性的数学证明是什么？ Layer Normalization蕴含的神经网络的假设是什么？为何使用Layer Norm？请提供具体的数学分析
97 Encoder/Decoder L3 请从数学原理的角度分析Transformer中的Decoder和Encoder的依存关系
98 Tokenization,数理 L3 请描述Transformer中的Tokenization的数学原理、运行流程、问题及具体改进方法
99 BERT L3 Bert能够有效的表达Sentence Embeddings吗？请至少提出两种提升Bert的Sentence表达能力的方式
100 Encoder/Decoder L3 请描述只由一个Encoder和Decoder的Transformer使用了Attention的三个地方及其功能
101 编程 L3 请使用Einsum的方式编码实现Transformer的Attention机制

  </pre>
</b>
