# Hi, I'm Harsh Khatri 👋

**Lead Machine Learning Engineer** at [Logile](https://www.logile.com) · Boston, MA · M.S. Computer Science, Boston University (4.0 GPA)

I build ML systems that go to production. Right now that means **AI agents and LLM applications** (RAG, MCP tool-calling agents, LLM observability) and **transformer-based demand forecasting** for retail. I've been in industry for over 5 years: I started as a software engineer on enterprise analytics products, then did computer vision research at BU before moving into applied ML. I like work where training the model and engineering the system around it both matter.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/harsh242/)
[![Website](https://img.shields.io/badge/Website-222222?style=flat-square&logo=githubpages&logoColor=white)](https://harshk242.github.io/)
[![Substack](https://img.shields.io/badge/Substack-FF6719?style=flat-square&logo=substack&logoColor=white)](https://thedlcompass.substack.com/)
[![X](https://img.shields.io/badge/X-000000?style=flat-square&logo=x&logoColor=white)](https://x.com/harshkhatri242)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:harshkhatri242@gmail.com)

---

## What I work on

- **Enterprise agent platform:** I architected and shipped a shared agent harness built on LangGraph, with three agents running on it:
  - a **RAG agent** over docs, tickets, SharePoint and wikis that cut knowledge-search time by 93%;
  - an **employee self-service agent** built on workforce APIs through an MCP client / MCP server architecture, with 54 tools covering scheduling, availability, timesheets and staffing;
  - a **Text-to-SQL analytics agent** that uses a semantic layer and SQL guardrails.

  The harness handles identity and least-privilege tool access, typed delegation to sub-agents, and human approval before any write action. It also produces one Langfuse trace per turn, which helped cut hallucinations by 16%.
- **Agent evaluation & improvement flywheel:** I built a complete evaluation pipeline for these agents. It starts by tracing every turn. Next it surfaces the traces worth reading: user feedback, frustration signals, outliers, clusters and a random sample. Errors from those traces become a failure taxonomy, which drives reference datasets and rubrics. Scoring goes from code checks to LLM-as-judge, with the judge calibrated against human labels. Each round's findings feed the next, so the agents keep improving.
- **Forecasting at scale:** a transformer-based demand-forecasting model (+8%) trained with mixed precision on multiple GPUs. I also re-engineered a legacy pipeline so it runs 60% faster at half the cost.
- **Computer vision & 3D:** research at BU on open-vocabulary 3D recognition, sim-to-real point-cloud classification, and synthetic training data from diffusion models.

## Featured projects

| Project | What it is | Context |
|---|---|---|
| [**BURP**](https://github.com/harshk242/burp) | A biomedical research agent that chains 10 public databases (UniProt, ChEMBL, Open Targets, ClinicalTrials.gov, …), maps identifiers between them, and cites every claim. Live at [tryburp.com](https://tryburp.com). | Personal · TypeScript, MCP, Vercel AI SDK, Langfuse |
| [**my-agent-skills**](https://github.com/harshk242/my-agent-skills) | Agent skills I wrote for my own Claude Code workflow (structured HTML artifacts, multi-article synthesis, WhisperX transcription with diarization). | Personal · Agents tooling |
| [**OpenShape3D**](https://github.com/harshk242/OpenShape3D) | A failure analysis of OpenShape, a zero-shot 3D shape recognizer: why it confuses categories, with coarse-to-fine fine-tuning, linear probes and hard-negative mining as fixes. | M.S. research, BU IVC Lab · PyTorch, CLIP |
| [**sim2real-3d-classification**](https://github.com/harshk242/sim2real-3d-classification) | Took a point-cloud classifier's accuracy on real scans from 9.4% to 59.1% while training only on synthetic CAD data. | M.S. project, BU · CurveNet, point clouds |
| [**synthetic-face-attributes**](https://github.com/harshk242/synthetic-face-attributes) | Generate faces with Stable Diffusion → filter them with few-shot foundation-model features → train a ResNet. Scores 99.5% on synthetic data and 82.3% on real photos it never trained on. | CV internship, Wicket |
| [**robot-learning**](https://github.com/harshk242/robot-learning) | Teaching a car to drive in CarRacing three ways: imitation learning + DAgger, a modular perception-and-control pipeline, and RL with DQN and PPO. | M.S. coursework, BU · PyTorch, Gym |

## Skills

**ML / AI:** AI agents, agent harness design, agent evaluation, RAG, context engineering, LLM observability, Text-to-SQL, transformers, time-series forecasting, deep learning, computer vision, multimodal learning<br>
**Frameworks:** PyTorch, Lightning, LangChain, LangGraph, MCP, Langfuse, OpenCV, MLflow, Prefect<br>
**Languages:** Python, TypeScript/JavaScript, Java, C++, SQL<br>
**Infra & data:** AWS (Batch, S3, EC2, ECR, Athena), GCP, Docker, CI/CD, PostgreSQL + pgvector, Iceberg, Superset

## Publications

- Co-author of two multi-omics studies of COVID-19 patient severity (proteomics + metabolomics, ML classification). IIT Bombay, 2021.

---

<sub>I write about deep learning at <a href="https://thedlcompass.substack.com/">The DL Compass</a>.</sub>
