# labelImg2easydl
labelImg标记文件导入easydl工具

labelImg标记转Easydl物体检测模型数据集封装

1 修改esaydl.conf，修改自己的client_id、client_secret

2 在easydl物体检测模型中创建一个数据集，并记下数据集id

3 参考test.py,一个语句就可以完成数据集（参数为数据集id和labelImg数据目录）

代码基于python 3.6，不同版本请自行修改代码调试


代码调用方式(参考test.py)

import easydl

easydl.addentitybatch(20076,r"C:\\Users\\KOOKY\\Desktop\\works")

直接命令行方式

python main.py -dataset_id 20076 -xmlpath C:\\Users\\KOOKY\\Desktop\\works


________________________________________________________________

自己的easydl数据集导出工具参见：

https://github.com/kooky126/easydl2labelImg
