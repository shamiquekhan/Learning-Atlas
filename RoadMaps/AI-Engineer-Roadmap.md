## AI Engineer Roadmap

«From Software Engineering → Machine Learning → LLMs → AI Systems → Production

A practical, engineering-first roadmap for becoming an AI Engineer capable of designing, building, evaluating, deploying, optimizing, and operating real AI systems.»

Repository: "Learning-Atlas" (https://github.com/shamiquekhan/Learning-Atlas)
Recommended path: Foundations → ML → Deep Learning → LLMs → Retrieval → Agents → Evaluation → Inference → Production → Optimization → Advanced AI Systems

---

What Is an AI Engineer?

An AI Engineer is not simply someone who knows how to call an LLM API.

Modern AI engineering sits at the intersection of:

Software Engineering
        +
Machine Learning
        +
Deep Learning
        +
LLM / Foundation Models
        +
Data Engineering
        +
Systems Engineering
        +
Inference / Optimization
        +
Cloud / Infrastructure
        +
Evaluation / Observability

The job is to turn models into reliable, measurable, cost-effective software systems.

A useful mental model is:

        ┌──────────────────────┐
        │       Product        │
        └──────────┬───────────┘
                   │
        ┌──────────▼───────────┐
        │    AI Application    │
        └──────────┬───────────┘
                   │
      ┌────────────▼────────────┐
      │   Agents / RAG / Tools   │
      └────────────┬────────────┘
                   │
        ┌──────────▼───────────┐
        │   Model / Inference  │
        └──────────┬───────────┘
                   │
      ┌────────────▼────────────┐
      │ GPU / Runtime / Serving │
      └────────────┬────────────┘
                   │
        ┌──────────▼───────────┐
        │ Infrastructure / OS  │
        └──────────────────────┘

You should eventually understand every layer well enough to debug the layer below the one you normally work in.

---

0. The AI Engineer Mindset

Before technologies, develop the correct engineering instincts.

Stop thinking:

«"Which framework should I use?"»

Start thinking:

«"What problem am I solving, what are the constraints, and what is the simplest system that satisfies them?"»

For every AI system, ask:

- What is the objective?
- What is the input distribution?
- What is the output contract?
- What does "correct" mean?
- What is the acceptable latency?
- What is the expected throughput?
- What is the memory budget?
- What is the compute budget?
- What is the cost per request?
- What happens when the model fails?
- How do we evaluate regressions?
- How do we observe production behavior?
- Can the system be reproduced?
- What happens when traffic increases by 100×?

---

1. Programming Foundations

Goal

Become a software engineer who happens to specialize in AI.

Python

Learn:

- Variables and data types
- Functions
- Classes
- Exceptions
- Iterators
- Generators
- Decorators
- Context managers
- Type hints
- Dataclasses
- Modules and packages
- Virtual environments
- Dependency management
- Async programming
- Concurrency
- Multiprocessing
- Profiling
- Testing

Python ecosystem

Learn:

- "numpy"
- "pandas"
- "scipy"
- "polars"
- "pydantic"
- "pytest"
- "httpx"
- "asyncio"
- "typing"

Engineering practices

Learn:

- Clean code
- SOLID principles
- Design patterns
- Logging
- Configuration management
- Environment variables
- Error handling
- API contracts
- Unit tests
- Integration tests

Project

Build:

Production-style Python API

Requirements:

- FastAPI
- Pydantic
- PostgreSQL
- pytest
- Docker
- structured logging
- configuration management
- CI

---

2. Computer Science Fundamentals

AI engineers eventually hit systems problems.

You do not need to become a theoretical computer scientist, but you need strong engineering fundamentals.

Data Structures

Learn:

- Arrays
- Linked lists
- Stacks
- Queues
- Hash tables
- Trees
- Heaps
- Graphs
- Tries

Algorithms

Learn:

- Searching
- Sorting
- Graph traversal
- Dynamic programming
- Greedy algorithms
- Recursion
- Backtracking

Complexity

Understand:

O(1)
O(log n)
O(n)
O(n log n)
O(n²)

More importantly, understand why complexity matters in production systems.

Operating Systems

Learn:

- Processes
- Threads
- Scheduling
- Virtual memory
- Memory allocation
- File systems
- System calls
- IPC
- Signals
- Networking basics

Networking

Learn:

- TCP/IP
- DNS
- HTTP/HTTPS
- TLS
- REST
- WebSockets
- gRPC
- Load balancing
- Reverse proxies

---

3. Linux

AI infrastructure overwhelmingly runs on Linux.

Learn:

ssh
curl
wget
grep
sed
awk
find
xargs
top
htop
ps
kill
systemctl
journalctl
df
du
free
nvidia-smi

Understand:

- processes
- permissions
- environment variables
- filesystems
- services
- networking
- SSH
- shell scripting
- package management

GPU Linux

Learn:

- NVIDIA drivers
- CUDA
- CUDA runtime
- GPU memory
- GPU utilization
- "nvidia-smi"

You should be able to answer:

«Why is my GPU at 20% utilization while inference is slow?»

---

4. Git and Software Development

Learn Git beyond:

git add .
git commit
git push

Understand:

- branching
- rebasing
- merge conflicts
- cherry-picking
- tags
- releases
- semantic versioning
- conventional commits
- pull requests
- code review

Learn GitHub:

- Issues
- Projects
- Actions
- Releases
- Packages
- CI/CD

Standard

Every serious AI project should have:

README
LICENSE
requirements / pyproject
tests/
src/
configs/
scripts/
Dockerfile
CI
documentation

---

5. SQL and Data Engineering

AI systems are data systems.

Learn SQL deeply.

SQL

Learn:

- SELECT
- JOIN
- GROUP BY
- subqueries
- CTEs
- window functions
- indexes
- transactions
- query plans
- normalization
- denormalization

Databases

Understand:

- PostgreSQL
- Redis
- object storage
- NoSQL basics

Data pipelines

Learn:

Extract
   ↓
Validate
   ↓
Transform
   ↓
Store
   ↓
Version
   ↓
Serve

Understand:

- batch processing
- streaming
- ETL
- ELT
- data validation
- schema evolution
- data lineage

---

6. Mathematics for AI

Do not spend years proving mathematics before building.

Learn mathematics as required to understand models.

Linear Algebra

Master:

- vectors
- matrices
- tensors
- dot products
- matrix multiplication
- norms
- eigenvalues
- eigenvectors
- projections
- SVD

Calculus

Learn:

- derivatives
- partial derivatives
- gradients
- chain rule
- Jacobians
- optimization

Probability

Learn:

- probability distributions
- conditional probability
- Bayes theorem
- expectation
- variance
- covariance
- likelihood
- maximum likelihood

Statistics

Learn:

- sampling
- hypothesis testing
- confidence intervals
- regression
- correlation
- bias/variance

Optimization

Learn:

- gradient descent
- SGD
- Momentum
- Adam
- learning rates
- regularization
- convexity basics
- loss landscapes

---

7. Classical Machine Learning

Before becoming an LLM application developer, understand machine learning.

Learn:

Supervised learning

- Linear regression
- Logistic regression
- Decision trees
- Random forests
- Gradient boosting
- XGBoost
- LightGBM

Unsupervised learning

- K-means
- PCA
- clustering
- dimensionality reduction

ML fundamentals

Understand:

- train/validation/test splits
- cross-validation
- leakage
- feature engineering
- normalization
- class imbalance
- overfitting
- underfitting
- regularization

Metrics

Classification:

- accuracy
- precision
- recall
- F1
- ROC-AUC
- PR-AUC

Regression:

- MAE
- MSE
- RMSE
- R²

Ranking/retrieval:

- Precision@K
- Recall@K
- MRR
- NDCG

---

8. Deep Learning

Learn PyTorch.

Do not remain dependent on high-level abstractions.

PyTorch fundamentals

Learn:

- tensors
- autograd
- modules
- datasets
- dataloaders
- optimizers
- schedulers
- checkpoints
- mixed precision
- distributed training basics

Neural architectures

Understand:

- MLPs
- CNNs
- RNNs
- GRUs
- LSTMs
- attention
- Transformers

Training

Understand:

Dataset
   ↓
DataLoader
   ↓
Model
   ↓
Forward pass
   ↓
Loss
   ↓
Backward pass
   ↓
Optimizer
   ↓
Update weights

Be able to explain every step.

---

9. GPU and ML Systems Fundamentals

This is where an AI engineer starts separating from a notebook-only ML practitioner.

Understand:

- CPU vs GPU
- GPU memory
- VRAM
- HBM
- memory bandwidth
- FLOPs
- tensor cores
- CUDA
- kernels
- host/device transfer
- synchronization
- batching

Learn to inspect:

GPU utilization
GPU memory
CPU utilization
RAM
network
I/O
latency
throughput

Learn profiling

Understand:

- bottlenecks
- CPU-bound workloads
- GPU-bound workloads
- memory-bound workloads
- synchronization overhead

Learn tools such as:

- PyTorch Profiler
- Nsight Systems
- Nsight Compute
- NVIDIA SMI

---

10. Transformers

Transformers are mandatory for modern AI engineering.

Understand:

Architecture

Tokens
  ↓
Embeddings
  ↓
Positional Information
  ↓
Self Attention
  ↓
Feed Forward
  ↓
Residual + Normalization
  ↓
Repeated Blocks
  ↓
Output

Understand:

- queries
- keys
- values
- attention scores
- softmax
- multi-head attention
- causal masking
- positional encoding
- RoPE
- normalization
- residual connections

---

11. LLM Fundamentals

Understand what actually happens when an LLM generates a token.

Learn:

- tokenization
- vocabulary
- embeddings
- logits
- softmax
- sampling
- temperature
- top-k
- top-p
- greedy decoding
- beam search
- context window
- attention
- KV cache

Understand:

Prompt
 ↓
Tokenization
 ↓
Embeddings
 ↓
Transformer
 ↓
Logits
 ↓
Sampling
 ↓
Next token
 ↓
Repeat

Important concepts

Learn:

- pretraining
- instruction tuning
- supervised fine-tuning
- preference optimization
- RLHF
- DPO
- distillation
- quantization

---

12. Prompt Engineering

Prompt engineering is useful.

It is not the entire AI engineering discipline.

Learn:

- system instructions
- structured outputs
- few-shot prompting
- decomposition
- tool calling
- prompt templates
- prompt versioning
- prompt injection
- context management

But move quickly from:

«"How do I write a better prompt?"»

to:

«"How do I build a system that remains reliable when prompts, users and models change?"»

---

13. Context Engineering

Modern AI systems are increasingly constrained by the quality and management of context.

Learn:

- context windows
- context budgets
- context compression
- summarization
- retrieval
- conversation memory
- relevance filtering
- document selection
- prompt caching
- KV-cache awareness

Think of context as a finite engineering resource.

More context ≠ automatically better

Useful context
       ↓
Relevant context
       ↓
Well-structured context
       ↓
Better model performance

---

14. Embeddings

Understand embeddings rather than treating them as magic vectors.

Learn:

- vector representations
- semantic similarity
- cosine similarity
- dot product
- dimensionality
- embedding models
- embedding normalization
- multilingual embeddings

Understand when embeddings fail.

---

15. RAG

RAG should be learned as a retrieval system, not as:

vectorstore.similarity_search()

Pipeline

Documents
   ↓
Parsing
   ↓
Cleaning
   ↓
Chunking
   ↓
Embedding
   ↓
Index
   ↓
Query
   ↓
Retrieval
   ↓
Reranking
   ↓
Context construction
   ↓
LLM
   ↓
Answer

Learn:

Ingestion

- document parsing
- chunking
- metadata
- deduplication
- document versioning

Retrieval

- dense retrieval
- sparse retrieval
- BM25
- hybrid retrieval
- metadata filtering

Advanced retrieval

- reranking
- query expansion
- multi-query retrieval
- parent-child retrieval
- contextual retrieval
- graph-based retrieval

RAG evaluation

Measure:

- retrieval recall
- precision
- context relevance
- faithfulness
- answer correctness
- citation correctness

---

16. Vector Databases

Understand the underlying concepts before learning vendors.

Learn:

- ANN search
- HNSW
- IVF
- vector indexes
- filtering
- metadata
- namespaces
- collections
- indexing trade-offs

Explore:

- pgvector
- Qdrant
- Weaviate
- Milvus
- Pinecone

Do not memorize APIs.

Understand the indexing problem.

---

17. Tool Calling

Learn how models interact with external systems.

Understand:

User
 ↓
LLM
 ↓
Tool decision
 ↓
Tool invocation
 ↓
External system
 ↓
Tool result
 ↓
LLM
 ↓
Final response

Learn:

- function calling
- JSON schemas
- validation
- retries
- idempotency
- authentication
- permissions
- tool failure handling

---

18. AI Agents

An agent is more than:

while True:
    ask_llm()

Understand:

- state
- tools
- planning
- execution
- observation
- memory
- termination
- retries
- human approval
- failure recovery

Agent loop

Goal
 ↓
Reason / Plan
 ↓
Select Tool
 ↓
Execute
 ↓
Observe
 ↓
Update State
 ↓
Continue / Finish

Learn agent architectures:

- ReAct
- tool-use agents
- workflow agents
- state machines
- graph-based agents
- multi-agent systems

Frameworks

Understand at least one deeply:

- LangGraph
- OpenAI Agents SDK
- smolagents
- LlamaIndex

And understand how to build a simple agent without a framework.

---

19. MCP

Learn the Model Context Protocol.

Understand:

- MCP clients
- MCP servers
- tools
- resources
- prompts
- transport
- authentication
- permissions

The goal is not to memorize the protocol.

The goal is to understand standardized tool/data interfaces for AI systems.

---

20. Agent Security

Agents create a larger attack surface than ordinary APIs.

Learn:

- prompt injection
- indirect prompt injection
- tool poisoning
- excessive permissions
- data exfiltration
- insecure tool execution
- credential leakage
- sandboxing
- least privilege

Design tools with explicit permissions.

---

21. Evaluation Engineering

This is one of the most important AI engineering skills.

A demo answers:

«"Does it work?"»

An evaluation system answers:

«"Does it continue working after we change something?"»

Build evals for:

- correctness
- relevance
- groundedness
- hallucination
- tool selection
- tool arguments
- structured output
- safety
- latency
- cost

Evaluation hierarchy

Unit tests
    ↓
Component tests
    ↓
Model evaluations
    ↓
System evaluations
    ↓
Regression tests
    ↓
Production monitoring

Build an evaluation harness.

It should support:

Dataset
  ↓
Run system
  ↓
Collect outputs
  ↓
Score
  ↓
Compare versions
  ↓
Detect regression

---

22. LLM Observability

You cannot operate what you cannot see.

Track:

Application

- request count
- errors
- throughput
- latency

LLM

- input tokens
- output tokens
- model
- temperature
- cache hits
- tool calls

RAG

- retrieved documents
- retrieval scores
- reranker scores
- context size

Agents

- steps
- tool calls
- failures
- retries
- execution time

Infrastructure

- CPU
- RAM
- GPU utilization
- GPU memory
- network
- queue depth

Explore:

- OpenTelemetry
- MLflow
- Langfuse
- Arize Phoenix
- LangSmith

---

23. AI Cost Engineering

Production AI has an economic constraint.

Learn to calculate:

Cost / request
Cost / successful task
Cost / user
Cost / 1M tokens
GPU cost / hour
GPU utilization

Understand:

- token economics
- batching
- caching
- model selection
- prompt compression
- routing
- quantization
- smaller models
- asynchronous workloads

Example routing strategy

                  Request
                     │
          ┌──────────▼──────────┐
          │ Complexity classifier│
          └──────────┬──────────┘
                     │
        ┌────────────┼────────────┐
        ▼            ▼            ▼
     Small         Medium        Large
     Model         Model         Model

Do not use the largest model for every request.

---

24. Model Routing

Learn to route requests based on:

- complexity
- latency requirement
- cost
- context size
- modality
- reliability
- domain

Possible architecture:

Request
  ↓
Router
  ├── Fast model
  ├── Cheap model
  ├── Specialized model
  └── Reasoning model

Evaluate routing using actual workload data.

---

25. Fine-Tuning

Fine-tuning should not be the default answer to every model problem.

First determine whether the problem is caused by:

Prompt
Context
Retrieval
Tools
Model capability
Training data

Then choose an intervention.

Learn:

- supervised fine-tuning
- instruction tuning
- LoRA
- QLoRA
- PEFT
- adapters
- dataset formatting
- checkpointing
- gradient accumulation
- mixed precision

Understand:

- catastrophic forgetting
- overfitting
- data quality
- training/validation splits
- hyperparameters

Hugging Face's current training documentation describes fine-tuning as continuing training from pretrained weights rather than starting from random initialization.

---

26. Preference Optimization

Learn:

- RLHF
- reward models
- DPO
- preference datasets
- alignment objectives

Understand the difference between:

Supervised learning
Preference optimization
Reinforcement learning

---

27. Quantization

Learn why quantization matters.

Understand:

- FP32
- FP16
- BF16
- INT8
- INT4
- GPTQ
- AWQ
- activation quantization
- weight-only quantization

Trade-offs:

Memory ↓
Cost ↓
Latency potentially ↓
Accuracy potentially ↓

Measure the trade-off.

---

28. Inference Engineering

This is a major boundary between "AI app developer" and deeper AI engineering.

Understand:

- prefill
- decode
- KV cache
- batching
- continuous batching
- speculative decoding
- prefix caching
- quantization
- memory management
- scheduling

Key metrics

Learn:

- TTFT — Time To First Token
- TPOT — Time Per Output Token
- end-to-end latency
- throughput
- tokens/sec
- requests/sec
- queue time
- GPU utilization

---

29. Model Serving

Learn how models become network services.

Basic architecture

Client
  ↓
API Gateway
  ↓
Load Balancer
  ↓
Inference Server
  ↓
GPU
  ↓
Model

Explore:

- FastAPI
- vLLM
- NVIDIA Triton
- TensorRT-LLM
- Hugging Face TGI
- llama.cpp

vLLM currently supports both offline batched inference and online serving, including an OpenAI-compatible server interface.

---

30. vLLM

Learn vLLM beyond:

vllm serve model

Understand:

- continuous batching
- KV cache
- paged attention
- scheduling
- tensor parallelism
- quantization
- prefix caching
- OpenAI-compatible serving
- metrics
- throughput/latency trade-offs

Project

Deploy an open-source LLM with vLLM.

Benchmark:

Batch size
Concurrency
Input tokens
Output tokens
TTFT
TPOT
Total latency
Tokens/sec
GPU memory
Cost/request

Then optimize it.

---

31. NVIDIA Triton

Learn:

- model repositories
- model configuration
- dynamic batching
- model instances
- ensemble models
- metrics
- GPU utilization

Triton exposes request, execution, queue and compute timing metrics and can expose GPU/CPU metrics through Prometheus-compatible endpoints.

The important skill is not memorizing Triton configuration.

It is learning how serving architecture affects inference performance.

---

32. Distributed Inference

Learn when one GPU is insufficient.

Understand:

- data parallelism
- tensor parallelism
- pipeline parallelism
- expert parallelism
- distributed KV cache concepts
- communication overhead

Learn:

- NCCL
- multi-GPU communication
- GPU topology
- network bandwidth

---

33. Distributed Training

Understand:

Single GPU
   ↓
Data Parallel
   ↓
Distributed Data Parallel
   ↓
FSDP / ZeRO
   ↓
Multi-node training

Learn:

- DDP
- FSDP
- gradient accumulation
- gradient checkpointing
- mixed precision
- sharding
- checkpoint management

---

34. MLOps

MLOps connects experiments to production.

Learn:

Data
 ↓
Training
 ↓
Experiment tracking
 ↓
Evaluation
 ↓
Model registry
 ↓
Deployment
 ↓
Monitoring
 ↓
Retraining

Learn:

- experiment tracking
- model versioning
- data versioning
- model registry
- CI/CD
- reproducibility
- monitoring

Made With ML's production-oriented curriculum explicitly combines design, data, model development, testing, reproducibility, CI/CD, monitoring and production workflows.

---

35. Docker

Every AI engineer should be comfortable containerizing applications.

Learn:

- Dockerfiles
- images
- containers
- volumes
- networks
- multi-stage builds
- Docker Compose
- GPU containers

Project:

FastAPI
+
PostgreSQL
+
Redis
+
LLM service
+
Monitoring

Run the entire system using Docker Compose.

---

36. Kubernetes

Learn enough Kubernetes to deploy and operate AI services.

Understand:

- Pods
- Deployments
- Services
- ConfigMaps
- Secrets
- Ingress
- Jobs
- CronJobs
- Persistent Volumes
- HPA
- resource requests/limits

For AI workloads additionally understand:

- GPU scheduling
- GPU resource allocation
- node pools
- autoscaling
- model startup time

---

37. Cloud Infrastructure

Pick one cloud deeply.

AWS

Learn:

- EC2
- S3
- IAM
- VPC
- ECR
- ECS/EKS
- Lambda
- CloudWatch

OR:

GCP

Learn:

- Compute Engine
- Cloud Storage
- Artifact Registry
- GKE
- Cloud Run
- IAM
- Vertex AI

OR:

Azure

Learn:

- VMs
- Blob Storage
- AKS
- Container Registry
- Azure AI

Do not collect cloud certificates without deploying anything.

---

38. CI/CD for AI

Build pipelines that automatically:

Commit
 ↓
Lint
 ↓
Unit Tests
 ↓
Build
 ↓
Integration Tests
 ↓
Evaluation Suite
 ↓
Build Container
 ↓
Deploy
 ↓
Smoke Test

For AI systems add:

Model evaluation
Prompt regression
RAG regression
Latency benchmark
Cost benchmark

---

39. Production Architecture

Learn to design systems such as:

                    ┌─────────────┐
                    │    User     │
                    └──────┬──────┘
                           │
                    ┌──────▼──────┐
                    │ API Gateway │
                    └──────┬──────┘
                           │
                 ┌─────────▼─────────┐
                 │   AI Orchestrator │
                 └─────────┬─────────┘
                           │
          ┌────────────────┼────────────────┐
          │                │                │
          ▼                ▼                ▼
       Router             RAG             Tools
          │                │                │
          ▼                ▼                ▼
       Models          Vector DB       External APIs
          │
          ▼
      Inference
          │
          ▼
       GPU Pool
          │
          ▼
     Observability

---

40. Reliability Engineering

AI systems are probabilistic.

Traditional software often behaves like:

input → deterministic output

AI systems behave more like:

input → probabilistic output

Therefore learn:

- retries
- timeouts
- circuit breakers
- fallbacks
- idempotency
- graceful degradation
- validation
- rate limiting
- backpressure
- queues

Design for model failure.

---

41. AI Safety and Security

Learn:

- prompt injection
- jailbreaks
- data leakage
- insecure output handling
- model supply-chain risks
- malicious datasets
- tool abuse
- authentication
- authorization
- secrets management

For RAG:

- document-level permissions
- tenant isolation
- retrieval filtering

For agents:

- tool permissions
- sandboxing
- approval workflows
- action limits

---

42. Multimodal AI

After mastering language systems, explore:

Vision

- CNNs
- Vision Transformers
- image embeddings
- OCR
- vision-language models

Audio

- speech recognition
- speech synthesis
- audio embeddings
- speaker recognition

Video

- temporal modeling
- video embeddings
- multimodal reasoning

Multimodal LLMs

Understand:

Image
Text
Audio
Video
   ↓
Multimodal Encoder
   ↓
Shared Representation
   ↓
LLM / Decoder

---

43. AI Research Literacy

An AI engineer should be able to read papers.

Learn how to extract:

Problem
 ↓
Hypothesis
 ↓
Method
 ↓
Dataset
 ↓
Experiment
 ↓
Baseline
 ↓
Ablation
 ↓
Result
 ↓
Limitation

Learn to distinguish:

- benchmark improvement
- statistical significance
- ablation evidence
- engineering optimization
- marketing claims

Read papers from:

- NeurIPS
- ICML
- ICLR
- ACL
- CVPR
- MLSys
- arXiv

---

44. System Design for AI

Practice designing systems under constraints.

Examples:

Design a RAG system for 10M documents.

Consider:

- ingestion
- chunking
- embeddings
- indexing
- retrieval
- reranking
- storage
- caching
- evaluation
- access control

Design an LLM serving platform.

Consider:

- model registry
- GPU scheduling
- batching
- autoscaling
- routing
- observability
- cost

Design an AI coding agent.

Consider:

- repository indexing
- tool permissions
- context management
- execution sandbox
- tests
- patch generation
- evaluation
- rollback

---

45. Performance Engineering

Never optimize blindly.

Use:

Measure
 ↓
Profile
 ↓
Identify bottleneck
 ↓
Change one variable
 ↓
Benchmark
 ↓
Compare

Measure:

- latency
- throughput
- memory
- GPU utilization
- CPU utilization
- network
- token count
- cost

Example

If latency is 3 seconds:

Network        200 ms
Queue          300 ms
Prefill        700 ms
Decode         1.5 s
Postprocess    300 ms

Do not optimize the wrong component.

---

46. AI Caching

Learn multiple levels of caching.

Application cache

Cache:

- repeated requests
- expensive tool results
- database queries

Semantic cache

Cache semantically similar requests where appropriate.

Prompt/context caching

Reduce repeated processing of stable context.

Model-level caching

Understand:

- KV cache
- prefix caching
- response caching

Caching is a systems problem, not merely a dictionary.

---

47. Asynchronous AI Systems

Not every AI workload needs synchronous inference.

Learn:

User
 ↓
API
 ↓
Queue
 ↓
Worker
 ↓
Model
 ↓
Result

Explore:

- Redis
- Kafka
- RabbitMQ
- Celery
- background workers

Use asynchronous processing for:

- batch inference
- document ingestion
- large file processing
- report generation
- offline evaluation
- model jobs

---

48. Data and Model Versioning

Version:

Code
Data
Model
Prompt
Configuration
Evaluation
Infrastructure

A production result should be reproducible.

For example:

Model: v17
Prompt: v8
Dataset: v4
Retriever: v3
Embedding model: v2
Code: commit abc123

---

49. AI Product Engineering

AI engineering is not only model engineering.

Learn to define:

- user problem
- success metric
- failure metric
- latency budget
- cost budget
- quality threshold

Example:

Quality >= 90%
P95 latency <= 2.5 sec
Cost <= $0.01/request
Availability >= 99.9%

Engineering becomes much easier when constraints are explicit.

---

50. Advanced AI Systems

After mastering the previous layers, explore:

- mixture-of-experts
- speculative decoding
- retrieval-augmented generation variants
- long-context architectures
- model compression
- knowledge distillation
- synthetic data
- self-play
- test-time compute
- reasoning models
- multimodal agents
- distributed inference
- distributed training
- AI compiler stacks

---

51. Recommended Tool Stack

Do not learn every tool.

Learn concepts first.

Core

Python
Git
Linux
Docker
SQL
PostgreSQL
FastAPI

ML

NumPy
Pandas / Polars
Scikit-learn
PyTorch

LLM

Hugging Face
Transformers
Tokenizers
PEFT

RAG

pgvector
Qdrant
BM25
Rerankers

Agents

LangGraph
OpenAI Agents SDK
smolagents
MCP

Serving

vLLM
NVIDIA Triton
TensorRT-LLM
llama.cpp

MLOps

MLflow
Weights & Biases
DVC
Docker
GitHub Actions

Observability

OpenTelemetry
Prometheus
Grafana
Langfuse
Arize Phoenix

Cloud

AWS / GCP / Azure
Kubernetes
Terraform

---

52. Projects — Beginner

Build small systems first.

Project 1 — ML API

Dataset
 ↓
Train model
 ↓
FastAPI
 ↓
Docker
 ↓
Cloud deployment

Project 2 — Image classifier

Include:

- training
- evaluation
- API
- Docker
- monitoring

Project 3 — Search engine

Build:

- inverted index
- BM25
- semantic search
- ranking evaluation

---

53. Projects — Intermediate

Project 4 — Production RAG

Build a RAG system with:

- document ingestion
- chunking
- embeddings
- hybrid retrieval
- reranking
- citations
- evaluation
- observability
- authentication

---

Project 5 — Tool-Using Agent

Build an agent that can:

- search
- calculate
- query a database
- call an API
- produce a final report

Include:

- structured tool schemas
- retries
- permissions
- evaluation

---

Project 6 — Fine-Tuned Model

Build:

Base model
 ↓
Dataset
 ↓
LoRA / QLoRA
 ↓
Evaluation
 ↓
Quantization
 ↓
Deployment

Report:

- baseline
- fine-tuned result
- parameter count
- memory usage
- latency
- quality difference

---

54. Projects — Advanced

Project 7 — LLM Inference Benchmark

Serve the same model using multiple configurations.

Compare:

vLLM
Triton
llama.cpp

Measure:

- TTFT
- TPOT
- throughput
- concurrency
- VRAM
- CPU
- cost/request

Produce a technical report.

---

55. Project 8 — Model Router

Build:

                 Request
                    │
                    ▼
                 Router
             /      |      \
            /       |       \
       Cheap      Fast     Strong
       Model      Model     Model

Route based on:

- complexity
- latency
- token count
- cost
- task type

Evaluate against:

Always-small
Always-large
Router

---

56. Project 9 — AI Evaluation Platform

Build a system where developers can submit:

Prompt
Model
RAG configuration
Agent configuration

and automatically receive:

Accuracy
Faithfulness
Latency
Tokens
Cost
Failure rate

Include regression detection.

---

57. Project 10 — Production AI Platform

The capstone.

Build:

Frontend
   ↓
API Gateway
   ↓
Authentication
   ↓
AI Router
   ↓
┌──────────────┬───────────────┐
│              │               │
RAG          Agent          Direct LLM
│              │               │
└──────────────┴───────────────┘
               ↓
          Model Serving
               ↓
             vLLM
               ↓
              GPU

Add:

- PostgreSQL
- Redis
- vector database
- Docker
- Kubernetes
- CI/CD
- evaluation
- tracing
- metrics
- alerts
- cost tracking

---

58. The Portfolio Standard

Avoid:

"Built a chatbot using LangChain."

Prefer:

Built a production RAG service over 2M documents.

Reduced p95 latency from 4.2s → 1.7s
Reduced retrieval errors by 31%
Implemented hybrid BM25 + dense retrieval
Added reranking
Built 1,500-case evaluation suite
Deployed with Docker + Kubernetes
Added OpenTelemetry tracing

The second demonstrates engineering.

---

59. AI Engineer Competency Matrix

Area| Beginner| Intermediate| Advanced
Python| Scripts| Production APIs| Large systems
ML| Models| Pipelines| Research/optimization
PyTorch| Training| Custom architectures| Performance/distributed
LLMs| API usage| Applications| Model internals
RAG| Basic vector search| Hybrid + reranking| Retrieval research
Agents| Tool calling| Stateful agents| Reliable agent systems
Evaluation| Manual| Automated evals| Regression platform
Deployment| Docker| Cloud| Kubernetes/GPU infra
Inference| API calls| Serving| Optimization
vLLM| Basic serving| Benchmarking| Production tuning
GPUs| Usage| Profiling| Kernel/runtime optimization
MLOps| Tracking| CI/CD| Full lifecycle
Security| Basics| AI threats| Secure AI infrastructure
Systems| APIs| Distributed services| AI infrastructure
Cost| Awareness| Optimization| Architecture-level economics

---

60. Self-Assessment Checklist

You should be able to answer yes to these before calling yourself production-ready.

Software

- [ ] I can write production-quality Python.
- [ ] I understand async programming.
- [ ] I can design REST APIs.
- [ ] I can use SQL confidently.
- [ ] I can debug Linux systems.
- [ ] I can use Git professionally.
- [ ] I can write tests.
- [ ] I can containerize an application.

ML

- [ ] I understand classical ML.
- [ ] I understand neural networks.
- [ ] I can train a PyTorch model.
- [ ] I understand loss functions.
- [ ] I understand optimization.
- [ ] I can diagnose overfitting.
- [ ] I can design meaningful evaluations.

LLMs

- [ ] I understand tokenization.
- [ ] I understand attention.
- [ ] I understand Transformers.
- [ ] I understand KV cache.
- [ ] I understand decoding.
- [ ] I understand context windows.
- [ ] I understand embeddings.
- [ ] I understand fine-tuning.
- [ ] I understand quantization.

RAG

- [ ] I can design an ingestion pipeline.
- [ ] I understand chunking trade-offs.
- [ ] I understand dense retrieval.
- [ ] I understand BM25.
- [ ] I understand reranking.
- [ ] I can evaluate retrieval quality.
- [ ] I can debug bad retrieval.

Agents

- [ ] I understand tool calling.
- [ ] I can build an agent without a framework.
- [ ] I understand agent state.
- [ ] I understand retries and failure recovery.
- [ ] I understand MCP.
- [ ] I understand agent security.
- [ ] I can evaluate agent behavior.

Production

- [ ] I can deploy an AI API.
- [ ] I can use Docker.
- [ ] I understand CI/CD.
- [ ] I understand cloud infrastructure.
- [ ] I understand Kubernetes basics.
- [ ] I can add observability.
- [ ] I can measure production latency.
- [ ] I can monitor failures.

Inference

- [ ] I understand batching.
- [ ] I understand continuous batching.
- [ ] I understand prefill/decode.
- [ ] I understand KV caching.
- [ ] I can deploy with vLLM.
- [ ] I can benchmark inference.
- [ ] I understand TTFT.
- [ ] I understand TPOT.
- [ ] I can profile GPU utilization.
- [ ] I can reason about cost/latency trade-offs.

---

61. The Learning Order

Do not attempt to learn everything simultaneously.

Recommended order:

1. Python
      ↓
2. Computer Science
      ↓
3. Linux + Git
      ↓
4. SQL + Data
      ↓
5. Mathematics
      ↓
6. Classical ML
      ↓
7. PyTorch
      ↓
8. Deep Learning
      ↓
9. Transformers
      ↓
10. LLM Fundamentals
      ↓
11. RAG
      ↓
12. Tool Calling
      ↓
13. Agents
      ↓
14. Evaluation
      ↓
15. Deployment
      ↓
16. MLOps
      ↓
17. Inference
      ↓
18. GPU Optimization
      ↓
19. Distributed Systems
      ↓
20. Advanced AI Infrastructure

The later stages should increasingly become project-driven rather than course-driven.

---

62. The 70/20/10 Rule

A useful learning allocation:

70% Building
20% Reading / Documentation / Papers
10% Courses

Do not spend six months collecting certificates.

Build.

Break things.

Benchmark them.

Read the documentation.

Read the source code.

Profile the system.

Fix the bottleneck.

Repeat.

---

63. What NOT To Do

Avoid building your entire identity around:

- prompt engineering alone
- chatbot wrappers
- copying RAG tutorials
- blindly using agent frameworks
- collecting certificates
- deploying only Streamlit demos
- memorizing framework APIs
- calling every workflow an "agent"
- using the largest model by default
- fine-tuning without a baseline
- adding a vector database because "RAG needs one"
- adding Kubernetes because it looks impressive

Technology should follow the problem.

---

64. The Depth Test

A useful test for every technology:

Level 1 — User

«I can use it.»

Level 2 — Builder

«I can build with it.»

Level 3 — Debugger

«I can diagnose when it fails.»

Level 4 — Optimizer

«I can make it faster, cheaper or more reliable.»

Level 5 — Engineer

«I understand the trade-offs well enough to decide whether I should use it at all.»

Aim for Level 4–5 on your core stack.

---

65. The AI Engineer Stack

A mature AI Engineer should eventually be comfortable moving across this entire stack:

                    PRODUCT
                       │
                ┌──────▼──────┐
                │ AI Workflows│
                └──────┬──────┘
                       │
          ┌────────────▼────────────┐
          │ Agents / RAG / Tools    │
          └────────────┬────────────┘
                       │
          ┌────────────▼────────────┐
          │ Evaluation / Guardrails │
          └────────────┬────────────┘
                       │
          ┌────────────▼────────────┐
          │ Model Routing / APIs    │
          └────────────┬────────────┘
                       │
          ┌────────────▼────────────┐
          │ Inference / Serving     │
          └────────────┬────────────┘
                       │
          ┌────────────▼────────────┐
          │ GPU / CUDA / Runtime    │
          └────────────┬────────────┘
                       │
          ┌────────────▼────────────┐
          │ Cloud / Kubernetes      │
          └────────────┬────────────┘
                       │
          ┌────────────▼────────────┐
          │ Linux / Networking      │
          └────────────┬────────────┘
                       │
          ┌────────────▼────────────┐
          │ Software Engineering   │
          └─────────────────────────┘

---

66. Final Definition

You do not become an AI Engineer because you know:

«RAG + Agents + LLMs + LangChain.»

You become an AI Engineer when you can take:

A vague problem
      ↓
Requirements
      ↓
Architecture
      ↓
Data
      ↓
Model
      ↓
Application
      ↓
Evaluation
      ↓
Deployment
      ↓
Monitoring
      ↓
Optimization
      ↓
Scale

and make the system actually work.

A strong AI Engineer can answer:

«What should we build?»

«Why this model?»

«Why this architecture?»

«How do we know it works?»

«What happens when it fails?»

«How fast is it?»

«How much does it cost?»

«How does it behave at 10× traffic?»

«How do we monitor it?»

«How do we improve it?»

That is the standard this roadmap is designed to build toward.

---

Research Basis

This roadmap was synthesized from current AI/ML engineering roadmaps and primary technical learning/documentation sources rather than from a single roadmap.

Roadmaps

- "roadmap.sh — AI & Data Scientist Roadmap" (https://roadmap.sh/ai-data-scientist)
- "roadmap.sh — Developer Roadmaps" (https://roadmap.sh/get-started)
- "AI Engineer Roadmap — dswh" (https://github.com/dswh/ai-engineer-roadmap)
- "AI Engineer Roadmap 2026 — atryx" (https://github.com/atryx/ai-engineer-roadmap-2026)
- "Learning-Atlas — AI/ML Roadmap" (https://github.com/shamiquekhan/Learning-Atlas/blob/main/RoadMaps/AI-ML-Roadmap-Zero-to-Engineer.md)

Production ML / MLOps

- Made With ML — MLOps
- Full Stack Deep Learning
- MLflow documentation

LLMs / Agents

- Hugging Face Transformers
- Hugging Face LLM Course
- Hugging Face Agents Course
- Hugging Face MCP Course
- OpenAI developer documentation and cookbook

Inference / Systems

- vLLM documentation
- NVIDIA Triton Inference Server
- PyTorch documentation
- NVIDIA CUDA documentation

---

Relationship to the Existing Learning-Atlas Roadmap

The existing:

"AI-ML-Roadmap-Zero-to-Engineer.md"

should remain the foundational AI/ML learning path.

This roadmap is intentionally more engineering- and production-oriented.

AI-ML-Roadmap
     │
     │ foundations
     ▼
ML / DL / NLP / GenAI
     │
     ▼
AI Engineer Roadmap
     │
     ├── Production systems
     ├── RAG
     ├── Agents
     ├── Evaluation
     ├── MLOps
     ├── Inference
     ├── GPU systems
     ├── Optimization
     └── AI infrastructure

Together they form a broader path:

Learn the models → build the systems → measure them → deploy them → operate them → optimize them.
