# GAIIC2022商品标题实体识别Baseline，使用GlobalPointer实现

## 简介

比赛名称：GAIIC2022商品标题实体识别

测评任务：本赛题要求选手使用模型抽取出商品标题文本中的实体。与传统的实体抽取不同，京东商品标题文本的实体密度高、实体粒度细，赛题具有特色性。 

任务类型：命名实体

测评链接：<https://gaiic.caai.cn/ai2022>

注意事项：本Baseline开源经大赛组委会同意 ，建议大家开源Baseline前先联系主办方

## 思路

使用苏神提出的[GlobalPointer](https://github.com/bojone/GlobalPointer)设计，它利用全局归一化的思路来进行命名实体识别（NER），可以无差别地识别嵌套实体和非嵌套实体。


## 环境

```
pip install ark-nlp
pip install pandas
```
ark-nlp开源地址：https://github.com/xiangking/ark-nlp

## 目录结构

```shell
│
├── data                                    # 数据文件夹
│   ├── source_datasets                                                   
│
└── code                                    # 代码
```

## 使用说明

下载数据并解压到`data/source_datasets`中，运行`code`文件夹中的`baseline.ipynb`

## 效果

- 线上测试：0.80151539
