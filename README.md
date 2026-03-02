# ABIDE自闭症功能连接矩阵数据集
本文档是自闭症脑影像数据交换中心（Autism Brain Imaging Data Exchange, ABIDE）中多个站点的功能脑影像数据在医学标准处理后的数据，包含处理后的功能连接矩阵（FC）和临床诊断量表。

脑区模板：AAL116模板 和 Dosenbach160模板

## 文件结构与内容说明
ABIDEI文件夹

	NYU_I_age6-39  	 //NYU_I站点样本
		FC_Dosenbach160   	 //Dosenbach160模板的功能连接矩阵
			GretnaSFCMatrixR   	 //原始功能连接矩阵（脑区时间序列的皮尔逊相关系数矩阵）
				rASD29539.txt   	 //样本矩阵（自闭症患者），为160x160的对称矩阵
				rTC29552.txt   	 //样本矩阵（健康对照）
				...
			GretnaSFCMatrixZ   	 //Fisher-Z 变换后的功能连接矩阵
				zASD29539.txt   	 //样本矩阵（自闭症患者）
				zTC29552.txt   	 //样本矩阵（健康对照）
				...
			GretnaTimeCourse   	 //脑区时间序列数据
				ASD29539.txt   	 //样本矩阵（自闭症患者）
				TC29552.txt   	 //样本矩阵（健康对照）
				...
		FC_AAL116   	 //AAL116模板的功能连接矩阵
			...
	KKI_I_age8-13  	 //KKI_I站点样本
	...
ABIDEII文件夹

	...（与ABIDEI类似）
ABIDEI_phenotypic_fMRI.xlsx   	&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; //ABIDEI对应样本的基本信息和临床诊断表

	SITE_ID：站点
	SUB_ID：样本编号
	DX_GROUP：组别，1为自闭症，2为健康对照
	AGE_AT_SCAN：年龄
	SEX：性别
	FIQ：全量表智商
	VIQ：语言智商
	PIQ：操作智商（非语言智商）
	ADOS_TOTAL：ADOS是诊断观察量表的核心指标，这里是ADOS评估的总分
	ADOS_COMM：ADOS沟通维度得分
	ADOS_SOCIAL：ADOS社交维度得分
	ADOS_STEREO_BEHAV：ADOS刻板行为维度得分
	...
ABIDEII_phenotypic_fMRI.xlsx   	 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;//ABIDEII对应样本的基本信息和临床诊断表

	...

其中每个患者仅有一次脑影像扫描数据，无发育过程中的连续扫描数据。

