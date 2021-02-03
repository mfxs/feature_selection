# Feature Selection

+ **Feature Selection with Neural Networks**
> 介绍了三类基于神经网络的特征选择方法，分别采用基于零阶、一阶和二阶导数的变量重要性度量指标，通常基于神经网络的特征选择方法采用后向搜索，即从特征全集逐个删除不重要的特征。

+ **A new wrapper feature selection approach using neural network**
> 提出一种在提取特征的同时对网络结构（即隐层神经元个数）进行自适应学习的包裹式特征选择方法，首先将所有特征依据相关系数分为两类，再在不断增加特征的同时根据模型在验证集上的表现增加隐层神经元的个数。

+ **Eliminating redundancy and irrelevance using a new MLP-based feature selection method**
> 基于神经网络的连接权重计算特征的贡献程度，同时考虑特征间的相关性大小，实现冗余和不相关变量的剔除。

+ **The ANNIGMA-Wrapper Approach to Fast Feature Selection for Neural Nets**
> 提出一种基于连接权重和模型预测误差的特征重要性度量方式，并结合后向搜索策略实现特征选择。

+ **Neural-Network Feature Selector**
> 通过在网络的loss中加入模型参数项以使得不重要特征的连接权重尽可能小，再比较将不同特征连接权重置为零时模型性能的下降情况，实现特征的选择。

+ **Feature Selection Using a Neural Network With Group Lasso Regularization and Controlled Redundancy**
> 利用Group Lasso正则项实现权重系数矩阵的分组稀疏化，从而实现特征选择，同时控制特征的冗余性，避免过多冗余特征的引入以及过少冗余特征导致鲁棒性下降，因此损失函数包含预测误差损失、Group Lasso正则项损失和特征冗余损失三项，使用平滑函数对正则项进行估计，避免由于在原点处不可导导致训练过程中产生震荡。

+ **Design and Application of a Variable Selection Method for Multilayer Perceptron Neural Network With LASSO**
> 每个特征在参与网络运算时多引入一个对应的系数，并在目标函数中加入该系数的一范数，从而实现稀疏化进行特征选择。

+ **Efficient and Robust Feature Selection via Joint $l_{2,1}$-Norms Minimization**
> 提出一种同时在预测误差损失和正则项中使用$L_{2,1}$范数的特征选择方法和求解方法，在预测误差损失中使用$L_{2,1}$范数能够减小离群点的影响作用，这个不是很清楚原因。

+ **Group sparse regularization for deep neural networks**
> 提出一种稀疏分组Lasso正则项，通过分组计算网络中权重和偏置的损失，使得参数的学习更容易满足结构化稀疏性，同时加入$L_1$正则项进一步压缩无法实现结构化稀疏的参数，最终能够实现特征选择和神经元剪枝，获得更精简的网络模型。

+ **Sparse group LASSO based uncertain feature selection**
> 提出一种应用于不确定性数据的稀疏分组Lasso特征选择方法，本质上通过在每个样本点附近采样来描述数据的不确定性，即特征扩展，进而使得特征呈现出分组特性，再采用稀疏分组Lasso进行特征选择。