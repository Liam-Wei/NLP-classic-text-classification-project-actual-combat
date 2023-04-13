![在这里插入图片描述](https://img-blog.csdnimg.cn/6334194be4d94ebca2dd18245cb4e1ef.jpeg#pic_center)


---

# 前言
大家好，我是阿光。

本专栏整理了《NLP文本分类算法集锦》，内包含了各种常见的中英文文本分类算法，以及常见的NLP任务：情感分析、新闻分类以及谣言检测等。

![在这里插入图片描述](https://img-blog.csdnimg.cn/8a8c6cc103fe46abadc877f2e3742e06.png#pic_center)

文本分类是NLP的必备入门任务，在搜索、推荐、对话等场景中随处可见，并有情感分析、新闻分类、标签分类等成熟的研究分支和数据集。

不同模型的适用场景不同，常用的模型有：

`Fasttext`、`TextCNN`、`DPCNN`、`TextRCNN`、`BiLSTM+Attention`、`HAN`、`LSTM`、`Transformer`、`BERT`、`Capsule`、`TextGCN` 等。

文本分类广泛应用于 `长短文本分类`、`情感分析`、`新闻分类`、`事件类别分类`、`政务数据分类`、`商品信息分类`、`商品类目预测`、`文章分类`、`论文类别分类`、`专利分类`、`案件描述分类`、`罪名分类`、`意图分类`、`论文专利分类`、`邮件自动标签`、`评论正负识别`、`药物反应分类`、`对话分类`、`税种识别`、`来电信息自动分类`、`投诉分类`、`广告检测`、`敏感违法内容检测`、`内容安全检测`、`舆情分析`、`话题标记` 等日常或专业领域中。


正在更新中~ ✨  

![在这里插入图片描述](https://img-blog.csdnimg.cn/img_convert/e0fb91ed8ee12ea1d35b3a0339ff9282.jpeg#pic_center)



🚨 我的项目环境：

+ 平台：Windows10
+ 语言环境：python3.7
+ 编译器：PyCharm
+ PyTorch版本：1.8.1

---

# 🌠 『精品学习专栏导航帖』

+ **🐧[<font color=Tomato>【Matplotlib绘制图像目录】Python数据可视化之美](https://weibaohang.blog.csdn.net/article/details/128132121)🐧**

+ **🎠[<font color=Sienna>【Pandas数据处理100例目录】Python数据分析玩转Excel表格数据](https://weibaohang.blog.csdn.net/article/details/128067702)🎠**

+ **🐳[<font color=red>最适合入门的100个深度学习实战项目](https://weibaohang.blog.csdn.net/article/details/127365867?spm=1001.2014.3001.5502)🐳**
+ **🐙[<font color=orange>【PyTorch深度学习项目实战100例目录】项目详解 + 数据集 + 完整源码](https://weibaohang.blog.csdn.net/article/details/127128637?spm=1001.2014.3001.5502)🐙**
+ **🐶[<font color=gold>【机器学习入门项目10例目录】项目详解 + 数据集 + 完整源码](https://blog.csdn.net/m0_47256162/article/details/128011714?spm=1001.2014.3001.5501)🐶**
+ **🦜[<font color=green>【机器学习项目实战10例目录】项目详解 + 数据集 + 完整源码](https://blog.csdn.net/m0_47256162/article/details/128055406?spm=1001.2014.3001.5501)🦜**
+ **🐌[<font color=darkcyan>Java经典编程100例](https://blog.csdn.net/m0_47256162/article/details/113728127)🐌**
+ **🦋[<font color=blue>Python经典编程100例](https://blog.csdn.net/m0_47256162/article/details/110746376)🦋**
+ **🦄[<font color=purple>蓝桥杯历届真题题目+解析+代码+答案](https://blog.csdn.net/m0_47256162/article/details/110476937)🦄**
+ **🐯[<font color=deepskyblue>【2023王道数据结构目录】课后算法设计题C、C++代码实现完整版大全](https://weibaohang.blog.csdn.net/article/details/124415748)🐯**

---

### 🍭『目录』
**📢 经典模型篇**

+ [（一）：基于TextCNN实现情感分析任务](https://weibaohang.blog.csdn.net/article/details/128423227)
+ [（二）：基于FastText实现情感二分类任务](https://weibaohang.blog.csdn.net/article/details/128423624)
+ [（三）：基于DPCNN实现电商情感分析任务](https://weibaohang.blog.csdn.net/article/details/128424383)
+ [（四）：基于TextRNN实现情感短文本分类任务](https://weibaohang.blog.csdn.net/article/details/128426941)
+ [（五）：基于TextRCNN实现中文短文本分类任务](https://weibaohang.blog.csdn.net/article/details/128427344)
+ [（六）：基于CharCNN实现中文情感分类任务](https://weibaohang.blog.csdn.net/article/details/128428873)
+ [（七）：基于PyTorch+TextCNN实现英文长文本诗歌文本分类](https://weibaohang.blog.csdn.net/article/details/128433605)
+ [（八）：基于PyTorch+HAN实现中文情感分类任务](https://weibaohang.blog.csdn.net/article/details/128431563)
+ [（九）：基于MultinomialNB多项式贝叶斯分类器实现中文文本情感分类任务](https://weibaohang.blog.csdn.net/article/details/128438762)
+ [（十）：基于一维卷积Conv1D对电商评论数据文本情感分类](https://weibaohang.blog.csdn.net/article/details/127313642)
+ [（十一）：基于自注意力机制（Self-Attention）对twitter数据进行情感分析](https://weibaohang.blog.csdn.net/article/details/127288852)
+ [（十二）：基于RNN实现微博热点新闻分类](https://weibaohang.blog.csdn.net/article/details/127234487)
+ [（十三）：基于词级ngram的词袋模型对twitter数据进行情感分析](https://blog.csdn.net/m0_47256162/article/details/127208908?spm=1001.2014.3001.5501)
+ [（十四）：基于pytorch使用LSTM实现新闻本文分类任务](https://weibaohang.blog.csdn.net/article/details/127159062?spm=1001.2014.3001.5501)
+ [（十五）：基于pytorch使用LSTM进行谣言检测](https://weibaohang.blog.csdn.net/article/details/127155442?spm=1001.2014.3001.5501)
+ [（十六）：基于pytorch使用LSTM进行文本情感分析](https://weibaohang.blog.csdn.net/article/details/127154284?spm=1001.2014.3001.5501)
+ [（十七）：基于CNN实现冠状病毒推文NLP文本分类](https://weibaohang.blog.csdn.net/article/details/127348054)

---
**📢 融合模型篇**

+ [（一）：基于PyTorch+Conv-GRNN & LSTM-GRNN实现中文情感分类任务](https://weibaohang.blog.csdn.net/article/details/128432227)
+ [（二）：基于PyTorch+CNN实现谣言检测任务](https://weibaohang.blog.csdn.net/article/details/128438944)
+ [（三）：基于PyTorch+Transformer实现谣言检测系统](https://weibaohang.blog.csdn.net/article/details/128439218)
+ [（四）：基于RNN+CNN实现NLP判别新闻真伪](https://weibaohang.blog.csdn.net/article/details/127350130)
+ [（五）：基于BiLSTM-Attention实现中文文本分类任务](https://weibaohang.blog.csdn.net/article/details/128427523)

---
**📢 大模型篇**

+ [（一）：基于Pytorch+Bert实现电商情感多分类任务](https://weibaohang.blog.csdn.net/article/details/128425021)
+ [（二）：基于ERNIE2.0文心大模型实现中文短文本分类任务](https://weibaohang.blog.csdn.net/article/details/128425948)
+ [（三）：基于飞浆ERNIE3.0百亿级大模型实现中文短文本分类任务](https://weibaohang.blog.csdn.net/article/details/128426059)
+ [（四）：基于Google的预训练模型XLNet实现电商情感多分类任务](https://weibaohang.blog.csdn.net/article/details/128429547)
+ [（五）：基于GPT2实现中文新闻文本分类任务](https://weibaohang.blog.csdn.net/article/details/128430935)
+ [（六）：基于Transformer实现Twitter文本隐喻二分类](https://weibaohang.blog.csdn.net/article/details/127337832)
+ [（七）：基于Transformer实现电影评论星级分类任务](https://weibaohang.blog.csdn.net/article/details/127335678)
