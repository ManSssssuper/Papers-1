#1 多任务学习
&emsp;&emsp;同时优化多个相关的学习任务
##任务（Task）的定义
&emsp;&emsp;A task is generally referred to the learning of an output target using a single input source. If the input source consists of a single variable (or feature), we will have **a univariate analysis**, if the input source consists of multiple variables (or features), we will have **a multivariate analysis**.

&emsp;&emsp;任务通常是指使用单个输入源学习输出目标。
如果输入源由单个变量(或特征)组成，我们将进行**单变量分析**;如果输入源由多个变量(或特征)组成，我们将进行**多元分析**。
##多任务学习的形式
&emsp;&emsp;“multiple tasks” could mean the learning of multiple output targets using a single input source, or the learning of single output target using multiple input sources, or a mixture of both.

&emsp;&emsp;“多任务”可能意味着使用一个输入源学习多个输出目标，或者使用多个输入源学习单个输出目标，或者两者兼而有之。
##多任务学习的目的
&emsp;&emsp;MTL is an approach to inductive transfer that improves generalization by using the domain information contained in the training signals of related tasks as an inductive bias. It does this by learning tasks in parallel while using a shared low dimensional representation; what is learned for each task can help other tasks be learned better.

&emsp;&emsp;MTL是一种归纳转移方法，它使用包含在相关任务训练信号中的域信息作为归纳偏差来提高泛化。同在使用一个共享的低维表示的同时并行地学习任务；在每个任务中所学到的东西可以帮助其他任务学得更好。
##1.3MTL的一些应用
&emsp;&emsp;特征选择问题：特征选择的时候使用联合选择正则化矩阵方法，效果比多多个源数据单独进行特征选择要好。

&emsp;&emsp;神经性疾病诊断：单数据源多输出。

&emsp;&emsp;汽车的目标检测：神经网络预测多类别目标。

##1.4相关研究领域
&emsp;&emsp;归纳迁移学习是MTL的一个特殊例子：归纳迁移学习学习任务有主次之分，而MTL所有任务都是平等的。

&emsp;&emsp;MTL与learning-to-learn相联系。
#2 多任务学习算法表述
&emsp;&emsp;传统MTL算法的典型表示：

<div align=center>![Formulation of MTL algorithms](https://i.imgur.com/8daFzTA.png)


