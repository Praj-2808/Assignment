# 🔍 ReSearch Project: Integrating Search and Reasoning with Reinforcement Learning

## 📘 Paper Reference
- **Title:** [ReSearch: Integrating Search and Reasoning with Reinforcement Learning for Large Language Models](https://arxiv.org/abs/2503.19470)
- **Authors:** Mingyang Chen et al.
- **Affiliations:** Baichuan Inc., Tongji University, University of Edinburgh, Zhejiang University
- **Summary:**  
  ReSearch is a novel framework that teaches Large Language Models (LLMs) to combine **external web search** with **internal multi-step reasoning** using **Reinforcement Learning (RL)**. It introduces **Group Relative Policy Optimization (GRPO)** — a critic-free, group-based policy optimization algorithm that rewards answer correctness and format consistency.

---

## 📦 Official Repository
- GitHub: [Agent-RL/ReSearch](https://github.com/Agent-RL/ReSearch)
- The repo includes:
  - Core GRPO algorithm
  - FlashRAG retriever setup
  - Training & evaluation scripts
  - Configs, prompt templates, and model checkpoints

---

## 🧠 Objective
This project focuses on:
- Understanding the **ReSearch paper and architecture**
- Exploring and analyzing the **official GitHub repo**
- Implementing and testing **baseline training with GRPO**
- Summarizing insights through slides and documentation

---

## 🔧 Implementation Highlights

✅ Reproduced baseline experiments  
✅ Understood and applied **GRPO** for training LLMs  
✅ Integrated reasoning steps with real-time retrieval  
✅ Ran training pipeline and generated sample outputs  

---

## 📊 Deliverables

### 🔹 Working Implementation
- Cloned and structured the ReSearch repo
- Installed dependencies (PyTorch, Hydra, FlashRAG)
- Set up reinforcement learning environment
- Ran GRPO training loop using `train_flashrag_rl.py`

### 🔹 Technical Summary Report
- Overview of the RL setup and reward structure
- GRPO explained:
  - Group-based comparison of multiple rollouts
  - No critic model required
- Results from generation and evaluation scripts
- Observations on rollout behavior, search frequency, and model strategy

### 🔹 Presentation Slides
- Covered motivation, key components, and architecture
- Walkthrough of <think>, <search>, <result>, and \boxed{} tags
- Visualized reasoning with search example
- Discussed results and future improvements

### 🔹 Discussion Points
| Model | Strength | Limitation |
|-------|----------|------------|
| **RAG** | Good at retrieval | Weak reasoning |
| **SFT** | Supervised reasoning | Needs labeled data |
| **ReSearch** | Autonomous reasoning via RL | Training cost, complexity |

- Future direction:
  - Connect with tools (calculator, browser)
  - Real-time retrieval APIs
  - Chain-of-thought + feedback loops

---

## 🧪 Benchmarks Used
- HotpotQA  
- 2WikiMultiHopQA  
- MuSiQue  
- Bamboogle  

These datasets test the model's ability to search and reason over **multiple steps**.


## 📌 License
- Based on the official ReSearch repository by Baichuan Inc.  
- Distributed under the **MIT License**

> Feel free to fork, modify, and extend this project for future research or academic work.

