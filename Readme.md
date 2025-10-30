# CrewAI: YouTube → Blog Generator

Multi-agent pipeline that:

1. Searches a target YouTube channel for the best video on a topic.
2. Extracts the transcription and key points.
3. Writes a concise, blog-ready summary.

## Why This Exists

You have good technical videos. You don’t always have time to turn them into written posts. This repo automates research and writing using CrewAI agents that collaborate like a small editorial team — one doing the research, the other crafting the narrative.

## What This Project Does

This project demonstrates how **CrewAI** can coordinate multiple intelligent agents to transform unstructured YouTube video content into structured blog posts.
It uses a **YouTube search tool**, **memory sharing**, and **sequential task execution** to replicate the human workflow of researching, summarizing, and writing.

### Step-by-step Workflow

1. **User gives a topic** — e.g., “MIT Introduction to Deep Learning.”
2. The **Research Agent** uses the YouTubeChannelSearchTool to locate relevant videos on that topic from the specified channel.
3. It extracts detailed transcriptions and identifies the core ideas, definitions, and insights.
4. The **Writer Agent** then summarizes the findings into a clear, engaging blog post.
5. The **Crew** orchestrates both agents sequentially, ensuring consistency and shared context across tasks.

## How It Works

* **Tools**: `YoutubeChannelSearchTool` scoped to one channel (configurable via `.env`).
* **Agents**:

  * **Researcher** – finds and analyzes the most relevant video and extracts key insights.
  * **Writer** – converts those insights into a short, clear, readable blog post.
* **Process**: Sequential task execution with memory and caching enabled, so both agents share context efficiently.

---

