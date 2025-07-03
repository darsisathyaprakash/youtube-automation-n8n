# YouTube Automation with n8n (My Learning Journey)

## 📌 Overview

This is my personal project where I built a **YouTube content automation system** using `n8n`, OpenAI, and an AI video generator called **MCP server**.

The idea was to generate short videos automatically based on AI-generated scripts and optionally upload them to YouTube.

---

## 🧠 What I Learned

I started this project to learn **AI automation**, **n8n workflow building**, and how to connect APIs like OpenAI and MCP.

Here’s what I learned:
- How to use **Function Nodes** and **HTTP Requests** in n8n
- Posting JSON data to video generation APIs like MCP
- Handling delays and using **Wait Nodes**
- Downloading videos programmatically
- Troubleshooting errors like quota issues and bad requests

---

## ⚙️ What the Workflow Does

1. Starts with a **Schedule Trigger** or manual run
2. Sends a prompt to OpenAI to generate a script
3. Passes that script to a second agent to convert into a video prompt
4. Sends a POST request to **MCP server** to generate a video
5. Waits until the video is ready
6. Downloads the video
7. (Optional) Uploads to YouTube (part not implemented due to limitations)

---

## 🚧 Challenges I Faced

- OpenAI quota issues (Insufficient quota, invalid keys)
- Gemini API errors and model compatibility
- MCP video taking longer than expected
- File download errors and wrong video mapping
- Understanding how to parse JSON responses correctly

---

## 🧰 Stack Used

- **n8n** (self-hosted, local)
- **OpenAI API** (GPT-4.0 and mini)
- **MCP video server** (Docker)
- (Planned) YouTube Data API

---

## 📁 Files

- `youtube_automation.json` → The complete n8n workflow
- `README.md` → This file

---

## 🔄 Future Improvements

- Fix YouTube upload using OAuth2 and YouTube Data API
- Add better prompt generation and personalization
- Auto-thumbnail and title generator using AI
- Add Airtable or Google Sheet log

---

## 🙋 About Me

I’m **Sathya Prakash Darsi**, currently learning **AI automation** and **workflow tools like n8n**. I built this project to explore what’s possible with open tools without relying on expensive APIs.

📬 [My Portfolio](https://sathya-protfilo-web.netlify.app)

[🎥 Click to watch demo video](images/Recording%202025-07-02%20112543.mp4)
## 🎥 Demo - Website Monitoring with n8n

Web development is rapidly evolving — now with the rise of LLMs and automation, even websites can be monitored, maintained, and even built using AI tools.  
Watch how this no-code **Website Monitoring System** built with **n8n** can send Gmail alerts when your site goes down.

[![Watch the demo video](images/demo-thumbnail.png)](https://drive.google.com/file/d/1tNGVxUTpx0D8uO9SnCn2m6ZEDkUz1EAz/view?usp=sharing)

> 🔗 Click the image above to watch the screen recording.



---

## 💡 Tip for Others

Don’t be afraid to try, break, fix, and learn. I made **tons of mistakes**, got stuck on errors—but that’s how I figured out how to automate things using n8n!

