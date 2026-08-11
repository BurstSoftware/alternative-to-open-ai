# what services does the chatgpt ui offer the openai customer

If by “the ChatGPT UI” you mean what OpenAI is actually selling/providing to a customer through chatgpt.com or the ChatGPT apps, it's much more than a textbox connected to an LLM.

Think of ChatGPT as a customer-facing AI operating environment.

The main services exposed through the UI
Service	What the customer gets
AI chat	Conversation, writing, explanation, brainstorming, reasoning, coding
Web Search	Current information from the internet with citations
Deep Research	Multi-step web research that produces a documented report
File analysis	Upload PDFs, spreadsheets, presentations, images, etc. and analyze them
Data Analysis / Python	Calculations, data processing, charts, transformations
Image generation	Create and edit images from natural-language instructions
Vision	Understand photos, screenshots, diagrams, charts and other images
Voice	Speak naturally with ChatGPT and receive spoken responses
Memory	Personalization across conversations where enabled
Projects	Organize conversations, files and context around ongoing work
Custom GPTs	Create specialized versions of ChatGPT
Apps / integrations	Connect external tools and information sources to ChatGPT
Codex / Work	Delegate coding and other tasks to specialized agents/workflows
Library	Store and reuse uploaded/generated files

OpenAI's current capabilities documentation explicitly lists search, deep research, image input/generation and file uploads, while the current ChatGPT FAQ describes ChatGPT as supporting everyday work such as writing, studying, planning, math, coding, and analyzing images/files.

The really interesting part

These aren't necessarily separate AI models.

The UI acts more like an orchestrator:

                         CHATGPT UI
                             │
              ┌──────────────┼──────────────┐
              │              │              │
             Chat           Tools          Data
              │              │              │
              ▼              ▼              ▼
           GPT model     Web Search       Files
              │          Deep Research    Memory
              │          Python           Apps
              │          Images
              │          Voice
              │
              └──────────────┬──────────────┘
                             ▼
                       Final response

So when you ask:

“Analyze this Excel spreadsheet and tell me why sales dropped.”

ChatGPT may effectively coordinate several services:

UI → upload file → model → data-analysis/Python environment → model interprets results → response + charts

OpenAI specifically describes ChatGPT's file capability as allowing users to analyze spreadsheets, edit documents, summarize PDFs and work with images directly in a conversation.

Search is another service

If you ask:

“What happened in the stock market today?”

the model doesn't have to rely solely on its learned knowledge.

ChatGPT can invoke Search, retrieve current information, and produce an answer with citations. OpenAI distinguishes ordinary Search—which is intended for quick current information—from Deep Research, which performs multi-source investigation and synthesis.

Deep Research is basically an agentic service

This is significantly more than ordinary chat.

You give it:

“Compare the 10 largest AI companies and determine which has the strongest economics.”

It can:

Understand the objective
Create a research plan
Search sources
Read information
Continue searching
Synthesize the findings
Produce a structured report
Give you citations

OpenAI says you can review/modify its research plan, monitor progress, interrupt it, and ultimately receive a cited report that can be downloaded as Markdown, Word, or PDF.

Voice turns it into an interface rather than just a chatbot

With Voice, the service becomes:

microphone → speech processing → AI → response generation → speech

The current Voice system can maintain a natural conversation, and Live can use web search and memory and work with text and images in the same conversation.

Images are another compute service

You can say:

“Create a photorealistic image of a modern cabin beside a frozen lake.”

The ChatGPT UI sends that request to the image-generation system.

You can also upload an existing image and request edits. OpenAI's current Images documentation describes creation, editing, selection-based edits, aspect-ratio controls, and transparent backgrounds.

Apps are effectively an API layer inside the UI

This is particularly important for understanding the business.

ChatGPT can connect to external applications and data sources so that the AI can search, reference, and work with information outside OpenAI's own systems.

Conceptually:

                    ChatGPT
                       │
        ┌──────────────┼──────────────┐
        ▼              ▼              ▼
    OpenAI data     Your files    External apps
                                    │
                         ┌──────────┼─────────┐
                         ▼          ▼         ▼
                       Drive    Business DB   Other tools

That's a huge shift from:

“AI that answers questions”

to:

“AI that can interact with your information and software.”

So what is a ChatGPT customer actually buying?

I'd describe it as five layers:

1. Intelligence
Access to OpenAI's models.

2. Tools
Search, Python/data analysis, image generation, file processing, etc.

3. Context
Conversation history, memory, projects and uploaded files.

4. Agents/workflows
Deep Research, Codex, Work and other systems that can perform multi-step tasks.

5. Interface
Web, iOS, Android, desktop and voice interfaces that make all of this accessible.

That's why the ChatGPT UI is strategically important to OpenAI. The model is the underlying engine, but ChatGPT is the product that packages the engine, tools, data, memory, agents and integrations into something a customer can actually use.

And economically, this means OpenAI isn't just selling “tokens of model inference.” It's increasingly selling completed work—research reports, analyzed spreadsheets, generated images, code, answers, documents, and eventually entire workflows.
