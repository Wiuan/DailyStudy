---
title: "开源RAG框架汇总"
source: "https://juejin.cn/post/7367215439032303626"
author:
  - "[[深度学习机器]]"
published: 2024-05-10
created: 2025-09-27
description: "本文搜集了一些开源的基于LLM的RAG（Retrieval-Augmented Generation）框架"
tags:
  - "clippings"
---
![横幅](https://p9-piu.byteimg.com/tos-cn-i-8jisjyls3a/8c759ddb57d0440986f4768fc644f879~tplv-8jisjyls3a-2:0:0:q75.image)

[深度学习机器](https://juejin.cn/user/486421344552179/posts)

2,915 阅读3分钟

专栏：

大语言模型

![](https://p3-piu.byteimg.com/tos-cn-i-8jisjyls3a/b37ce6cd3dfa46f699d8fc9c7c888f2f~tplv-8jisjyls3a-3:0:0:q75.png)

## 前言

本文搜集了一些开源的基于LLM的RAG（Retrieval-Augmented Generation）框架，旨在吸纳业界最新的RAG应用方法与思路。如有错误或者意见可以提出，同时也欢迎大家把自己常用而这里未列出的框架贡献出来，感谢~

## RAG应用框架

1. RAGFlow
- 项目地址： [github.com/infiniflow/…](https://link.juejin.cn/?target=https%3A%2F%2Fgithub.com%2Finfiniflow%2Fragflow "https://github.com/infiniflow/ragflow")
- 简介：RAGFlow 是一款基于深度文档理解构建的开源 RAG（Retrieval-Augmented Generation）引擎。RAGFlow 可以为各种规模的企业及个人提供一套精简的 RAG 工作流程，结合大语言模型（LLM）针对用户各类不同的复杂格式数据提供可靠的问答以及有理有据的引用。
- 特性：OCR、 **内置多种文档切分模板** 、文档切分可视化并且可修改、兼容多种文档数据类型
- 架构： ![在这里插入图片描述](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/62b06f7e25204bbe8624b5796ad27cee~tplv-k3u1fbpfcp-jj-mark:3024:0:0:0:q75.awebp#?w=7680&h=4320&s=769059&e=png&b=f1f2f7)
- 硬件要求：CPU >= 4 核、RAM >= 16 GB、Disk >= 50 GB、Docker >= 24.0.0 & Docker Compose >= v2.26.1
1. QAnything
- 项目地址： [github.com/netease-you…](https://link.juejin.cn/?target=https%3A%2F%2Fgithub.com%2Fnetease-youdao%2FQAnything "https://github.com/netease-youdao/QAnything")
- 简介：QAnything ( Q uestion based on Anything ) 是贡献支持任何格式文件或数据库的本地知识库问答系统，可断网安装使用。您的任何格式的本地文件都可以往里扔，即可获得准确、快速、靠谱的问答体验。
- 特性：支持离线安装使用、 **跨语种问答** 、 **粗排和精排的二阶段召回**
- 架构： ![在这里插入图片描述](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/7f09aee4689a49918e4d6b035c92623d~tplv-k3u1fbpfcp-jj-mark:3024:0:0:0:q75.awebp#?w=1146&h=1016&s=283618&e=png&b=fdfbfb)
- 硬件要求：最低CPU即可；使用GPU环境需要NVIDIA GPU Memory >= 4GB (use OpenAI API) & Docker Desktop >= 4.26.1（131620）
1. open-webui
- 项目地址： [github.com/open-webui/…](https://link.juejin.cn/?target=https%3A%2F%2Fgithub.com%2Fopen-webui%2Fopen-webui "https://github.com/open-webui/open-webui")
- 简介：Open WebUI 是一个可扩展、功能丰富且用户友好的自托管 WebUI，旨在完全离线操作。它支持各种 LLM 运行程序，包括 Ollama 和 OpenAI 兼容的 API。
- 特性： **原生支持Ollama** 、 **支持安装和卸载模型** 、 **支持多模态模型** 、 **支持切换模型** 、 **多用户管理**
- 架构： ![在这里插入图片描述](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/7ac083633a174598bb8d8c56e67c2c5a~tplv-k3u1fbpfcp-jj-mark:3024:0:0:0:q75.awebp#?w=1920&h=1080&s=5192022&e=gif&f=380&b=141312)
- 硬件要求：最低CPU即可，使用GPU环境需要NVIDIA GPU Memory >= 4GB (取决于使用Ollama的模型大小)
1. FastGPT
- 项目地址： [github.com/labring/Fas…](https://link.juejin.cn/?target=https%3A%2F%2Fgithub.com%2Flabring%2FFastGPT "https://github.com/labring/FastGPT")
- 简介：FastGPT 是一个基于 LLM 大语言模型的知识库问答系统，提供开箱即用的数据处理、模型调用等能力。同时可以通过 Flow 可视化进行工作流编排，从而实现复杂的问答场景！
- 特性： **支持应用编排** 、 **免登录分享** 、 **支持接入飞书、企业微信等应用**
- 架构： ![在这里插入图片描述](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/b6a77d25a4084bb38741dfb849c5bf0e~tplv-k3u1fbpfcp-jj-mark:3024:0:0:0:q75.awebp#?w=4605&h=3333&s=167820&e=webp&b=fbfbfb)
- 硬件要求：CPU >= 2 核、RAM >= 4 GB用于安装数据库，GPU取决于使用的模型
1. Langchain-Chatchat
- 项目地址： [github.com/chatchat-sp…](https://link.juejin.cn/?target=https%3A%2F%2Fgithub.com%2Fchatchat-space%2FLangchain-Chatchat "https://github.com/chatchat-space/Langchain-Chatchat")
- 简介：基于 ChatGLM 等大语言模型与 Langchain 等应用框架实现，开源、可离线部署的检索增强生成(RAG)大模型知识库项目。
- 特性：算是比较早期的RAG框架了，使用的基本全是python的框架。该项目是一个可以实现 **完全本地化** 推理的知识库增强方案, 重点解决数据安全保护，私域化部署的企业痛点。支持市面上主流的本地大语言模型和Embedding模型，支持开源的本地向量数据库。 本开源方案采用Apache License，可以 **免费商用，无需付费** 。
- 架构： ![在这里插入图片描述](https://p3-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/6c085db36b4841d6a6dea51629712c9e~tplv-k3u1fbpfcp-jj-mark:3024:0:0:0:q75.awebp#?w=1206&h=798&s=1120970&e=png&b=fdf9f9)
- 硬件要求：对GPU要求较高
1. MaxKB
- 项目地址： [github.com/1Panel-dev/…](https://link.juejin.cn/?target=https%3A%2F%2Fgithub.com%2F1Panel-dev%2FMaxKB "https://github.com/1Panel-dev/MaxKB")
- 简介：MaxKB 是一款基于 LLM 大语言模型的知识库问答系统。MaxKB = Max Knowledge Base，旨在成为企业的最强大脑。
- 特性：开箱即用，支持直接上传文档、自动爬取在线文档；支持零编码快速嵌入到第三方业务系统；支持对接主流的大模型，包括 Ollama 本地私有大模型以及API调用
- 架构： 前端：Vue.js 后端：Python / Django LangChain：LangChain 向量数据库：PostgreSQL / pgvector 大模型：Azure OpenAI、OpenAI、百度千帆大模型、Ollama、通义千问、Kimi、智谱 AI、讯飞星火
- 硬件要求： 操作系统：Ubuntu 22.04 / CentOS 7 64 位系统 CPU/内存： 推荐 2C/4GB 以上 磁盘空间：100GB

![cover](https://p1-juejin.byteimg.com/tos-cn-i-k3u1fbpfcp/95414745836549ce9143753e2a30facd~tplv-k3u1fbpfcp-jj:100:75:0:0:q75.avis)

大语言模型

专栏目录

大语言模型相关的算法、工程实现及优秀项目

14 订阅

·

55 篇文章

上一篇

【高级RAG技巧】使用二阶段检索器平衡检索的效率和精度

下一篇

热门开源Text2SQL框架

评论 0

![avatar](https://lf-web-assets.juejin.cn/obj/juejin-web/xitu_juejin_web/58aaf1326ac763d8a1054056f3b7f2ef.svg)

0 / 1000

即可发布评论！

暂无评论数据

![](https://lf-web-assets.juejin.cn/obj/juejin-web/xitu_juejin_web/c12d6646efb2245fa4e88f0e1a9565b7.svg) 3

![](https://lf-web-assets.juejin.cn/obj/juejin-web/xitu_juejin_web/336af4d1fafabcca3b770c8ad7a50781.svg) 评论

![](https://lf-web-assets.juejin.cn/obj/juejin-web/xitu_juejin_web/3d482c7a948bac826e155953b2a28a9e.svg) 收藏

![avatar](https://p26-passport.byteacctimg.com/img/user-avatar/907935e5eeff608e0a35aee1a4a67031~40x40.awebp)