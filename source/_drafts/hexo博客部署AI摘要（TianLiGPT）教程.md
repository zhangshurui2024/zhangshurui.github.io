---
abbrlink: ''
categories:
- - Hexo
- - 教程
date: '2024-08-08T18:38:18.059321+08:00'
description: null
mathjax: true
tags:
- 教程
- Hexo
title: hexo博客部署AI摘要（TianLiGPT）教程
updated: '2024-08-08T18:38:20.771+08:00'
---
# **前言**

**现在ai挺火的，给博客整个ai摘要岂不美哉？本文不算打广告哦，因为……确实挺好用的，并且有任何问题都可以很快反馈（博主亲身经历）**

# **什么是TianliGPT**

**TianliGPT是一个基于GPT-3.5的文字摘要生成工具，你可以将需要提取摘要的文本内容发送给TianliGPT，稍等一会他就可以给你发送一个基于这段文本内容的摘要。**

* **实时生成的摘要**
* **自动生成，无需人工干预**
* **一次生成，再次生成无需消耗key**
* **包含文字审核过滤，适用于中国大陆**
* **支持中国大陆访问**

# **部署ai摘要**

## **引用**

**在博客靠后的位置位置引入js和css（需要在文章之后）**

**XML**

`

```
<link rel="stylesheet" href="https://cdn1.tianli0.top/gh/zhheo/Post-Abstract-AI@0.15.2/tianli_gpt.css">  
<script>  
let tianliGPT_postSelector = '#post #article-container';  
let tianliGPT_key = '5Q5mpqRK5DkwT1X9Gi5e';  
</script>  
<script src="https://cdn1.tianli0.top/gh/zhheo/Post-Abstract-AI@0.15.2/tianli_gpt.js"></script>
````

如果你使用的是Butterfly主题，可以在主题文件夹下的themes/butterfly/\_config.yml文件中的inject属性中配置：

**XQUERY**

`

```
inject:  
  head:  
  	- <link rel="stylesheet" href="https://cdn1.tianli0.top/gh/zhheo/Post-Abstract-AI@0.15.2/tianli_gpt.css">  
  bottom:  
  	- <script>let tianliGPT_postSelector = '\#post \#article-container';let tianliGPT_key = '5Q5mpqRK5DkwT1X9Gi5e';</script>  
	- <script src="https://cdn1.tianli0.top/gh/zhheo/Post-Abstract-AI@0.15.2/tianli_gpt.js"></script>
````

我们需要更改一些参数来让这个模型运作起来。

tianliGPT\_postSelector和tianliGPT\_key

## tianliGPT\_**postSelector

**这个参数是填写你的博客文章所在的元素属性的选择器，在生成提交的文本时，只会将这个选择器对应的元素内的文本进行提交，并且在这个选择器对应的元素上放插入AI摘要。如果你使用的是Butterfly主题，那么为#post #article-container。**

**这里列出一些常见博客主题的选择器值：**

[图片](https://picst.sunbangyan.cn/2023/11/24/448b4c69c6782f59f4e6e5370ecacb06.jpeg)

## **tianliGPT\_**key****

**到**[爱发电](https://afdian.net/item/f18c2e08db4411eda2f25254001e7c00)中购买，原价10元5万字符（Heo限量限时折扣9元）。请求过的内容再次请求不会消耗key，可以无限期使用。

**购买完成后，进入管理后台：**[https://summary.zhheo.com/](https://summary.zhheo.com/)

**登录后点击右上角的“添加新网站”，输入密钥即可**

**即可绑定成功。**

**参考链接： **[https://blog.zhheo.com/p/ec57d8b2.html](https://blog.zhheo.com/p/ec57d8b2.html)
