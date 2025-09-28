---
title: My AI Code Prep & Cline Workflow for Budget Coding/Debugging (Part 3)
source: https://wuu73.org/blog/aiguide3.html
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

## TL;DR: Quickstart GuideTL;DR：快速入门指南

- **Models & Roles:**
	- Planning & Brainstorming: GLM 4.5, Kimi K2, the newest Qwen3 Coder and 2507's, Gemini 2.5 Pro (AI Studio), o4-mini (OpenRouter), Claude 3.7 or 4 (Poe), if you have OpenAI Playground configured for the 250k free daily tokens, I recommend using those up with o3 and GPT 5.  
		规划和头脑风暴：GLM 4.5、Kimi K2、最新的 Qwen3 Coder 和 2507、Gemini 2.5 Pro （AI Studio）、o4-mini （OpenRouter）、Claude 3.7 或 4 （Poe），如果您为 OpenAI Playground 配置了 250k 免费每日代币，我建议将它们与 o3 和 GPT 5 一起使用。
	- Problem Solving & Debugging: GPT-5 (free tokens in Playground), GLM-4.5 (it seems to be a genius, about Claude 4 level) Claude 4 (free daily on Poe)  
		问题解决和调试：GPT-5（Playground 中的免费代币）、GLM-4.5（似乎是天才，大约是 Claude 4 级别）、Claude 4（Poe 上每天免费）
	- Actual Coding: GPT-4.1 via Cline; fallback to Claude 3.5.. or the new ones: Qwen3 Coder, Instruct, 2507, GLM 4.5, Kimi K2.  
		实际编码：GPT-4.1 通过 Cline;回退到 Claude 3.5。或新的：Qwen3 Coder、Instruct、2507、GLM 4.5、Kimi K2。
- **Key Tools:**
	- VS Code VS 代码
	- AI Code Prep GUI – locally scan & curate only the files you need, saves so much time  
		[[AI]] 代码准备 GUI – 本地扫描和仅整理您需要的文件，节省大量时间
	- Cline (VS Code agent) for step-by-step code execution  
		Cline（VS Code 代理）用于逐步执行代码
	- Free web chats for multi-perspective advice: Poe.com, ChatGPT, Grok, Deepseek, Perplexity, OpenAI Playground, AI Studio w/Gemini 2.5 Pro, Openrouter, duck.ai  
		免费网络聊天，提供多角度建议：Poe.com、ChatGPT、Grok、Deepseek、Perplexity、OpenAI Playground、带 Gemini 2.5 Pro 的 AI Studio、Openrouter duck.ai
- **Quick Workflow:**
	1. Run AI Code Prep GUI to bundle your (if already existing) project’s relevant files.  
		运行 AI Code Prep GUI 以捆绑您的（如果已存在）项目的相关文件。
	2. Paste that context into your favorite web chat models for planning & debugging.  
		将该上下文粘贴到您最喜欢的网络聊天模型中，以进行规划和调试。
	3. Ask one model to “Write me a detailed Cline prompt for these tasks,” then refine it (e.g. in ChatGPT).  
		要求一个模型“为我写一个详细的 Cline 提示来处理这些任务”，然后对其进行优化（例如在 ChatGPT 中）。
	4. Copy/paste into Cline set to GPT-4.1 to generate or fix code; if it stalls, switch to Claude 3.5.  
		复制/粘贴到设置为 GPT-4.1 的 Cline 中以生成或修复代码;如果它停滞不前，请切换到 Claude 3.5。
- **Cost-Saving Hacks:**
	- Enable “share data” in OpenAI Playground for 250k free GPT-4.5, o3, (both genius expensive models) & 2.5 MILLION free tokens/day for o4-mini, o3-mini!!  
		在 OpenAI Playground 中启用“共享数据”，每天可获得 250k 免费 GPT-4.5、o3（均为天才昂贵模型）和 250 万个免费代币，适用于 o4-mini、o3-mini！
	- $10/mo GitHub Copilot subscription gives you rate-limited access to Claude models via Cline  
		10 美元/月 GitHub Copilot 订阅让您可以通过 Cline 限速访问 Claude 模型
	- Pay-as-you-go on OpenRouter for o4-mini, Claude 3.7, and other new models  
		在 OpenRouter 上为 o4-mini、Claude 3.7 和其他新型号提供即用即付

## Note about some free CLI agent tools关于一些免费的 CLI 代理工具的注意事项

Currently as of end of August 2025, Qwen Code (using the GREAT Qwen3 Coder 480b model!) is totally free, 1000-2000 requests a day (I have not run into limits with heavy use). It is an agentic tool that runs in the terminal, but you can also 'borrow' the API key to use in anything. Kilo Code currently has it set up automatically, just choose the Qwen provider. Gemini CLI is also free with high limits but I have heard about getting limited fast. Claude Code is currently said to be the best CLI tool, but it really eats tokens if you aren't getting them for free. Claude Code Router, a free repo on github, allows you to use whatever API you want for Claude Code. OpenCode.ai is another one, it allows me to use my unlimited GPT 4.1 from the $10/month co-pilot subcription. I still have not found that any of these are as good as doing it my way where I use [AI Code Prep GUI](https://wuu73.org/aicp) to plan with models on their native web chat's, then implement with GPT 4.1. Maybe I should try to create my own agentic tool, that separates things so that difficult problems are sent to the smartest AIs without the tools, MCPs, emulating this way of doing it, then send to smaller model for coding.  
目前截至 2025 年 8 月底，Qwen Code（使用 GREAT Qwen3 Coder 480b 型号）是完全免费的，每天 1000-2000 个请求（我没有在大量使用时遇到限制）。它是在终端中运行的代理工具，但您也可以“借用”API 密钥以用于任何内容。Kilo Code 目前已自动设置，只需选择 Qwen 提供商即可。Gemini CLI 也是免费的，但限制很高，但我听说过快速受到限制。Claude Code 目前据说是最好的 CLI 工具，但如果你不免费获得它们，它真的会吃掉代币。Claude Code Router 是 github 上的一个免费存储库，允许您为 Claude Code 使用任何您想要的 API。OpenCode.ai 是另一个，它允许我从每月 4.1 美元的副驾驶订阅中使用我的无限 GPT 10。我仍然没有发现其中任何一个都像我使用 AI Code Prep GUI 在模型的本机网络聊天中对模型进行规划，然后使用 GPT 4.1 实现的方式一样好。也许我应该尝试创建自己的代理工具，将事物分开，以便将困难的问题发送给最聪明的 AI，而无需模拟这种方法的工具 MCP，然后发送到较小的模型进行编码。

## Latest Model Updates (Aug 2025)最新型号更新（2025 年 8 月）

#### GPT 4.5

This model was discontinued.  
该型号已停产。

#### o3

Possibly equal to Claude 4 in abilities, really great at fixing hard problems, genius level. Throw your entire codebase in here with [AI Code Prep GUI](https://wuu73.org/aicp)  
能力可能与克劳德4相当，非常擅长解决难题，天才水平。使用 AI Code Prep GUI 将您的整个代码库放入此处

**Free Tokens:** 250k daily when you enable data sharing in [Data Controls/Sharing settings](https://platform.openai.com/settings/organization/data-controls/sharing)  
免费代币：每天 250k 当您在数据控制/共享设置中启用数据共享时

#### o4-mini O4-迷你

Not as smart as o3, but very very good, like o3's younger brother  
没有o3聪明，但非常非常好，像o3的弟弟

**Free Tokens:** 2.5 million daily when you enable data sharing in [Data Controls/Sharing settings](https://platform.openai.com/settings/organization/data-controls/sharing)  
免费令牌：在数据控制/共享设置中启用数据共享时，每天 250 万个

#### Gemini 2.5 Pro 双子座 2.5 Pro

Free to use in [AI Studio](https://aistudio.google.com/). Also very good at fixing hard problems  
在 AI Studio 中免费使用。也非常擅长解决难题

**Best For:** Complex debugging and architectural planning

#### Deepseek R1 0528

Super smart model with enhanced reasoning capabilities

**Availability:** Free on Deepseek's web interface

#### Claude 4 Sonnet

The mega genius, can fix most problems in one shot if you provide enough context ([AICodePrep is what I use](https://wuu73.org/aicp)). These also seem to be the best writers, best at everything really.. the secret sauce

**Use Case:** When you absolutely need it fixed right the first time

#### Claude 4 Opus

$75 per million tokens, haven't tried it yet myself but I hear its a super mega genius like Sonnet but even better, magic sauce

**Performance:** Rumored to be the ultimate problem solver

## Solid Worker Models

These models listen to instructions really well and do as they are told:

#### GPT 4.1

Use the above smarter models for abstract high level design or to fix problems, then 4.1 to make changes. You can cut and paste output from anywhere else right into Cline with 4.1 to do the coding.

#### Claude Sonnet 3.5

Good solid model for coding and editing, slightly slower vs 4.1 but very reliable.

#### Deepseek v3

Pretty good and very cheap for a model that can do edits/code/agent work.

#### OpenRouter Free Models

Drag the price filter to $0 on [OpenRouter](https://openrouter.ai/) to see free models available for testing. Worth experimenting with new ones as they become available.

## Free Claude 4: lmarena.ai, and More

#### Claude Opus 4 and lmarena.ai

[lmarena.ai](https://lmarena.ai/) offers free access to Claude Opus 4 and Sonnet 4 and others.

Any free usage of anything by Anthropic is worth saving, remembering, and using. When all else fails, or when you need to get stuff done, perfectly, and now, choose Claude 4 Sonnet or Opus.

### Latest Model Updates (2025)

#### Claude Sonnet 4 & Opus 4

**Status:** Just released and proving to be the best models for everything

**Performance:** Fixed some bugs today that were hard for most other models to handle

**Cost:** More expensive, but accessible through GitHub Copilot $10/month (rate limited)

**GitHub Copilot Value:** The cheap $10/mo GitHub Copilot subscription seems to be giving me a very generous amount of Claude 4 uses through the VS Code LM API. I keep using it as my main model in Cline/Roo Code, and it has not run out yet. I either use GPT 4.1 or Claude 4, been waiting for it to limit me but it hasn't yet (they say that GPT 4.1 is unlimited). I always hate subscriptions for anything, but this particular one is insanely good value.

**Strategy:** Save Claude 4 for tough problems, use GPT 4.1 for regular coding

#### GPT 4.5

**Performance:** Excellent for bug fixing and complex problem solving

**Token Limits:** 250k tokens daily if you allow data for model training

**Cost Hack:** Free under the 250k token limit when you enable data sharing in settings

**Use Case:** Great for using AI Code Prep tool to analyze entire codebases

## NEW!! Bad ass new Chinese models + GPT 5

#### GLM 4.5

Very much like Claude 4 Opus or Sonnet; follows agentic rules and uses tools near perfectly. Fixes really hard bugs and handles complicated tasks with lots of context.

#### Qwen3 Coder 480B

Another super great one; a favorite for being powerful and cheap.

#### Qwen3 Instruct & Thinking 2507

Similar to Qwen3 Coder—strong, dependable, and cost-effective.

#### Kimi K2 (Moonshot)

Feels Anthropic-inspired or trained on Claude-like synthetic data. Really good; used a lot.

#### GPT-5

\*\*edit\*\* -- OpenAI has vastly improved GPT-5 since I wrote this and it is actually pretty decent at tools now....but the first week was bad which is when i wrote this: Not very good at custom tool usage (e.g., your own tools/MCP/Cline). Better to plan and fix like this guide suggests using GPT 5 and other insanely great models like GLM 4.5, then have it write a prompt for a simpler agent model to do actual editing and tool usage. GPT 4.1 still wins on value, and the new Chinese models handle custom tools/Cline easily. I have not played around with this one yet to know if its good but usually all models are going to be great at certain things. I am honestly more excited about the Chinese models, because of cost and the experiences so far have proven them to be reliably great pretty much all the time.

### Current Coding Workflows that I use (2025)

#### For New Projects:

1. **Planning Phase:** Type your idea(s) and ask several AI's in web chat's to brainstorm with you and help you figure out a real plan, into notepad or a blank file. - this is just so you can paste into multiple web chat's
2. **Multi-Model Consultation:** Paste into two or three of these models web chat's for different "doctor's opinions":
	- Gemini 2.5 Pro (free)
	- GLM 4.5 (free and unlimited!)
	- Qwen3-Coder or one of the -2507 models
	- o4-mini on OpenAI Playground to use the free 2.5mil daily tokens
	- Claude 4 on Poe.com (free daily credits)
3. **Refinement:** Go back and forth to fine-tune details
4. **Task Generation:** Have model write a PRD (Product Requirements Document) markdown file or similar, like "APP\_REQUIREMENTS.md" or website requirements etc with a list of all the things it must have. Then have it write step-by-step task list with subtasks, for an AI coding agent to implement. Save this to a new project folder - and you might want to run 'git init' if you use Git.
5. **Execution:** Copy/paste into Cline (or just tell it "your task is in the project requirements.md file") set to GPT 4.1 for 'act' mode (or Qwen 3 Coder, GLM 4.5 Flash.. also free currently and excellent). If you prompt the web models to break a big project into small enough sub-tasks, then you can get away with using a cheaper implementation/agent model. "Cheap" right now for me is GPT 4.1 using the Github Copilot API (I don't even use the actual copilot much I just like the unlimited 4.1 - also every month you get credits to use all the top expensive models like Opus/Sonnet 4 which are great for top level planning, you can also use copilot's own web chat interface)

#### For Problem Solving, fixing hard bugs:

1. Load AI Code Prep GUI tool (type 'aicp' in terminal) and type the problem into the prompt box, look at which files are already selected to make sure that it looks good for context (when in doubt, add more code files, usually it helps)
2. Set the options to 'Add prompt to top' and ''..bottom' is usually how i leave that setting.. it seems like it would be wasteful but it seems to help focus the model on the problem better than only having the prompt on top or bottom
3. If I am confident that it will be able to fix my problem I will click one of the preset buttons for Cline/Roo Code or one for an agent prompt which just pastes some extra text to the end of the current text in the prompt box, telling the AI to write a solution for an agent to implement the changes (experimenting with this will be the easiest way to understand what it is for - it just saves you from typing that)
4. Click the "GENERATE CONTEXT!" button, and if its a hard problem.. i'll paste it into Gemini 2.5 Pro, GLM 4.5, Kimi K2, Qwen3 Coder or 2507 Thinking.. all on their native web chat website (Qwen has an annoying web chat where it pastes it into a file so you have to tell it to read the file)
5. Sit back and watch several solutions stream in, bathroom break. Using several AI's from several different companies is a great way to get some diversity in the outputs and it is better than for example.. just using 5 OpenAI models or just using Anthropic's models. It reminds me of how people will have healthier kids if they mate with people from different cultures/different parts of the world. It just produces a faster / better solution. You can even cut and paste the outputs of all of these into Gemini 2.5 Pro (its got such a large context window to handle it) and have AI again compare them all and produce a final "best of all" solution.
6. Problem solving like this will often "one shot" a perfect solution, instead of letting agents run around your file system trying to slowly figure out solutions with all the tools and MCPs and other stuff it is often just faster to do it this way!

### Task List & Test Driven Development (Coming Soon)

**Test Driven Development & Task Lists:**

Coming to this guide soon (these other topics)Have the AIs create a detailed task list for Cline, Roo Code, Trae agent, to execute. You can also instruct Cline or Roo Code to use a markdown file to keep track of everything it does, checking things off as it completes them. This will make it easier to track and ensure nothing gets missed.

For now, you can experiment by having a model generate a checklist in markdown, and then ask Cline or Roo Code to update the file as tasks are completed.

### Money-Saving Hacks

- **GLM 4.5, Kimi K2, o3:** 250k tokens free daily by enabling data sharing for model training
- **Cheaper Models:** 2.5 million tokens on o4-mini (excellent model), 4.1-mini/nano, GPT 5 Mini
- **GitHub Copilot:** $10/month gives access to new Claude models (rate limited) and GPT 4.1 UNLIMITED for agent work
- Qwen3 has new models Coder and 2507's
- **Poe.com:** Free daily credits for every type of model
- **Web Interfaces:** Use free web chat interfaces for planning and consultation

### Coming Soon: Live Reddit Data & Insights

**Live Reddit Data Scraping & Daily Insights:**

A new feature is coming soon: live scraping of Reddit data and daily updated info about how people are using AI models. This will include detailed usage breakdowns, data visualizations, and new insights into real-world coding workflows and trends.

If you buy the Pro version of [aicodeprep-gui](https://tombrothers.gumroad.com/l/zthvs), you will get updated content about more free stuff, free api's, updated model information, any new cost hacks I discover but updated more frequently