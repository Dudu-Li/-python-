# -*- coding: utf-8 -*-
"""
函数说明:打开并解析文件，创建测试数据集和标签集
 
Parameters:
    filename - 文件名
Returns:
    dataSet - 数据集
    labels - 特征标签
Author:
    lizj
"""
def createDataSet(filename):   
    #打开文件
    fr = open(filename)
    #读取文件所有内容
    Lines = fr.readlines()
    dataSet = []
    labels = []
    i = 0
    for line in Lines:
		#s.strip(rm)，当rm空时,默认删除空白符(包括'\n','\r','\t',' ')
        line = line.strip()
        #使用s.split(str="",num=string,cout(str))将字符串根据'\t'分隔符进行切片。
        listFromLine = line.split('\t')
        #将数据提取出来,存放到数据集dataSet中
        dataSet.append(listFromLine)
        #将分类标签提取出来，放在labels中
        labels.append(listFromLine[-1])
        i += 1
    return dataSet, labels
