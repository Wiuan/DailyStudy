---
title: My AI Code Prep & Cline Workflow for Budget Coding/Debugging (Part 2)
source: https://wuu73.org/blog/aiguide2.html
author: "[[wuu73]]"
published:
created: 2025-09-28
description: A personal guide on using AI Code Prep GUI, Cline, and various free AI web interfaces like Gemini, Grok, Deepseek, and Poe for cost-effective coding and debugging.
tags:
  - clippings
type: webpage
domain: wuu73.org
---
[Visit wuu73.org](https://wuu73.org/)

Last updated: July 2025

## Model Strategy: Picking the Right Brain for the Job模型策略：为工作选择合适的大脑

Since many great models are free to use via web interfaces (like Gemini in [AI Studio](https://aistudio.google.com/), [Grok](https://grok.com/), [Deepseek](https://chat.deepseek.com/)), I prioritize these. [Poe.com](https://poe.com/) also gives free daily credits for top models like Claude and the new o4 series.  
由于许多出色的模型都可以通过 Web 界面免费使用（例如 [[AI]] Studio 中的 Gemini、Grok、Deepseek），因此我优先考虑这些模型。Poe.com 还为 Claude 和新 o4 系列等顶级型号提供免费的每日积分。

**Gemini 2.5 Pro** (via [AI Studio](https://aistudio.google.com/)) is great for debugging, great for planning, and also finding it the best at lots of things now. For really thorny issues, I might try the new **o4-mini** (available via [OpenRouter](https://openrouter.ai/) or [Poe](https://poe.com/)). It surprisingly fixed a persistent bug for me right away, though I'm still figuring out its best use cases. It's notably cheaper via API than the previous top dogs like Claude 3.5/3.7/4.  
Gemini 2.5 Pro（通过 AI Studio）非常适合调试，非常适合规划，并且发现它现在在很多事情上都是最好的。对于非常棘手的问题，我可能会尝试新的 o4-mini（可通过 OpenRouter 或 Poe 获得）。令人惊讶的是，它立即为我修复了一个持续存在的错误，尽管我仍在找出它的最佳用例。通过 API 的它比之前的顶级狗（如 Claude 3.5/3.7/4）便宜得多。

I usually try **Claude 3.7 or 4** at some point, via [Poe](https://poe.com/) or API ([OpenRouter](https://openrouter.ai/) makes this easy), or github Copilot chat (you can get some free usage from that if you don't pay) but it's pricier for frequent use. Think of Claude 3.7 and 4 as Claude on Adderall – brilliant, sometimes verbose, maybe a bit 'psychotic' like Hunter S. Thompson. Lots of great output, but you might need a calmer model like **Claude 3.5** to refine it or do the actual coding.  
我通常会在某个时候尝试 Claude 3.7 或 4，通过 Poe 或 API（OpenRouter 使这变得容易），或 github Copilot 聊天（如果你不付费，你可以从中获得一些免费使用），但经常使用会更贵。将 Claude 3.7 和 4 想象成 Adderall 上的 Claude——才华横溢，有时冗长，也许有点像 Hunter S. Thompson 一样“精神病”。很多很棒的输出，但你可能需要一个更平静的模型，比如 Claude 3.5 来完善它或进行实际编码。

**Gemini 2.5 Pro** (via [AI Studio](https://aistudio.google.com/)) is great for debugging, great for planning, and also finding it the best at lots of things now. The new **Gemini 2.5 Pro** model shows even better performance across coding tasks. For really thorny issues, I might try the new **o4-mini** (available via [OpenRouter](https://openrouter.ai/) or [Poe](https://poe.com/)). It surprisingly fixed a persistent bug for me right away, though I'm still figuring out its best use cases. It's notably cheaper via API than the previous top dogs like Claude 3.5/3.7.  
Gemini 2.5 Pro（通过 AI Studio）非常适合调试，非常适合规划，并且发现它现在在很多事情上都是最好的。新的 Gemini 2.5 Pro 型号在编码任务中表现出更好的性能。对于非常棘手的问题，我可能会尝试新的 o4-mini（可通过 OpenRouter 或 Poe 获得）。令人惊讶的是，它立即为我修复了一个持续存在的错误，尽管我仍在找出它的最佳用例。它通过 API 明显比之前的顶级狗（如 Claude 3.5/3.7）便宜。

For really hard problems, try using OpenAI's o3 or GLM 4.5, Qwen3 Coder 480b. You can get lots of free daily tokens if you set your account to allow sharing of your data to help train models. Go to the Open AI Playground page, click the settings icon in the upper right, then click Data Controls on the left sidebar, then Sharing on the displayed page, there you can change the "Share inputs and outputs with OpenAI" setting to Enabled, which will give you:  
对于非常困难的问题，请尝试使用 OpenAI 的 o3 或 GLM 4.5、Qwen3 Coder 480b。如果您将帐户设置为允许共享数据以帮助训练模型，则可以获得大量免费的每日代币。转到“打开 AI Playground”页面，单击右上角的设置图标，然后单击左侧边栏上的“数据控件”，然后单击显示页面上的“共享”，在那里您可以将“与 OpenAI 共享输入和输出”设置更改为“已启用”，这将为您提供：

- Up to 250 thousand tokens per day across gpt-5, gpt-4.1, gpt-4o, o1 and o3  
	每天多达 25 万个代币，涵盖 gpt-5、gpt-4.1、gpt-4o、o1 和 o3
- Up to 2.5 million tokens per day across gpt-4.1-mini, gpt-4.1-nano, gpt-4o-mini, o1-mini, o3-mini, o4-mini, and codex-mini-latest  
	每天多达 250 万个代币，涵盖 gpt-4.1-mini、gpt-4.1-nano、gpt-4o-mini、o1-mini、o3-mini、o4-mini 和 codex-mini-latest

This is really awesome, o3 and GPT 4.5 seem super genius! Sometimes in the OpenAI Playground, I have it set up to use o3 and o4-mini side-by-side, to compare them. This helps me get a feel for which ones are best for which types of problems.  
这真是太牛了，o3和GPT 4.5看起来超级天才！有时在 OpenAI Playground 中，我将其设置为并排使用 o3 和 o4-mini 来比较它们。这有助于我了解哪些最适合哪些类型的问题。

**Claude 4 and 3.7** is always a good option to try and fix hard problems quickly, it is just harder to access it for cheap or free. But it is often the best out of them all. When you really need to fix something fast, use it. [Poe](https://poe.com/) has free tokens for all models, daily. [OpenRouter](https://openrouter.ai/) has all models paid and/or free. Claude 3.7 is Claude on caffeine – brilliant, sometimes verbose, maybe a bit 'psychotic' like Hunter S. Thompson. Lots of great output, but you might need a calmer model like **Claude 3.5 / 4** to refine it or do the actual coding.  
Claude 4 和 3.7 始终是尝试快速解决难题的不错选择，只是更难以便宜或免费的方式访问它。但它通常是其中最好的。当您确实需要快速修复某些内容时，请使用它。Poe 每天为所有型号提供免费代币。OpenRouter 提供所有型号付费和/或免费。Claude 3.7 是咖啡因的 Claude——才华横溢，有时冗长，可能像 Hunter S. Thompson 一样有点“精神病”。很多很棒的输出，但您可能需要一个更平静的模型，比如 Claude 3.5 / 4 来完善它或进行实际编码。

## The Hybrid Approach: Premium Planning + Budget Execution

After extensive testing with various models, I've developed a hybrid strategy that maximizes both quality and cost-effectiveness. The key insight is that different models excel at different parts of the development process.

## My "smart juice" theory of model intelligence - How Models become stupid under certain circumstances

AI models are usually smarter the less text you send to them. Think of each model as having a fixed amount of "intelligence" or "smart juice" available for every question or problem you ask. When you send a simple, focused prompt, nearly 100% of that intelligence is available to solve your problem. But the more complex your input—long agentic instructions about how to use tools, lots of context unrelated to your specific problem, or multiple pages of code—the more of that "smart juice" gets used up just processing the unrelated stuff like how it can use tools in your IDE, leaving less intelligence energy available for your actual problem.

This is why tools like Cursor, Cline, and other agentic systems can sometimes seem less effective: if they send five giant pages of instructions and context before even getting to your real question, the model's available intelligence for your specific problem drops. The more "stuff" you send, the more diluted the model's focus becomes. For best results, keep your prompts as concise and targeted as possible—curate the context so the model can use its full intelligence on what matters most.

When you have a hard problem or bug, you will usually save time by using AI Code Prep to dump it into a web chat (as discussed on page 1 of this guide). It cuts out all the extra instructions and stuff that get sent in agentic IDEs/apps. I noticed that this works better even if you give the AI ALL of the files from your project. The agentic instructions/stuff/bloat that is unrelated to your actual problem is the content that seems to make the AI dumber/run out of juice.

**My Workflow is something like this when starting a new project:**

1. **Plan & Brainstorm:** Use the smarter/free web models (Gemini 2.5, o4-mini, Claude 3.7, 4, o3, etc) to figure out the approach, plan the steps, identify libraries, etc.
2. **Generate Agent Prompt:** Ask one of these smart models: "Write a detailed-enough prompt for [Cline](https://cline.bot/), my AI coding agent, to complete the following tasks: \[describe tasks\]". Sometimes, I'll copy this generated prompt and paste it into *another* free AI good at rewriting (like [ChatGPT](https://chatgpt.com/)) to refine it further.
3. **Execute with Cline:** Paste the step-by-step task list into [Cline](https://cline.bot/), configured to use a stable and efficient model like **GPT 4.1 or Claude 3.5** (or Claude 4 if it is doing really complicated things). The 4.1's have been trained to follow instructions well.
4. **Fallback:** If GPT 4.1 struggles, switch [Cline](https://cline.bot/) to use **Claude 3.5** via API. It seems to be the next best for reliable execution. [Deepseek v3 or R1](https://chat.deepseek.com/) is really great at following instructions as well.

Essentially: Use expensive/smart models (and the excellent free Gemini 2.5 Pro) to strategize and plan. Validate the plan by pasting it into 2-3 other free models ([Deepseek R1](https://chat.deepseek.com/), Claude on [Poe](https://poe.com/) if context allows) and ask "Is this good? Can you improve it or find flaws?". Then, use a stable workhorse like GPT 4.1 or Claude 3.5 within [Cline](https://cline.bot/) to do the heavy lifting (coding).

**o4-mini** seems particularly adept at untangling complex code logic or figuring out high-level implementation strategies (like choosing frameworks or libraries). I'll often throw my initial idea at Gemini 2.5, o4-mini, GPT 4.1, [ChatGPT](https://chatgpt.com/), maybe o3-mini (try [duck.ai](https://duckduckgo.com/chat) - often free), and [Phind](https://phind.com/) to get a range of ideas. If the free/cheap options don't crack it, I'll escalate to pricier models via API.

## Alternative Agents & Setups

[Trae.ai](https://trae.ai/) (from Bytedance, makers of TikTok) is a free VS Code compatible IDE with free AI usage, including Claude 4, Claude 3.7, Claude 3.5, and GPT 4.1. Their agents aren't as good as Cline (nothing is as good, to be honest!) but it's free and gives access to the best models. Sometimes, I find its built-in agent isn't as robust as [Cline](https://cline.bot/). However, since [Trae](https://trae.ai/) seems to be a VS Code clone, you can likely install the [Cline](https://cline.bot/) extension within it! However... it is too overloaded to get any free usage from it, its too slow. I'll still mention it though.. but meh.

So, you could have two setups:

- VS Code + [Cline](https://cline.bot/) extension + [Copilot](https://github.com/features/copilot) extension (get the $10/mo subscription for cheap API access via Cline, though the free tier might offer some basic use).
- [Trae.ai](https://trae.ai/) + [Cline](https://cline.bot/) extension (potentially leveraging Trae's free model access if Cline can use it, or using your own API keys).

Try both! Sometimes the native [Copilot](https://github.com/features/copilot) agent solves things [Cline](https://cline.bot/) struggles with, and vice-versa. I suspect [Cline](https://cline.bot/) sometimes sends overly large prompts which might hinder performance on certain tasks compared to the more integrated Copilot agent.

### Roo Code: Cline's Clone

#### Roo Code

Roo Code is a clone of Cline, very similar but with some different features that are worth trying out. Sometimes Cline might work better for your workflow, and sometimes Roo Code will. It's a good idea to try both and see which fits your needs for a given project or coding style.

[Cline](https://cline.bot/) for VS Code is free, but remember you pay for the API calls unless you're leveraging the [Copilot](https://github.com/features/copilot) subscription trick. Using the VS Code LM API setting in [Cline](https://cline.bot/) with a $10/month Copilot sub is currently the most cost-effective way to get near-unlimited access to powerful models within the agent.

#### New CLI Tools: Claude Code, Qwen Code, Gemini CLI

There’s a lot of buzz about new CLI tools for coding, especially **Claude Code**, **Qwen Code**, and **Gemini CLI**. People rave about Claude Code’s capabilities, though I haven’t tried it myself yet. When I do, I plan to set it up to use **GLM 4.5** instead (there’s a guide for this on the z.ai website).

Claude Code supports subagents—these are agents that only do one task and don’t use extra tools. This setup can mimic the streamlined workflow described in this guide, focusing the model’s intelligence on a single job. Subagents are a clever way to avoid the “bloat” of agentic instructions and keep things efficient.

If you want to experiment, check out the guides and community tips for configuring these tools. The ecosystem is evolving quickly, and each tool has its own strengths for different workflows.