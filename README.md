<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:1e3a8a,100:7c3aed&height=200&section=header&text=Meet%20Jain&fontColor=ffffff&fontSize=60&fontAlignY=38&desc=AI%20products%20%C2%B7%20Backend%20%C2%B7%20Full%20stack&descAlignY=60&descSize=18&animation=fadeIn" />

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3000&pause=1000&color=8B5CF6&center=true&vCenter=true&width=720&lines=I+build+AI+products+end+to+end.;Agents+that+check+their+own+work.;Backends+that+survive+a+SIGKILL.;Frontends+that+ship+with+a+live+link." alt="Typing SVG" />

<br/>

<a href="https://linkedin.com/in/meet-jain05"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:meetsvnjain@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://leetcode.com/u/Meet_Jain_07/"><img src="https://img.shields.io/badge/LeetCode-1860_Knight-FFA116?style=for-the-badge&logo=leetcode&logoColor=white"/></a>
<a href="https://codeforces.com/profile/Meet_Jain07"><img src="https://img.shields.io/badge/Codeforces-Specialist-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white"/></a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=MeetJain05&style=flat-square&color=8B5CF6&label=Profile+views" alt="Profile views" />

</div>

---

### 👋 About me

Computer Engineering @ **PDEU '27** · Software Engineering Intern @ **OpsHub**

I like taking an idea all the way to something deployed, with a link you can click.

| 🤖 **AI products** | ⚙️ **Backend** | 🖥️ **Full stack** |
|:---|:---|:---|
| Agents that grade their own retrieval, check their answers against evidence, ask a human before acting, and get **measured** with real evals. | APIs, queues and streaming pipelines that keep working when a worker is killed or a model provider times out. | React and Next.js frontends deployed on Vercel, Render, Cloudflare and AWS, so the result is a product, not a notebook. |

---

### 🚀 Featured projects

<table>
<tr>
<td width="55%" valign="top">

#### 🧠 [Agentic Adaptive RAG](https://github.com/MeetJain05/agentic-rag)
**[▶ Try the live demo](https://agentic-rag-chi.vercel.app)**

Ask questions over your own documents and get cited answers. Behind the chat is a **LangGraph state machine** that:
- routes on retrieved evidence, not just the question
- grades chunks and checks its answer for hallucinations
- rewrites the query and retries when an answer fails
- pauses for **human approval** before searching the web, with Postgres checkpoints so the approval survives a restart

![](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square) ![](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![](https://img.shields.io/badge/Next.js-000?style=flat-square&logo=nextdotjs) ![](https://img.shields.io/badge/RAGAS-eval-8B5CF6?style=flat-square)

</td>
<td width="45%" valign="middle">
<a href="https://agentic-rag-chi.vercel.app"><img src="https://raw.githubusercontent.com/MeetJain05/agentic-rag/main/project_images/dashboard.png" width="100%"/></a>
</td>
</tr>

<tr>
<td width="55%" valign="top">

#### ⚙️ [WorkQueue](https://github.com/MeetJain05/work-queue)
**1,740 jobs/s with 20 workers, benchmarked in CI on every push**

A background job queue in Go on Redis Streams:
- acknowledgement-based processing, so no job is lost
- retries with backoff and a replayable dead-letter queue
- `SIGKILL` a worker mid-job and `XAUTOCLAIM` hands its work to another one

![](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![](https://img.shields.io/badge/Redis_Streams-DC382D?style=flat-square&logo=redis&logoColor=white) ![](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

</td>
<td width="45%" valign="middle">
<a href="https://github.com/MeetJain05/work-queue"><img src="https://raw.githubusercontent.com/MeetJain05/work-queue/main/docs/dashboard.png" width="100%"/></a>
</td>
</tr>

<tr>
<td width="55%" valign="top">

#### 🚚 [Cold-Chain Dispatch Agent](https://github.com/MeetJain05/cold-chain-logistics-fde-project)
**Three dispatcher screens collapsed into one conversation**

A dispatcher asks in plain English, and a **LangGraph ReAct agent** pulls together everything needed to decide fast:
- reefer telemetry, through a secured read-only SQL view
- live weather at the truck's GPS location
- compliance SOPs, via vector search

It returns a cited incident report. Every tool call is audit-logged, Groq falls back to local Ollama, and the app deploys to AWS EC2 through GitHub Actions.

![](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square) ![](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white) ![](https://img.shields.io/badge/Pinecone-000?style=flat-square) ![](https://img.shields.io/badge/AWS_EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white)

</td>
<td width="45%" valign="middle">

```text
 "Is truck 14's produce at risk?"
               │
       ┌───────┴───────┐
       │  ReAct agent  │
       └───────┬───────┘
   ┌───────────┼───────────┐
   ▼           ▼           ▼
 SQL view   Weather     SOP search
(telemetry) (GPS)      (Pinecone)
   └───────────┼───────────┘
               ▼
   Cited incident report
       + audit log
```

</td>
</tr>
</table>

<details>
<summary><b>📂 View more projects</b></summary>
<br/>

| Project | What it is | Stack |
|---|---|---|
| **[RecruitAI](https://github.com/MeetJain05/breach-26)** 🥈 | Recruitment platform that ingests resumes, Gmail, BambooHR and LinkedIn data, deduplicates candidates and supports semantic search. 2nd place at a fintech hackathon | LangGraph · FastAPI · pgvector · Gemini |
| **[Agent Eval Lab](https://github.com/MeetJain05/agent-eval)** | Refund-support agent scored on 8 scenarios × 7 DeepEval metrics: task completion, plan quality, tool selection and more | LangChain · DeepEval · Streamlit |
| **[Clarity CRAG](https://github.com/MeetJain05/crag)** | Corrective RAG with three-way retrieval grading and web fallback, evaluated against a plain-RAG baseline | LangGraph · FastAPI · React |
| **[VibeStream](https://github.com/MeetJain05/crypto-analytics)** | Real-time crypto anomaly detection: Binance → Kafka → rolling z-scores → TimescaleDB → live dashboard | Kafka · TimescaleDB · React |
| **[Commonplace](https://github.com/MeetJain05/commonplace-bill-splitter)** | Household bill splitter that stores money as integer cents and makes payments idempotent | Hono · Cloudflare D1 · React · TS |
| **[Intrusion Detection](https://github.com/MeetJain05/ml-project)** | Logistic regression, Naive Bayes and K-Means written from scratch in NumPy on UNSW-NB15 (0.91 F1) | NumPy · Streamlit |
| **[Lets Code](https://github.com/MeetJain05/realtime-collab-editor)** | Real-time collaborative code editor with rooms and presence | React · Socket.io |

</details>

---

### 💼 Experience

<details open>
<summary><b>Software Engineering Intern · OpsHub</b></summary>
<br/>

- Built a Python dead-code analyzer that combines Git history, usage analysis and JaCoCo coverage. It led to **150,000+ lines** of obsolete production code and **11 unused JARs** being removed, and cut build time by **12%**.
- Worked on live production: debugged and fixed bugs and failures in the enterprise integration platform customers run on, including SQL and data-retrieval issues in integration connectors.

</details>

<details open>
<summary><b>AI Engineering Intern · La Sirene Exim</b></summary>
<br/>

- Designed a multi-tenant AI SaaS backend (Python + PostgreSQL) with RAG over Groq, Whisper and pgvector.
- Added retry and timeout handling for model calls. The backend powers per-client chatbots at **85%+ response accuracy**.

</details>

---

### 🛠️ Toolbox

<div align="center">

<img src="https://skillicons.dev/icons?i=python,go,cpp,java,ts,js&perline=12" /><br/>
<img src="https://skillicons.dev/icons?i=fastapi,nodejs,postgres,redis,kafka,mongodb&perline=12" /><br/>
<img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,vite,docker,aws,cloudflare,vercel,githubactions,linux&perline=12" />

<br/><br/>

![](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square) ![](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain) ![](https://img.shields.io/badge/RAG-8B5CF6?style=flat-square) ![](https://img.shields.io/badge/DeepEval-147D64?style=flat-square) ![](https://img.shields.io/badge/RAGAS-F97316?style=flat-square) ![](https://img.shields.io/badge/pgvector-4169E1?style=flat-square) ![](https://img.shields.io/badge/Pinecone-000?style=flat-square) ![](https://img.shields.io/badge/Groq-F55036?style=flat-square) ![](https://img.shields.io/badge/Ollama-000?style=flat-square&logo=ollama)

</div>

---

### 🏆 Highlights

<div align="center">

| 🥇 **HackOut '25** | 🏆 **Flipkart GRiD 8.0** | 🥈 **Fintech hackathon** |
|:---:|:---:|:---:|
| 1st of 1,000+ teams | National Semi-Finalist · 165K+ registrations | 2nd place with RecruitAI |
| 🧠 **LeetCode** | 💻 **Codeforces** | 📈 **LeetCode Weekly 485** |
| 1860 Knight · 550+ solved | 1411 Specialist | 1,619 / 34,222 |

</div>

---

<div align="center">

### 🤝 Let's build something

**Open to SWE, full-stack and AI engineering internships and new-grad roles.**
If you're building an AI product, I'd love to talk.

<a href="https://linkedin.com/in/meet-jain05"><img src="https://img.shields.io/badge/Say_hi_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:meetsvnjain@gmail.com"><img src="https://img.shields.io/badge/Drop_an_email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/></a>

</div>

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:7c3aed,50:1e3a8a,100:0f172a&height=110&section=footer" />
