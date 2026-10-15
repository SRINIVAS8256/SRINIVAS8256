<!--
PROFILE README SETUP
1. Create a PUBLIC repository named exactly SRINIVAS8256.
2. Add this README.md to the repository root.
3. Add .github/workflows/snake.yml from your pack.
4. In Settings → Actions → General, allow workflows to write to the repository.
5. Run "Generate contribution snake" from Actions once.
-->

<div align="center">

<a href="https://github.com/SRINIVAS8256">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=27&duration=2800&pause=800&color=36BCF7&center=true&vCenter=true&width=850&lines=Hi%2C+I'm+Srinivas+DR+%F0%9F%91%8B;AI%2FML+%7C+Data+Science+%7C+Python;Building+intelligent%2C+data-driven+systems;From+raw+data+to+production-minded+AI" alt="Typing SVG"/>
</a>


<a href="https://leetcode.com/u/Srinivas_DR_8256/"><img src="https://img.shields.io/badge/LeetCode-Srinivas__DR__8256-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode"/></a>
<a href="mailto:srinivasdr25@gmail.com"><img src="https://img.shields.io/badge/Email-Contact%20me-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
<a href="https://github.com/SRINIVAS8256"><img src="https://img.shields.io/badge/GitHub-Building%20in%20public-181717?style=for-the-badge&logo=github" alt="GitHub"/></a>
<a href="https://wondrous-kheer-38ca1e.netlify.app"><img src="https://img.shields.io/badge/Portfolio-Visit%20my%20website-0A66C2?style=for-the-badge&logo=netlify&logoColor=white" alt="Portfolio"/></a>
<img src="https://komarev.com/ghpvc/?username=SRINIVAS8256&style=for-the-badge&color=blueviolet" alt="Profile views"/>

</div>

> whoami
I'm Srinivas DR, a Computer Science Engineering student focused on AI/ML, Data Science, and Python engineering. I’m interested in building complete intelligent systems—from exploring data and training models to serving model-powered features through reliable backend APIs.
- 🤖 Primary focus: AI/ML · Data Science · Generative AI
- 🐍 Engineering: Python · REST APIs · FastAPI · SQL
- 🧪 ML toolkit: NumPy · Pandas · scikit-learn · model evaluation
- 🧠 Exploring: Multimodal RAG · streaming fraud detection · LLM fine-tuning with LoRA/QLoRA
- 🏆 Hackathons: 1st place at Xypher ML Hackathon; 6th at MITM 2025 Hackathon; 12th at Atria Institute of Technology hackathon
- 🎓 Education: B.E. Computer Science, Maharaja Institute of Technology, Mysore — expected 2027
- 🎯 Goal: Build AI systems that are measurable, reliable, useful, and deployable.
My approach: Understand the problem → inspect the data → build a baseline → evaluate rigorously → expose it through an API → monitor and improve.

⚡ Tech stack
<div align="center">

<img src="https://skillicons.dev/icons?i=python,fastapi,mysql,docker,git,github,linux&perline=7" alt="Python, FastAPI, MySQL, Docker, Git, GitHub and Linux"/>




<img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" alt="NumPy"/>
<img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="Pandas"/>
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn"/>
<img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" alt="Apache Kafka"/>
<img src="https://img.shields.io/badge/GenAI%20%26%20RAG-Exploring-7B61FF?style=flat-square" alt="GenAI and RAG"/>
<img src="https://img.shields.io/badge/LoRA%20%2F%20QLoRA-LLM%20Fine--Tuning-0A7E8C?style=flat-square" alt="LoRA and QLoRA"/>

</div>

<details>
<summary><b>🧭 Technical areas</b></summary>
<br/>

Track	Focus
AI / Machine Learning	Supervised and unsupervised learning, regression, classification, clustering, ensembles, tuning, model evaluation
Data Science	EDA, data cleaning, feature engineering, statistics, visualization, communicating findings
Python & Backend Engineering	Python, FastAPI, REST API design, validation, database integration, testing, error handling
Generative AI	LLM applications, prompt engineering, RAG, embeddings, multimodal retrieval, NLP
LLM Adaptation	Parameter-efficient fine-tuning concepts including LoRA and QLoRA
Streaming Data	Apache Kafka concepts for event-driven and real-time data pipelines
Engineering & Delivery	Git/GitHub, Docker, CI basics, model serving, MLOps fundamentals
Problem solving	Python, arrays, strings, linked lists, stacks, queues, searching and sorting


</details>

🚀 Featured AI projects
These are the three project directions I’m focusing on. The descriptions below define a strong engineering scope; update each section with implementation details, benchmarks, and repository links as the projects are built and validated.

01 · Multimodal RAG System
Python · FastAPI · LLMs · Embeddings · Vector Search · OCR/Vision
Build a retrieval-augmented generation pipeline that can answer questions grounded in mixed-format knowledge sources such as PDFs, text, tables, and images.
- Ingestion and parsing: Extract text and document structure; process scanned pages with OCR and image content with suitable vision models. Preserve page, section, and source metadata for traceability.
- Multimodal representation: Generate embeddings for supported text and visual content, and store them with metadata in a searchable vector index. Use modality-appropriate encoders rather than assuming one embedding model fits every input.
- Retrieval and ranking: Retrieve candidate passages or image-linked chunks, apply metadata filters, and optionally rerank candidates to improve relevance before generation.
- Grounded generation: Assemble context-aware prompts, instruct the model to answer from retrieved evidence, and return citations or source references so users can inspect supporting material.
- Evaluation: Build a representative question set and measure retrieval quality (for example, Recall@K and MRR), answer faithfulness, citation correctness, latency, and failure cases. Compare baseline retrieval against improved chunking or reranking.
- Backend design: Expose ingestion and query workflows through FastAPI, validate requests, handle long-running jobs, log failures, and keep secrets outside source control.
Engineering objective: Make answers traceable to source evidence and evaluate retrieval and generation separately—not just demonstrate a chatbot that appears to work.
02 · Real-Time UPI Fraud Detection with Apache Kafka
Python · Apache Kafka · Stream Processing · Machine Learning · FastAPI
Design an event-driven fraud detection pipeline that scores transaction events as they arrive and makes risk decisions with low latency.
- Event ingestion: Publish transaction-shaped events to Kafka topics using a documented schema, event identifiers, timestamps, and schema/version handling. Use synthetic or properly authorized data; do not imply access to private live UPI transactions.
- Streaming pipeline: Consume events, validate and normalize fields, handle malformed messages, and manage retries and dead-letter events. Design for duplicate delivery and idempotent downstream processing.
- Fraud scoring: Apply a trained classifier or rules-plus-model approach to produce a risk score and decision. Avoid target leakage and use time-aware validation to reflect production conditions.
- Class imbalance: Evaluate precision, recall, PR-AUC, false-positive rate, and recall at a chosen alert budget—not accuracy alone. Tune thresholds according to the cost of missed fraud versus legitimate transactions being blocked.
- Serving and review: Expose scoring or alert-review functionality through FastAPI, store decisions and audit metadata, and make it possible to trace an alert back to its input event.
- Reliability and observability: Track consumer lag, throughput, processing latency, error rate, model version, and decision distribution. Test replay, duplicate events, late events, and service restarts.
Engineering objective: Demonstrate a reproducible streaming fraud-detection system with measurable latency and model quality. For a portfolio demo, clearly label generated transactions as simulated.
03 · LLM Fine-Tuning with LoRA / QLoRA
Python · Hugging Face · Transformers · PEFT · PyTorch
Explore parameter-efficient adaptation of a pretrained language model for a clearly defined task, while keeping experiments reproducible and evaluating whether fine-tuning actually improves results.
- Task and dataset design: Define the target behavior, prepare high-quality instruction/response examples, remove sensitive data, deduplicate records, and create leakage-resistant train/validation/test splits.
- Baseline first: Evaluate the original model with a fixed prompt and test set before fine-tuning. Define task-specific quality measures and representative qualitative checks.
- LoRA adaptation: Configure low-rank trainable adapters on selected model modules while freezing the base weights; document rank, alpha, dropout, target modules, sequence length, and training settings.
- QLoRA experiment: Where hardware and model support permit, load a quantized base model and train adapters to reduce memory requirements. Record quantization configuration, precision, hardware, and any limitations.
- Evaluation and comparison: Compare base model, prompt-only baseline, and fine-tuned variants on the same held-out examples. Report quality, hallucination or failure patterns, inference latency, memory usage, and training cost where measured.
- Reproducibility and serving: Version datasets/configurations, save adapter artifacts and evaluation results, document limitations, and optionally serve the selected model behind a Python/FastAPI endpoint.
Engineering objective: Show evidence that the adaptation improves the chosen task at an acceptable compute and quality cost. Never claim performance gains until they are measured on a held-out evaluation set.
📊 GitHub telemetry
<div align="center">

<a href="https://github.com/SRINIVAS8256">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=SRINIVAS8256&show_icons=true&rank_icon=github&hide_border=true&theme=tokyonight&include_all_commits=true" alt="GitHub stats"/>
</a>
<a href="https://github.com/SRINIVAS8256">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=SRINIVAS8256&layout=compact&langs_count=8&hide_border=true&theme=tokyonight" alt="Top languages"/>
</a>


<img src="https://streak-stats.demolab.com?user=SRINIVAS8256&theme=tokyonight&hide_border=true" alt="GitHub contribution streak"/>


</div>

🐍 Animated contribution calendar
<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/SRINIVAS8256/SRINIVAS8256/output/github-contribution-grid-snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/SRINIVAS8256/SRINIVAS8256/output/github-contribution-grid-snake.svg"/>
  <img alt="Animated GitHub contribution snake" src="https://raw.githubusercontent.com/SRINIVAS8256/SRINIVAS8256/output/github-contribution-grid-snake.svg"/>
</picture>

</div>

🧩 LeetCode
<div align="center">

<a href="https://leetcode.com/u/Srinivas_DR_8256/">
  <img src="https://leetcard.jacoblin.cool/Srinivas_DR_8256?theme=dark&font=Fira%20Code&ext=heatmap" alt="LeetCode profile card"/>
</a>


<a href="https://leetcode.com/u/Srinivas_DR_8256/">
  <img src="https://img.shields.io/badge/LeetCode-View%20my%20profile-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="View LeetCode profile"/>
</a>

</div>

🌱 Current goals
- Strengthen foundations in ML, statistics, and data analysis.
- Build useful AI systems with careful evaluation and clear failure handling.
- Develop reliable Python backends for model-powered applications.
- Learn streaming architecture and event-driven data processing.
- Run reproducible LoRA/QLoRA experiments and report honest results.
- Contribute consistently and keep improving through feedback.
🤝 Connect
<div align="center">

<a href="mailto:srinivasdr25@gmail.com"><img src="https://img.shields.io/badge/Email-srinivasdr25%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
<a href="https://leetcode.com/u/Srinivas_DR_8256/"><img src="https://img.shields.io/badge/LeetCode-Srinivas__DR__8256-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode"/></a>
<a href="https://github.com/SRINIVAS8256"><img src="https://img.shields.io/badge/GitHub-Follow%20my%20work-181717?style=for-the-badge&logo=github" alt="GitHub"/></a>
<a href="https://wondrous-kheer-38ca1e.netlify.app"><img src="https://img.shields.io/badge/Portfolio-Visit%20my%20portfolio-0A66C2?style=for-the-badge&logo=netlify&logoColor=white" alt="Portfolio"/></a>
</div>

<div align="center">

Build with curiosity. Validate with evidence. Ship with purpose.
<img src="https://capsule-render.vercel.app/api?type=waving&height=100&section=footer&color=gradient" alt="Animated footer"/>

</div>
