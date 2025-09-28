---
title: My AI Code Prep & Cline Workflow for Budget Coding/Debugging (Part 1)
source: https://wuu73.org/blog/aiguide1.html
author: "[[wuu73]]"
published:
created: 2025-09-28
description: A personal guide on using AI Code Prep GUI, Cline, and various free AI web interfaces like Gemini, Grok, Deepseek, and Poe for cost-effective coding and debugging.
tags:
  - clippings
type: webpage
domain: wuu73.org
---
[See trending Hacker News conversation about this](https://news.ycombinator.com/item?id=44850913)

[Visit wuu73.org](https://wuu73.org/)

Last updated: July 2025 - If you want faster/more frequent/recent updates, buy my low cost context helper tool (cheap!!) [AI Code Prep Pro](https://tombrothers.gumroad.com/l/dcgufn)

## How I Code with [[AI]] on a budget/free我如何在预算/免费的情况下使用 AI 进行编码

## My Browser Setup: The Free AI Buffet我的浏览器设置：[[免费]]的 AI 自助餐

First things first, I have a browser open loaded with tabs pointing to the free tiers of powerful AI models. Why stick to one when you can get multiple perspectives for free? My typical lineup includes:  
首先，我打开了一个浏览器，其中加载了指向强大 AI 模型的免费层的选项卡。当您可以免费获得多种视角时，为什么还要坚持一个呢？我的典型阵容包括：

- At least 2-3 tabs of z.ai's GLM 4.5(https://chat.z.ai/) – free on web, and seems as good or better than Claude 4! no joke.  
	至少 2-3 个 z.ai 的 GLM 4.5 选项卡 – 在网络上免费，并且看起来与 Claude 4 一样好或更好！不是开玩笑。
- 1 or 2 tabs of [Kimi K2](https://kimi.com/).. another Claude or Opus-like model. Free to use on website.  
	1 或 2 片 Kimi K2..另一个类似 Claude 或 Opus 的模型。在网站上免费使用。
- Qwen3 Coder and other new ones at [chat.qwen.ai](https://chat.qwen.ai/).  
	Qwen3 Coder 和其他新产品在 chat.qwen.ai。
- 2 tabs of Kimi K2 at [kimi.com](https://kimi.com/). This one was fixing hard bugs multiple times a day before GLM seemed even better at it possibly.  
	2 片 Kimi K2 在 kimi.com。这个每天要多次修复硬错误，然后 GLM 似乎在这方面做得更好。
- At least one tab of [OpenAI Playground](https://platform.openai.com/playground/prompts?models=o3). If you set your account's data settings to allow OpenAI to use your data for model training, you get free tokens to use on GPT-4.5, o3, and other models.  
	至少一个 OpenAI Playground 选项卡。如果您将帐户的数据设置设置为允许 OpenAI 使用您的数据进行模型训练，您将获得可用于 GPT-4.5、o3 和其他模型的免费令牌。
- At least one tab but more like three of Google [Gemini AI Studio](https://aistudio.google.com/) (Gemini 2.5 Pro/Flash are often free and unlimited here).  
	Also, try [Google Gemini 2.5 Pro](https://gemini.google.com/app) (different than AI Studio, has better image generation and deep research; I always have a couple tabs of this along with a couple tabs of AI Studio).  
	至少有一个选项卡，但更像是三个 Google Gemini AI Studio（Gemini 2.5 Pro/Flash 通常在这里免费且无限制）。 另外，试试谷歌Gemini 2.5 Pro（与AI Studio不同，图像生成更好，研究更深入;我总是有几个选项卡以及几个 AI Studio 选项卡）。
- Couple tabs of [Poe.com](https://poe.com/) usually set to Claude 4 or o4-mini for its free daily credits on premium models.  
	Poe.com 的几个选项卡通常设置为 Claude 4 或 o4-mini，以获得高级型号的免费每日积分。
- Several tabs of [OpenRouter](https://openrouter.ai/), set to several models, some free models, some not.  
	OpenRouter 的几个选项卡，设置为多种型号，有些免费型号，有些则不然。
- At least one tab for [ChatGPT](https://chatgpt.com/) (the free version is still useful).  
	ChatGPT 至少有一个选项卡（免费版本仍然有用）。
- At least one tab for [Perplexity AI](https://www.perplexity.ai/), especially good for research-heavy questions.  
	Perplexity AI 至少有一个选项卡，特别适合研究繁重的问题。
- At least one tab for [Deepseek](https://chat.deepseek.com/) (v3 and r1 are free on their web interface, though watch the context limit).  
	Deepseek 至少有一个选项卡（v3 和 r1 在其 Web 界面上是免费的，但请注意上下文限制）。
- One tab for [Grok.com](https://grok.com/). Good, free and seemingly unlimited for general use and deep research/image editing. I mainly use the deep research feature, similar to perplexity.  
	一个选项卡用于 Grok.com。很好，免费，似乎无限制，适合一般用途和深度研究/图像编辑。我主要使用深度研究功能，类似于困惑。
- [Phind](https://phind.com/) is another free one, it tries to show you flowcharts/diagram visuals.  
	Phind 是另一个免费的，它试图向您展示流程图/图表视觉效果。
- [lmarena.ai](https://lmarena.ai/) offers free access to Claude Opus 4 and Sonnet 4 and others. Free Opus 4 is so good.  
	lmarena.ai 提供对 Claude Opus 4 和 Sonnet 4 等的免费访问。免费作品 4 太好了。

[Claude.ai](https://claude.ai/new) - Free but sometimes so limited it's annoying to use, so I use other sites/ways to access Claude like Cody extension, Copilot, etc.  
Claude.ai - 免费，但有时非常有限，使用起来很烦人，所以我使用其他网站/方式来访问 Claude，例如 Cody 扩展、Copilot 等。

Grok offers free compute and uncensored image generation, which can be useful when other models' safety systems interfere with legitimate tasks. However, reports indicate that Grok has been instructed to lie about about some things. While the misinformation appears to be mostly on X, if you keep in mind to restrict usage to coding or be cautious knowing it might be programmed with questionable motives, it can occasionally be useful. It was never that great though but its sometimes okay.

## A smarter, cheaper workflow: Focused Context更智能、更便宜的工作流程：聚焦上下文

When you use AI in web chat's (the chat interfaces like AI Studio, ChatGPT, Openrouter, instead of thru an IDE or agent framework) are almost always better at solving problems, and coming up with solutions compared to the agents like Cline, Trae, Copilot.. Not always, but usually.  
当您在网络聊天中使用 AI 时（AI Studio、ChatGPT、Openrouter 等聊天界面，而不是通过 IDE 或代理框架）几乎总是更擅长解决问题并提出解决方案，与 Cline、Trae、Copilot 等代理相比。并非总是，但通常如此。

When you use things like Cursor, Cline, Roo Code for everything, they are sending tons of text to the AI about how to use their tools, how to use or activate MCP server stuff, edit files, etc it "dumbs it down" too much. It gets confused. People end up paying for the most expensive best models to do everything and even that isn't enough to get over the dumbing down effect from the AIs getting tons of unneeded information unrelated to your problem.  
当你对所有内容使用 Cursor、Cline、Roo Code 之类的东西时，他们会向 AI 发送大量关于如何使用他们的工具、如何使用或激活 MCP 服务器的东西、编辑文件等的文本，它“愚蠢”太多了。它变得混乱。人们最终会花钱购买最昂贵的最佳模型来做所有事情，即使这样也不足以克服人工智能获取大量与您的问题无关的不需要的信息的哑巴效应。

So when that happens, I use my tool to generate the right context to solve my problem. Then I paste it into one of the many AI web chat's (sometimes more than one, since they sometimes give different answers) and just ask it questions or ask it to code review, to try to figure out why x is happening when y is happening...etc then when it figures out a solution.. i have it write a prompt for Cline or another agent type thing to do the actual file edits. GPT 4.1 can handle this just fine and I have unlimited. No reason to be wasting Claude credits to edit files. No reason to be sending Claude a bunch of crap it doesn't need making it dumb. I can use Claude to plan out anything or fix really hard problems, cheap, using Openrouter web chat then just paste it back in Cline and let it run.

After doing this for a while, you really get a feel for which models excel at which types of tasks.

**How AI Code Prep Helps (Example Prompt Structure):**

*Can you help me figure out why my program does x instead of y?*

Then, [AI Code Prep GUI](https://wuu73.org/aicp) (for Windows, Mac, Linux, and web) steps in. It recursively scans your project folder (subfolders, sub-subfolders, you name it) and grabs the code, formatting it nicely for AI like this:

The context block generated by AI Code Prep looks like this:

Can you help me figure out why my program does x instead of y?

fileName.js:  
<code>  
... the contents of the file..  
</code>  
  
nextFile.py:  
<code>  
import example  
...etc  
</code>

Can you help me figure out why my program does x instead of y?

It writes it twice if you have that option enabled, which helps get the AI to focus better on your question/prompt. You can choose to have it on top, bottom, or both. OpenAI claims this helps, I haven't really tested to see if that's true but it seems logical.

On Windows, you just right-click somewhere inside your project folder (or on the folder itself) and select "AI Code Prep GUI" from the context menu (look at the screenshots on the site). A GUI window pops up, usually with the right code files pre-selected. It smartly tries to skip things you likely don't need, like `node_modules`, `.git`, etc. If its guess isn't perfect, you can easily check or uncheck files.

This is super useful when your project is huge and blows past an AI's context limit. You can manually curate exactly what the AI needs to see.

The problem with many coding agents like [Cline](https://cline.bot/), Github Copilot, Cursor, Windsurf, etc., is that they often send either WAY too much context or WAY too little. This is why they can seem dumb or ineffective sometimes. Sometimes, you just gotta do things yourself, use a tool like mine to select the files yourself, but it helps auto-select the code files while skipping the stuff you probably don't need (but still have the option to add what you want with the checkboxes) and then dump that curated context into several AIs (especially the free web ones!).

There are other context-generating tools, but many are command-line only, or need a public GitHub repo link. What if your code is private? What if you want to keep it local? What if you prefer checkboxes on a GUI? For something like this a GUI makes sense. It has some other things I haven't seen anywhere else like the preset buttons, dual placement of problem/prompt, per-project saves.

**See my attempt to explain (auto-opens when in view)**

![Explanation diagram](https://wuu73.org/aicp/scrs/ar.png)