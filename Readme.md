📘 Project Overview

This project turns YouTube learning content into structured written summaries.
It uses a coordinated system of research and writing agents that work together to find a relevant video, extract its key points, and produce a blog-ready writeup — all in one automated flow.

🎯 Goal

To save time for people who want the essence of a YouTube lecture, tutorial, or tech talk in written form without watching the full video.

⚙️ How It Works

YouTube Tool – Targets a specific channel and searches for the most relevant video based on the given topic.

Researcher Agent – Gathers the transcript and identifies important concepts, examples, and takeaways.

Writer Agent – Transforms those findings into a concise, well-structured blog post.

Crew Orchestration – Runs the process step-by-step, passing context between agents to maintain consistency and clarity.

🧩 Main Components

tools.py — Handles YouTube channel search setup.

agents.py — Defines the roles, goals, and behaviors of the Researcher and Writer.

tasks.py — Assigns what each agent needs to accomplish and what the output should look like.

main.py — Combines all parts into a single executable flow.

🚀 Highlights

Sequential multi-agent execution using CrewAI.

Each task is modular, so it’s easy to replace or extend the agents or tools.

Environment variables manage API keys and model settings securely.

Supports caching and memory for improved performance and context retention.

💡 Example

If you set the topic to “MIT Introduction to Deep Learning”, the researcher finds that video, extracts key explanations from the transcript, and the writer produces a short blog article summarizing the main ideas — from introduction to key concepts and closing thoughts.
