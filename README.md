一个英语不好的鼠鼠却要上全英课（且是有口音的外教）的自救指南  
欢迎继续补充，互帮互助！！！

### 目前功能：

> 进行**解读**和**翻译**和**格式转化-数学符号渲染**和**格式转化-图片**  
> 调用mineru，进行**图片截取**

### 效果展示：

<p align="center">
	<img src="images/Pasted image 20250926211635.png" alt="base motion" width="90%" />
</p>

### 食用方法：

- 如果你手上没有课件，资源只有上课拍的PPT：
	1. 手机电脑同时下载“微信输入法”，实现手机电脑信息互传
	2. 手机上将Prompt喂给豆包，再把照片喂给豆包，把结果复制给电脑
	3. 电脑用支持markdown的笔记软件渲染（首推Obsidian！本地存储+分屏功能非常适合知识库搭建）
- 如果在课前你已经有课件资源，可以用mineru的图片分割，截取功能增强你的笔记

### 功能增强：

1. 图片分割，截取功能
	- 有条件的话（6GB+ VRAM； 32GB+RAM；SSD recommended  20GB+）可以本地部署mineru（避免排队问题）  [https://github.com/opendatalab/mineru](https://github.com/opendatalab/mineru)
	- 用于提取文字和图片截取（不做格式调整和“解读”），然后把结果作为input，输入online的GPT模型（性能更强，理解更好）

### 可能遇到的问题：

- 大模型上下文token限制，一次性不要传太多内容，否则部分内容可能质量不高。
