# 🧠 Gemini AI Agent Crew with CrewAI

This project demonstrates how to build intelligent, collaborative AI agents using Google's Gemini models with [CrewAI](https://docs.crewai.com/). The system includes a **Senior Researcher** and a **Writer**, working together to generate compelling content on trending tech topics.

---

## 🚀 Features

- 🤖 Two autonomous agents:
  - `Senior Researcher`: Uncovers trends and insights in a given topic.
  - `Writer`: Crafts engaging, easy-to-read blog content.
- 🔍 Real-time web search with Serper.dev for up-to-date information (RAG-style).
- 📄 Outputs a Markdown blog article.
- 🔁 Sequential task execution.

---

## 🧱 Project Structure

gemini_agent/
├── agents.py         # Defines AI agents using Gemini LLM
├── crew.py           # Orchestrates tasks and agent workflow
├── tasks.py          # Defines what each agent needs to do
├── tools.py          # Sets up web-search tools (SerperDev)
├── .env              # Stores API keys and credentials
├── .gitignore        # Prevents sensitive files from being tracked
└── README.md         # You're reading it! 



🛠️ Setup
Clone this repo


git clone https://github.com/yourusername/gemini_agent.git
cd gemini_agent
Install dependencies


pip install -r requirements.txt
Set up your .env file
Create a .env file with:


GOOGLE_API_KEY=your_gemini_api_key
SERPER_API_KEY=your_serper_api_key
Run the crew!


python crew.py
🧠 How It Works
LLM Setup: Loads Google Gemini model using your API key.

Agents: Each AI agent has its own goal and personality (via agents.py).

Tools: Agents can access live web data via Serper.dev (like mini-RAG).

Tasks: Assigned goals like "Research latest AI in healthcare" and "Write a blog post."

Crew: Runs agents in sequence to generate final output.

📂 Sample Output
After running the code, a file named new-blog-post.md will be generated with a full-length article on your chosen topic.

