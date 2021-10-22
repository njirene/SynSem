一：clingo工具
1. clingo工具为使用ASP规则抽取评价对象的程序。
2. clingo工具的使用在其文件夹中有说明。

二：代码部分
1. SelectObjectRule压缩包内的根目录下的py文件为预处理数据的程序。
对于将原始文本处理为SEM-G和SYN-G方式的事实文件，涉及到的代码文件为：preprocessForPos.py、AMR_Dep.py、AMR_Dep_Pos.py、AMR_Pos.py、Dep.py、Dep_AMR.py、Dep_AMR_Pos.py、Dep_Pos.py。

2. SelectObjectRule压缩包内的AutoSelectRules文件夹内为特化规则进行抽取评价对象的程序。
对于SEM-C和SYN-C方式的规则特化代码文件：SynSemCAllStepsInOne.py
对于SEM-G和SYN-G方式的规则特化代码文件：SynSemCAllStepsInOneForG.py
对应的贪心选择代码文件分别为：insertRulesSortAndGreedy.py和greedy.py
对贪心选择的规则进行错误分析的代码文件：errorGet.py、diffFile.py、disAllAndDomain.py
单次使用ASP规则抽取评价对象的代码文件：execFindOT.py
对规则进行评价的代码文件：evaluation.py

三：配置说明
1. 路径配置：
(1)将代码和clingo工具放在D://PaperCodeAndResearch//文件夹中，然后将SelectObjectRule改名为AMR_code。
(2)若将代码放在其他文件夹，自己配置代码内部的路径。
2. 安装nltk包，python版本为3.x
