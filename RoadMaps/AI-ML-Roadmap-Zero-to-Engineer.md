# The Complete AI/ML Roadmap: From Absolute Beginner to AI/ML Engineer

### A free-resources-only guide for students starting their coding journey

> Compiled by Shamique Khan | Last updated: August 2026
> Built on top of [Free AI & ML Courses with Certificates](https://github.com/shamiquekhan/Learning-Atlas/blob/main/Free%20Courses/FREE_AI_ML_Courses_With_Certificates.md) and [Harvard CS50 Free Courses Guide](https://github.com/shamiquekhan/Learning-Atlas/blob/main/Free%20Courses/Harvard-CS50-Free-Courses-Guide.md), cross-checked against current course catalogs.
>
> Goal: Take you from "never written a line of code" to "AI/ML Engineer who can build, deploy, and explain real systems" — using 100% free resources, with honest notes on what's actually worth your time.

---

## How to Use This Guide

1. **Don't skip phases, but don't binge them either.** Each phase builds on the last. Spending two focused weeks on a phase beats two rushed days.
2. **Certificates are a bonus, not the goal.** A certificate proves you sat through a course. A project proves you can *do the job*. Weight your time roughly 30% courses / 70% building.
3. **One course per topic is enough.** You don't need five different "Intro to ML" videos. Pick one from this list, finish it, build something with it, move on.
4. **This is an 8–14 month roadmap** if you study 10–15 hrs/week, done properly (not rushed). Compress it if you can put in more hours, but don't skip the math or the projects to "save time" — that's the most common mistake beginners make.
5. **Share this.** If it helps you, pass it to the next junior. That's the whole point.

---

## Table of Contents

- [Phase 0: Setup and Mindset](#phase-0-setup-and-mindset)
- [Phase 1: Programming Foundations](#phase-1-programming-foundations)
- [Phase 2: Math for Machine Learning](#phase-2-math-for-machine-learning)
- [Phase 3: Data Handling and Analysis](#phase-3-data-handling-and-analysis)
- [Phase 4: Core Machine Learning](#phase-4-core-machine-learning)
- [Phase 5: Deep Learning](#phase-5-deep-learning)
- [Phase 6: NLP and Transformers](#phase-6-nlp-and-transformers)
- [Phase 7: Generative AI Foundations](#phase-7-generative-ai-foundations)
- [Phase 8: RAG (Retrieval-Augmented Generation)](#phase-8-rag-retrieval-augmented-generation)
- [Phase 9: Vector Databases Deep Dive](#phase-9-vector-databases-deep-dive)
- [Phase 10: LangChain and LangGraph](#phase-10-langchain-and-langgraph)
- [Phase 11: AI Agents and Agentic AI](#phase-11-ai-agents-and-agentic-ai)
- [Phase 12: MLOps and Deployment](#phase-12-mlops-and-deployment)
- [Phase 13: Specialization Tracks](#phase-13-specialization-tracks-pick-one)
- [Phase 14: Cloud AI (Optional)](#phase-14-cloud-ai-optional-but-valuable)
- [The Portfolio: What Actually Gets You Hired in 2026](#the-portfolio-what-actually-gets-you-hired-in-2026)
- [Certificates Worth Actually Doing](#certificates-worth-actually-doing-quick-reference)
- [Full Timeline (8–14 Months)](#suggested-full-timeline-8-14-months)
- [Communities, Practice and Staying Current](#communities-practice-and-staying-current)
- [Honest Tips from Someone Who's Done This](#honest-tips-from-someone-whos-done-this)

---

## Phase 0: Setup and Mindset

Before touching a single course, set up your environment. This takes one afternoon.

| Tool | Why You Need It | Link |
|---|---|---|
| VS Code | Your code editor. Free, industry standard. | [code.visualstudio.com](https://code.visualstudio.com/) |
| Python 3.11+ | The language of AI/ML. | [python.org](https://python.org) |
| Git + GitHub account | Version control and your public portfolio. Non-negotiable. | [github.com](https://github.com) |
| Google Colab | Free GPU/TPU notebooks in the browser, no setup needed. Use this for anything that needs a GPU before you can afford or access one locally. | [colab.research.google.com](https://colab.research.google.com) |
| Kaggle account | Free notebooks (with GPU quota), datasets, and competitions. | [kaggle.com](https://kaggle.com) |
| Anaconda / Miniconda (optional) | Environment management for local work. | [anaconda.com](https://www.anaconda.com/) |

**Mindset notes:**

- You do not need a powerful laptop. Colab and Kaggle give you free GPUs. A basic laptop with a browser is enough for the first six months.
- Tutorial hell is real. If you've watched three-plus hours of a course without opening your own editor and typing code, stop and go build something small with what you just learned.
- AI/ML is a marathon of layered skills: programming, then math, then ML, then DL, then GenAI and agents. Skipping a layer means the next one won't make sense. Resist the urge to jump straight to "building a chatbot" without understanding what's underneath it.

---

## Phase 1: Programming Foundations

*Goal: Get fluent in Python, basic CS concepts, and Git — before touching any ML.*

### 1.1 Computer Science and Python Fundamentals

| Course | Provider | Time | Certificate | Why It's Worth It |
|---|---|---|---|---|
| CS50x — Intro to Computer Science | Harvard (OCW) | ~100 hrs / 12 weeks | Free (via [cs50.harvard.edu/x](https://cs50.harvard.edu/x/), not edX) | The gold standard CS foundation course. Covers C, Python, SQL, memory, algorithms, and even a taste of AI. If you do only one foundational course, make it this one. |
| CS50P — Introduction to Programming with Python | Harvard (OCW) | ~20 hrs | Free | A faster, Python-only path if you want to skip C and get to Python quicker. Good if you're short on time. |
| freeCodeCamp — Scientific Computing with Python | freeCodeCamp | ~300 hrs (self-paced, go faster) | 100% Free | Practical, project-based Python. Pairs well with CS50P. |
| Python Essentials 1 & 2 | Cisco Networking Academy | ~80 hrs total | Free Certificate | Structured, beginner-friendly, good if you want a slower on-ramp. |

Note on CS50 certificates: the certificate is only free through cs50.harvard.edu, not through edX (edX charges $199+). Always start the course from the Harvard OCW link, not the edX link, if you want it free.

### 1.2 Data Structures and Algorithms (Basic Level)

You don't need LeetCode-grinder-level DSA to start ML, but you need to be comfortable with lists, dictionaries, loops, recursion, basic time complexity, and writing clean functions.

- CS50x (above) already covers this well.
- [NeetCode 150 (free, YouTube)](https://neetcode.io/) — once you're comfortable with Python, work through the "easy" tier over a few weeks. This matters because AI Engineer interviews at real companies still include basic coding rounds.

### 1.3 Git and GitHub

- [GitHub Skills](https://skills.github.com/) — free, interactive, official GitHub tutorials. Do "Introduction to GitHub" and "Communicate using Markdown."
- Learn: `git init`, `add`, `commit`, `push`, `pull`, branches, `.gitignore`, and writing a good `README.md`.

**Phase 1 checkpoint project:** Build two or three small CLI Python tools (a calculator, a to-do list, a simple web scraper) and push them to GitHub with clean READMEs. This is your first portfolio commit.

---

## Phase 2: Math for Machine Learning

*Goal: Understand the "why" behind ML, not just import sklearn and hope for the best. This is the phase most beginners skip — don't.*

You don't need a math degree. You need working intuition and the ability to read an equation in a paper without panicking.

### 2.1 The Core Four Areas

| Topic | Best Free Resource | Format | Notes |
|---|---|---|---|
| Linear Algebra | [3Blue1Brown — Essence of Linear Algebra](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab) | YouTube playlist (~3 hrs) | The best visual intuition-builder for vectors, matrices, dot products, and eigenvectors. Watch this before anything else. |
| Linear Algebra (rigorous) | [MIT OCW 18.06 — Gilbert Strang](https://ocw.mit.edu/courses/18-06-linear-algebra-spring-2010/) | Free video + notes | For depth after 3Blue1Brown. |
| Calculus | [3Blue1Brown — Essence of Calculus](https://www.youtube.com/playlist?list=PLZHQObOWTQDMsr9K-rj53DwVRMYO3t5Yr) | YouTube (~3 hrs) | Understand derivatives and gradients visually — this is how gradient descent and backpropagation work. |
| Probability and Statistics | [StatQuest with Josh Starmer](https://www.youtube.com/@statquest) | YouTube (as-needed) | The best resource for distributions, Bayes' theorem, p-values, and statistical concepts used constantly in ML. Reference per topic rather than binge-watch. |
| All-in-one (structured) | [Mathematics for Machine Learning Specialization](https://www.coursera.org/specializations/mathematics-machine-learning) (Imperial College London, Coursera) | ~2 months | Free to audit (no certificate without paying), but the audit gives full video and material access, which is what matters here. Covers linear algebra, multivariable calculus, and PCA. |
| Book (free PDF) | [Mathematics for Machine Learning (Deisenroth, Faisal, Ong)](https://mml-book.github.io/) | Free PDF textbook | The standard free reference textbook. Use it to look things up, not read cover to cover. |

### 2.2 What to Actually Prioritize

- Linear algebra: vectors, matrix multiplication, dot products, eigenvalues/eigenvectors (for PCA) — high priority.
- Calculus: derivatives, partial derivatives, chain rule, gradients — high priority (this is literally what backpropagation is).
- Probability/statistics: distributions, mean/variance, Bayes' theorem, hypothesis testing, conditional probability — high priority.
- Optimization: gradient descent and its variants (SGD, Adam) — you'll learn this naturally during Phase 4/5, no need to study it in isolation first.

Honest tip: don't try to "finish math" before starting ML. Learn math in parallel with Phase 3–4, filling gaps as concepts come up (you'll understand eigenvectors much better once you see PCA in action). Math in a vacuum is forgettable; math applied sticks.

---

## Phase 3: Data Handling and Analysis

*Goal: Every ML model is downstream of data. Learn to wrangle it first.*

| Skill | Resource | Certificate |
|---|---|---|
| NumPy | [NumPy official Quickstart](https://numpy.org/doc/stable/user/quickstart.html); also covered implicitly in Kaggle's Pandas course | Free |
| Pandas | [Kaggle Learn — Pandas](https://www.kaggle.com/learn/pandas) (~4 hrs) | Free Certificate |
| Data Cleaning | [Kaggle Learn — Data Cleaning](https://www.kaggle.com/learn/data-cleaning) (~4 hrs) | Free Certificate |
| Data Visualization | [Kaggle Learn — Data Visualization](https://www.kaggle.com/learn/data-visualization) + [freeCodeCamp Data Visualization](https://www.freecodecamp.org/learn/data-visualization/) | Free Certificates |
| SQL | [Kaggle Learn — Intro to SQL](https://www.kaggle.com/learn/intro-to-sql) + [Advanced SQL](https://www.kaggle.com/learn/advanced-sql) | Free Certificates |
| Full applied path | [freeCodeCamp — Data Analysis with Python](https://www.freecodecamp.org/learn/data-analysis-with-python/) | 100% Free Certificate |

**Phase 3 checkpoint project:** Pick a messy real-world dataset from Kaggle, clean it, run exploratory data analysis, and publish a notebook with visualizations and written insights on Kaggle or GitHub.

---

## Phase 4: Core Machine Learning

*Goal: Understand how models actually learn — regression, classification, trees, ensembles, evaluation.*

### 4.1 Primary Courses (Pick One Main Track)

| Course | Provider | Time | Certificate | Verdict |
|---|---|---|---|---|
| Machine Learning Specialization (Andrew Ng) | DeepLearning.AI + Stanford, Coursera | ~2 months | Free to audit; paid certificate (~$49/mo) | The best structured ML course available. Audit mode gives every video and assignment — genuinely worth it even without the certificate. |
| Stanford CS229: Machine Learning (Andrew Ng, full lectures) | Stanford (YouTube, Autumn 2018) | ~27 hrs of lectures | No certificate, fully free | The rigorous, math-heavy original. Do this after the Coursera version if you want deeper theory (SVMs, GLMs, EM algorithm, learning theory). |
| Kaggle Learn — Intro + Intermediate ML | Kaggle | ~7 hrs combined | Free Certificates | Fast, extremely practical, code-first. Great complement to Ng's theory-heavy course. |
| freeCodeCamp — Machine Learning with Python | freeCodeCamp | ~300 hrs (self-paced) | 100% Free Certificate | Full project-based certification using TensorFlow. |
| IBM — Machine Learning with Python (CognitiveClass.ai) | IBM | ~6 hrs | Free Badge | Good scikit-learn-focused supplement. |

### 4.2 What You Should Be Able to Do by the End

- Explain linear/logistic regression, decision trees, random forests, gradient boosting (XGBoost/LightGBM), k-NN, k-means, SVMs, and PCA.
- Explain the bias-variance tradeoff, overfitting/underfitting, train/validation/test splits, cross-validation, and regularization (L1/L2).
- Use scikit-learn fluently to build, evaluate, and tune models.
- Do feature engineering: [Kaggle Learn — Feature Engineering](https://www.kaggle.com/learn/feature-engineering) (~5 hrs, free certificate).

**Phase 4 checkpoint project:** Enter a beginner Kaggle competition (Titanic, House Prices) — not for the leaderboard, but to practice the full pipeline: EDA, cleaning, feature engineering, modeling, submission. Then do one more advanced tabular project on a dataset you personally chose (not a toy dataset) and deploy it as a simple Streamlit app.

---

## Phase 5: Deep Learning

*Goal: Neural networks — from the math up, and from working code down. Do both directions.*

### 5.1 Top-Down (Build First, Understand as You Go)

| Course | Provider | Time | Certificate |
|---|---|---|---|
| Practical Deep Learning for Coders | fast.ai (Jeremy Howard) | ~7 weeks (~20 hrs) | No certificate, fully free | The best code-first deep learning course. You'll train real computer vision/NLP models by lesson two. Uses PyTorch and the fastai library. Pairs with the free book at [fastai.github.io/fastbook2e](https://fastai.github.io/fastbook2e/). |
| Kaggle Learn — Intro to Deep Learning | Kaggle | ~4 hrs | Free Certificate | Fast, practical intro using Keras/TensorFlow. |

### 5.2 Bottom-Up (Build the Math and Code from Scratch)

| Course | Provider | Time | Certificate |
|---|---|---|---|
| Neural Networks: Zero to Hero | Andrej Karpathy (former Tesla AI Director, former OpenAI) | ~15+ hrs across the series | No certificate, fully free | The single best resource for truly understanding how neural nets and transformers work, built from raw Python/PyTorch with no hand-waving — from backpropagation to GPT. [karpathy.ai/zero-to-hero.html](https://karpathy.ai/zero-to-hero.html) |
| Deep Learning Fundamentals Lab | WorldQuant University | ~16 weeks | Free accredited certificate plus Credly badge | A rigorous, project-based, DEAC-accredited deep learning program — a rare truly accredited free credential. |
| Deep Learning Specialization (Andrew Ng) | DeepLearning.AI, Coursera | ~4 months | Free to audit | The theory-heavy companion — covers CNNs, RNNs/LSTMs, and sequence models. |
| CS231n: Convolutional Neural Networks for Visual Recognition | Stanford (YouTube lectures) | ~15 lectures | No certificate, free | The classic computer vision deep learning course, originally built by Karpathy himself. |
| Dive into Deep Learning (d2l.ai) | Free interactive textbook | Self-paced | No certificate | Code, math, and theory in one place with runnable notebooks. Excellent as a reference alongside any course above. |

### 5.3 Frameworks

Learn PyTorch as your primary framework (industry standard in research and increasingly in production). Know TensorFlow/Keras at a basic level too, since many free courses (Kaggle, freeCodeCamp) use it.

**Phase 5 checkpoint project:** Build an image classifier (computer vision) or a text classifier (NLP) from scratch using PyTorch, without high-level shortcuts, so you understand every step: data loader, model, loss, optimizer, training loop. Then fine-tune a small pretrained model on your own dataset.

---

## Phase 6: NLP and Transformers

*Goal: Understand what's actually inside GPT/Claude/Gemini before using them as black boxes.*

| Resource | Provider | Time | Certificate |
|---|---|---|---|
| Hugging Face LLM Course | Hugging Face | Self-paced (~40+ hrs) | Free Certificate | The best free, hands-on path to Transformers, tokenization, fine-tuning, and the Hugging Face ecosystem (`transformers`, `datasets`, `tokenizers`). The course most working AI engineers point beginners to. |
| CS224n: NLP with Deep Learning | Stanford (YouTube lectures, Manning) | ~20 lectures | No certificate, free | The academic-depth NLP/transformer course — attention, word embeddings, sequence models, and the theory behind modern LLMs. |
| The Illustrated Transformer (Jay Alammar) | Blog | ~1 hr read | Free | The most well-known visual explainer of transformer architecture. Read this before or alongside CS224n. |
| Hugging Face — Audio and Computer Vision courses (optional) | Hugging Face | Self-paced | Free Certificate | Only if you want to specialize further in multimodal AI. |

**Phase 6 checkpoint project:** Fine-tune a small pretrained transformer (for example, DistilBERT) on a text classification task using Hugging Face `transformers`, and write up what tokenization and attention are doing in your own words in the README.

---

## Phase 7: Generative AI Foundations

*Goal: Prompting, LLM APIs, and the conceptual foundation for everything downstream (RAG, agents).*

| Course | Provider | Time | Certificate |
|---|---|---|---|
| Anthropic Prompt Engineering Interactive Tutorial | Anthropic Academy | Self-paced (9 chapters) | Free | Hands-on, code-based prompt engineering straight from the maker of Claude — covers XML structuring, chain-of-thought, few-shot prompting, and how to get reliable outputs from LLMs. |
| Anthropic Academy — Building with the Claude API | Anthropic | ~8+ hrs, 84 lessons | Free with certificate | Deep dive into building real applications on top of an LLM API — directly transferable to OpenAI/Gemini APIs too. |
| Generative AI for Beginners | Microsoft (GitHub, open-source) | Self-paced, 21 lessons | Free Certificate | MIT-licensed, well-maintained curriculum: prompt engineering, RAG, agents, and responsible AI. |
| Google — Intro to Generative AI + Intro to LLMs | Google Cloud Skills Boost | ~2 hrs combined | Free Skill Badges | Short, good for the conceptual big picture. |
| DAIR.AI Prompt Engineering Guide | promptingguide.ai | Reference | Free | The best free reference for advanced prompting techniques (ReAct, self-consistency, and others) — bookmark rather than binge-read. |
| Kaggle — Intro to LLMs | Kaggle | ~2 hrs | Free Certificate | Quick, practical intro. |

**Phase 7 checkpoint project:** Build a small CLI or Streamlit app that calls an LLM API (Claude, OpenAI, and Gemini all have free tiers) to do something useful, such as a resume reviewer or study-notes summarizer. Focus on prompt design and structured outputs.

---

## Phase 8: RAG (Retrieval-Augmented Generation)

*Goal: Learn how to ground LLMs in real data — the single most in-demand GenAI skill in 2026 hiring.*

RAG is currently the top skill hiring managers look for in entry-level Gen AI / AI Engineer roles — it shows you can connect an LLM to real documents instead of relying on the model's training data alone.

| Course | Provider | Time | Certificate |
|---|---|---|---|
| RAG-related short courses (LangChain: Chat with Your Data; Building Applications with Vector Databases; Knowledge Graphs for RAG) | DeepLearning.AI | ~1–2 hrs each | Free to view (certificate availability varies — check current status) |
| Advanced RAG certification (35 lessons, 7+ projects) | Activeloop | Self-paced | Free certificate | Covers RAG fundamentals, LangChain, LlamaIndex, evaluation, and observability in real depth. |
| NVIDIA — Building RAG Agents with LLMs (intro) | NVIDIA DLI | ~1–2 hrs | Free Certificate | Short but from a top-tier lab; a good supplement. |
| LlamaIndex documentation and tutorials | LlamaIndex (open-source docs) | Self-paced | Free | The other major RAG framework besides LangChain — worth knowing both. |

### What "Understanding RAG" Actually Means

1. Chunking strategies — how you split documents matters more than beginners expect.
2. Embeddings — turning text into vectors (covered in Phase 9).
3. Retrieval — similarity search, hybrid search (vector plus keyword/BM25), re-ranking.
4. Generation — feeding retrieved context to the LLM correctly, handling "I don't know" cases, avoiding hallucination.
5. Evaluation — measuring whether your RAG system actually retrieves the right thing. This is what separates a toy RAG demo from a production-quality one.

**Phase 8 checkpoint project:** Build a RAG chatbot over a non-trivial document set in a domain you care about (legal docs, research papers, class notes, a codebase). Deploy it with a simple web interface (Streamlit or FastAPI plus a frontend). This is widely considered the single highest-leverage portfolio project for Gen AI roles in 2026.

---

## Phase 9: Vector Databases Deep Dive

*Goal: Understand the memory layer behind RAG and semantic search.*

| Resource | Notes |
|---|---|
| Official docs and free tiers of [Chroma](https://www.trychroma.com/), [Pinecone](https://www.pinecone.io/), [Qdrant](https://qdrant.tech/), [Weaviate](https://weaviate.io/), and [FAISS](https://github.com/facebookresearch/faiss) (Meta, fully open-source) | Learn by building, not by watching. Start with Chroma or FAISS (both fully free/local, no signup needed) to prototype, then try Qdrant (best free cloud tier) or Pinecone for a managed setup. |
| Vector Databases: Vector Search for AI (DeepLearning.AI / Pinecone) | Free short course covering embeddings, approximate nearest neighbor search, and how vector databases differ from traditional databases. |
| pgvector | If you already know PostgreSQL, this is a genuinely free, zero-extra-infrastructure way to add vector search to a Postgres database — worth knowing for smaller-scale production systems. |

### Quick Reference: Which Vector Database to Use

- Prototyping/learning locally: Chroma or FAISS (no server, no signup)
- Free cloud tier, best developer experience: Qdrant
- Postgres users: pgvector
- Managed, zero-ops, most recognizable name on a resume: Pinecone

**Phase 9 checkpoint:** No separate project needed — this feeds directly into your Phase 8 RAG project. Experiment with swapping vector databases in that project to understand the tradeoffs hands-on.

---

## Phase 10: LangChain and LangGraph

*Goal: The dominant orchestration framework for LLM apps and agents in 2026.*

| Course | Provider | Time | Certificate |
|---|---|---|---|
| LangChain Academy | LangChain (official, free) | Self-paced | Free | Straight from the source — LCEL chains, RAG pipelines, memory, and an intro to LangGraph. Learning from official docs avoids fighting outdated third-party tutorials. |
| AI Agents in LangGraph | DeepLearning.AI (taught by Harrison Chase, LangChain founder) | ~2 hrs | Free to view | Build an agent from scratch, then rebuild it in LangGraph — you'll understand why LangGraph exists, not just its syntax. |
| LangGraph official docs and tutorials | LangChain | Self-paced | Free | LangGraph is the dominant framework for building stateful, controllable multi-step agents in 2026 — worth deep familiarity, not just a surface pass. |

Why LangGraph specifically matters: plain LangChain chains are linear; LangGraph lets you build agents with loops, conditional branching, human-in-the-loop checkpoints, and persistent memory — what real production agent systems need.

**Phase 10 checkpoint project:** Rebuild your Phase 8 RAG chatbot as a LangGraph graph with explicit nodes (retrieve, grade relevance, generate, self-check) instead of a single linear chain. This alone demonstrates a meaningfully more advanced skill than most beginner portfolios.

---

## Phase 11: AI Agents and Agentic AI

*Goal: Move from "LLM answers a question" to "LLM uses tools and takes multi-step actions autonomously."*

| Course | Provider | Time | Certificate |
|---|---|---|---|
| Hugging Face AI Agents Course | Hugging Face | Self-paced | Free Certificate | The best structured, free path into agent concepts — ReAct, tool use, planning, and building agents with `smolagents`, LangGraph, and LlamaIndex. Widely respected in the open-source AI community. |
| Anthropic — Building Effective Agents (guide) + Agent SDK courses | Anthropic Academy / Anthropic Engineering Blog | Self-paced | Free | Practical, opinionated guidance on when (and when not) to use agents, and how to build reliable ones. |
| AI Agents in LangGraph | DeepLearning.AI | ~2 hrs | Free to view | Same as Phase 10 — this is where agents and LangGraph intersect. |
| CrewAI free tutorials/docs | CrewAI (open-source) | Self-paced | Free | The leading framework for multi-agent, role-based systems (a "researcher agent" and "writer agent" collaborating) — a good alternative pattern to LangGraph. |
| Model Context Protocol (MCP) Course | Hugging Face | Self-paced | Free Certificate | MCP is becoming the standard way agents connect to external tools and data sources across labs (Anthropic, OpenAI, Google) — an increasingly common keyword in 2026 job postings. |

### Pick Your Agent Framework Based on Where You Want to Work

- Working inside codebases/dev tools: Claude Agent SDK / Claude Code ecosystem
- Complex, stateful, controllable workflows: LangGraph
- Multi-agent role-play / business process automation: CrewAI or AutoGen
- Connecting agents to external tools/data in a standardized way: MCP

**Phase 11 checkpoint project:** Build an agent that uses at least two tools autonomously (for example, web search plus a calculator/code execution tool, or a CSV analyzer plus report generator) and makes multi-step decisions, not just a single tool call. This is one of the project types that most directly maps to what 2026 GenAI job descriptions ask for.

---

## Phase 12: MLOps and Deployment

*Goal: A model in a notebook is worthless to an employer. Learn to ship it.*

This phase separates "I did some ML tutorials" from "I can do the job." Recruiters in 2026 explicitly look for deployed, containerized projects, not just `.ipynb` files.

| Resource | Provider | Time | Certificate |
|---|---|---|---|
| Machine Learning Zoomcamp | DataTalks.Club (free, community-run) | ~4 months, self-paced | Free (community certificate) | An excellent full free course covering classical ML through deployment with Docker, FastAPI, and Kubernetes basics — one of the best-kept-secret free resources in ML learning. |
| MLOps Zoomcamp | DataTalks.Club | Self-paced | Free | Covers experiment tracking (MLflow), workflow orchestration, model monitoring, and CI/CD specifically for ML systems. |
| FastAPI official tutorial | FastAPI docs | ~4–6 hrs | Free | Learn to wrap any model (ML or LLM) in a clean REST API — the standard way to serve models in production. |
| Docker official Get Started guide | Docker | ~3–4 hrs | Free | Containerize your app so it runs anywhere — a baseline expectation for engineer roles, not just scientist roles. |
| GitHub Actions (CI/CD) | GitHub Skills / docs | Self-paced | Free | Automate testing and deployment — even a basic pipeline on a portfolio project stands out. |
| Hugging Face Spaces | Hugging Face | N/A | Free hosting | The easiest free way to publicly host and demo your models/apps — use this for every project from here on. |
| Streamlit | Streamlit docs | ~2–3 hrs | Free | The fastest way to put a usable UI on any Python/ML project — great for demos, less "production-grade" than FastAPI plus a real frontend, but ideal for fast iteration. |

**Phase 12 checkpoint project:** Take your best RAG or agent project from Phase 8/11 and: wrap it in a FastAPI backend, containerize with Docker, add basic tests, set up a GitHub Actions CI pipeline, and deploy it publicly (Hugging Face Spaces, Render, or Railway all have free tiers). This single project, done properly, is your strongest resume item.

---

## Phase 13: Specialization Tracks (Pick One)

Once you have the full stack above, branch into a specialty. Don't do all of these — pick based on interest.

| Track | Best Free Resource | Notes |
|---|---|---|
| Computer Vision | [OpenCV Bootcamp (free, OpenCV University)](https://opencv.org/university/free-opencv-course/), CS231n, and [WQU Computer Vision Lab](https://www.wqu.edu/ai-lab-computer-vision) (accredited, free) | Image processing, object detection, segmentation. |
| Reinforcement Learning | [Hugging Face Deep RL Course](https://huggingface.co/learn/deep-rl-course) (free certificate) | Niche but valuable for robotics, game AI, and advanced agent training. |
| Fine-tuning and PEFT (LoRA/QLoRA) | [Hugging Face Smol Course](https://huggingface.co/learn/smol-course) (free certificate) | Learn to fine-tune open-source LLMs efficiently on consumer hardware. |
| Diffusion Models / Image Generation | [Hugging Face Diffusion Models Course](https://huggingface.co/learn/diffusion-course) (free certificate) | Stable Diffusion internals, image generation pipelines. |
| Time Series | [Kaggle Learn — Time Series](https://www.kaggle.com/learn/time-series) (free certificate) | Forecasting — valuable in finance, operations, and IoT. |
| AI Governance / Responsible AI | [Kaggle — Intro to AI Ethics](https://www.kaggle.com/learn/intro-to-ai-ethics) and [Securiti AI Governance Certification](https://education.securiti.ai/certifications/ai-governance/) (free) | Increasingly relevant as regulation catches up with AI deployment. |
| Robotics | [Hugging Face Robotics Course (LeRobot)](https://huggingface.co/learn/robotics-course) (free certificate) | Advanced — needs strong DL fundamentals first. |

---

## Phase 14: Cloud AI (Optional but Valuable)

Cloud AI skills widen your job pool, since many companies deploy on AWS, Azure, or GCP, and free skill badges are quick wins for your resume.

| Track | Path | Certificate |
|---|---|---|
| AWS | [Fundamentals of ML & AI](https://skillbuilder.aws/) then [Foundations of Prompt Engineering](https://skillbuilder.aws/) | Free badges |
| Google Cloud | [Intro to Generative AI](https://www.cloudskillsboost.google/course_templates/536) then [Prompt Design in Vertex AI](https://www.cloudskillsboost.google/course_templates/976) | Free skill badges |
| Microsoft Azure | [Intro to Azure AI Studio](https://learn.microsoft.com/en-us/training/modules/introduction-to-azure-ai-studio/) then [AI Skills Fest (AI-900 prep)](https://learn.microsoft.com/en-us/training/challenges) | Free badges (the AI-900 exam itself is paid, but all learning content is free) |

These are supplementary — don't prioritize over Phases 1–12. Fit these in short bursts between major phases as quick, resume-friendly wins.

---

## The Portfolio: What Actually Gets You Hired in 2026

Based on current hiring signals, recruiters increasingly screen GitHub first and resumes second. A Titanic classifier or basic sentiment analysis notebook is now a red flag rather than a green one — thousands of other applicants have the identical project.

### Build These Five Projects, in This Order

1. A tabular ML project on a dataset you personally sourced (not a famous Kaggle toy dataset) — proves you can handle messy real-world data, not just pre-cleaned CSVs.
2. A RAG chatbot over a non-trivial document set, deployed with a UI. This is the highest-leverage single project in 2026 GenAI hiring.
3. An agent that uses two or more tools autonomously and makes multi-step decisions (LangGraph or CrewAI).
4. A fine-tuned model project — even a small one (a LoRA fine-tune of a small open-source LLM, or a fine-tuned classifier) — shows you can go beyond calling APIs.
5. An end-to-end deployed system: FastAPI, Docker, CI/CD, hosted publicly, with monitoring/logging if possible.

### Portfolio Rules That Matter

- Every project needs a clean README: what it does, why you built it, an architecture overview if relevant, how to run it, and what you'd improve with more time. Honest gap disclosure builds more trust than inflated claims — recruiters can tell the difference.
- Deploy everything. A model that only lives in a notebook proves nothing about your engineering ability. Hugging Face Spaces, Render, and Railway all have free tiers for this.
- Link your resume bullets directly to GitHub repos. "Built a RAG system" should link straight to the repo.
- Keep a mix: two or three broad projects across different domains, plus one or two deep specializations in whatever you're most drawn to. This "T-shaped" portfolio signals both range and depth.

---

## Certificates Worth Actually Doing (Quick Reference)

Sorted by real-world signal strength, based on employer recognition and rigor.

| Tier | Certificate | Why |
|---|---|---|
| Highest signal | Hugging Face course certificates (LLM Course, Agents Course) | Most recognized within the open-source AI/ML engineering community — the community actually hiring for these roles. |
| Highest signal | WorldQuant University (Applied Data Science Lab, Deep Learning Lab, Computer Vision Lab) | Genuinely DEAC-accredited — the only free credential on this list from an accredited university. Project-based and rigorous. |
| Highest signal | Harvard CS50x / CS50P / CS50 AI | Strong, universally recognized brand; free if claimed correctly via cs50.harvard.edu. |
| Strong signal | Google / Microsoft / AWS / IBM / Cisco skill badges | Solid brand recognition, especially for cloud-AI-adjacent roles. Quick to earn, good resume filler between bigger projects. |
| Strong signal | Anthropic Academy certificates | Directly from a top AI lab; strong for AI-integration and prompt-engineering-focused roles. |
| Good supplement | freeCodeCamp, Kaggle Learn | Legitimately free, no gimmicks, good for proving consistent hands-on skill-building — but lower brand recognition than the above. |
| Skip | "Audit mode" certificates on Coursera/edX (no certificate without paying) | Audit for the content, which is often excellent (Andrew Ng's specializations, for example), but don't expect or chase a certificate from these unless you're willing to pay. |

---

## Suggested Full Timeline (8-14 Months)

Assumes 10–15 hours per week. Adjust based on your pace — the order matters more than the exact timing.

| Months | Focus |
|---|---|
| 1 | Phase 0 + Phase 1 (Python, CS50, Git) |
| 2 | Phase 2 + Phase 3 (math foundations, Pandas/SQL/EDA) — done in parallel |
| 3–4 | Phase 4 (core ML) + first Kaggle competition |
| 5–6 | Phase 5 (deep learning — fast.ai and Karpathy) |
| 7 | Phase 6 (NLP/transformers) |
| 8 | Phase 7 (GenAI foundations and prompt engineering) |
| 9 | Phase 8 + 9 (RAG and vector databases) — build project 2 |
| 10 | Phase 10 (LangChain/LangGraph) |
| 11 | Phase 11 (AI agents) — build project 3 |
| 12 | Phase 12 (MLOps/deployment) — deploy everything properly |
| 13–14 | Phase 13/14 (specialization and cloud badges) + polish portfolio, apply to roles/internships |

You can start applying for internships around month 6–7, once you have one or two solid ML/DL projects — don't wait until you've "finished everything." Real-world experience accelerates the rest of this roadmap faster than any course will.

---

## Communities, Practice, and Staying Current

- Kaggle — competitions, datasets, notebooks, and a genuinely active community. Read top solutions after competitions end; this teaches more than most courses.
- r/MachineLearning, r/learnmachinelearning — good for staying current and asking questions.
- Papers With Code ([paperswithcode.com](https://paperswithcode.com/)) — track state-of-the-art research paired with actual code implementations.
- Hugging Face Hub — browse models, datasets, and spaces to see what's actually being built right now.
- GitHub Trending (AI category) — see what tools and frameworks are gaining traction.
- DataTalks.Club Slack/Discord — an active community around their free Zoomcamps.
- AI moves fast. Treat courses as foundations, and treat blogs, docs, GitHub repos, and papers as your ongoing education after this roadmap.

---

## Honest Tips from Someone Who's Done This

1. Disclose your gaps, don't hide them. In interviews and READMEs, saying "I haven't optimized this for scale yet, here's what I'd do" builds more trust than pretending everything is production-perfect. Interviewers can tell the difference immediately.
2. Ship broken things faster than you polish perfect things. A deployed, slightly rough RAG app beats a beautiful, never-deployed notebook.
3. The math will click in layers. You won't fully "get" backpropagation the first time you see it — you'll understand it more each time you re-encounter it (Karpathy's course, then a paper, then your own implementation). That's normal, not a sign you're behind.
4. Don't chase every new framework. LangGraph, CrewAI, AutoGen, and MCP — the underlying concepts (state, tools, memory, orchestration) matter more than any one library's syntax. Learn the concepts deeply in one framework; picking up the next takes days, not months.
5. Certificates open doors slightly; projects open them fully. Nobody has ever been hired because of a Coursera badge alone. But a badge plus a genuinely good project on the same topic is a strong combination.
6. Compute is not your bottleneck. Colab, Kaggle, and Hugging Face Spaces give you enough free GPU access to build a genuinely strong portfolio before you ever need to pay for cloud compute.
7. Talk about your projects like an engineer, not a student. "I built a model that got 92% accuracy" says less than "I found that my RAG system was failing on multi-hop questions, so I added a query decomposition step, which improved retrieval accuracy from X to Y." Depth of understanding matters more than headline metrics.

---

## Source Guides This Roadmap Was Built On

- [Free AI & ML Courses with Certificates](https://github.com/shamiquekhan/Free-Cources/blob/main/FREE_AI_ML_Courses_With_Certificates.md) — Shamique Khan
- [Harvard CS50 Free Courses Guide](https://github.com/shamiquekhan/Free-Cources/blob/main/Harvard-CS50-Free-Courses-Guide.md) — Shamique Khan
- Cross-referenced against current (2026) course catalogs from DeepLearning.AI, Hugging Face, fast.ai, Stanford Online, WorldQuant University, Anthropic Academy, and DataTalks.Club, plus current hiring-signal reporting on AI/ML portfolio expectations.

---

*If this helped you, star the source repo and pass this file to the next junior who asks where to even start with AI. That's the whole point of writing it.*
