# NAScompetition-gp-ensemble

文件夹说明：


B榜提交原始代码-附带提交时刻checkpoint：
  纯粹的原始代码，不含注释。
  包含可能是最后一次提交的原始代码以及checkpoint
  运行方式：
  依次运行task0.ipynb - task7.ipynb生成7个task的结果，最后运行Combinator.ipynb生成最后结果。

训练代码:
  训练模型的代码，输出模型参数到gp_ensemble_task0.pickle - gp_ensemble_task7.pickle
  在task0.ipynb，我们基于要求对于对应的步骤加入了解释性注释与一些讨论。
  其他的task1 - task7因为比较类似，因此暂时不添加。
  依次运行task0.ipynb - task7.ipynb生成7个task的结果

预测代码(需要将预训练结果复制进去）
文件夹内需要有gp_ensemble_task0.pickle - gp_ensemble_task7.pickle这样的训练好的模型文件
依次运行task0.ipynb - task7.ipynb生成7个task的结果，最后运行Combinator.ipynb整合之前的各个task的结果，并生成最后结果。




补充材料（基于贝叶斯优化的kernel weight 寻优）
基于贝叶斯优化的方式生成kernel的weight
注意：不同系统中运行的结果可能会比较不一致，本目录下有探讨推荐的系统配置。

  依次运行目录下5份ipynb文件，生成
  optimweight_fast.pkl
  
  optimweight_0703_leftskewness_fast.pkl
  
  optimweight_065035_fast.pkl
  
  optimweight_0703_fast.pkl
  
  optimweight_0109_skewness_fast.pkl
  
  
 这5个文件是5种不同的kernel weight, 使用的时候需要放在data目录下。
