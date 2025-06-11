# IJCAI Tutorial 2025; Evaluating LLM-based Agents: Foundations, Best Practices and Open Challenges

A Tutorial by **Roy Bar-Haim**, **Arman Cohan**, **Lilach Eden**, **Michal Shmueli-Scheuer**, and **Asaf Yehudai**

*Affiliations: The Hebrew University of Jerusalem, IBM Research, Yale University*

---

## Overview

The rapid advancement of Large Language Model (LLM)-based agents has sparked a growing interest in their evaluation, bringing forth both challenges and opportunities. This tutorial provides a comprehensive introduction to evaluating LLM-based agents, catering to participants from diverse backgrounds with little prior knowledge of agents, LLMs, metrics, or benchmarks.

We will establish foundational concepts and explore key benchmarks that measure critical agentic capabilities, including planning, tool use, self-reflection, and memory. We will examine evaluation strategies tailored to various agent types, ranging from web-based and software engineering to conversational and scientific applications. We will also cover benchmarks and leaderboards that evaluate generalist agents over diverse skill sets. Additionally, we will review prominent developer frameworks for agent evaluation. Finally, we will present emerging trends in the field, identify current limitations, and propose directions for future research.

## Tutorial Outline (Tentative)

The length of the tutorial is **half a day (3.5 hours)**.

### Part 1: Introduction to LLM Agent Evaluation (20 min)
*   **Preliminaries**: LLMs, Agent, LLM-as-a-Judge, Benchmarks
*   What are LLM-based Agents, and why are they important?
*   The shift from static LLMs to autonomous, interactive systems.
*   Why is reliable evaluation crucial for real-world deployment?

### Part 2: Evaluating Fundamental Agent Capabilities (40 min)
We will discuss the four main agentic capabilities: Planning and Multi-Step Reasoning, Function Calling & Tool Use, Self-Reflection, and Memory. For each of these capabilities, we will review:
*   Overview of the capability and its importance.
*   Challenges in evaluating the capability.
*   Common evaluation methodologies (datasets, metrics, benchmarks).
*   **Benchmark Examples**:
    *   **Planning and Multi-Step Reasoning**: `GSM8K`, `HotpotQA`, `PlanBench`.
    *   **Function Calling & Tool Use**: `ToolBench`, `API-Bank`, `BFCL`.
    *   **Self-Reflection**: `LLF-Bench`, `LLM-Evolve`.
    *   **Memory**: `ReadAgent`, `MemGPT`, `StreamBench`.

### Part 3: Evaluating Application-Specific Agents (45 min)
We will review prominent application-specific agents. For each type, we will cover:
*   Overview of the agent type, scope, tasks, and real-world applications.
*   Challenges in evaluating the agent type.
*   Common evaluation methodologies (datasets, metrics, environments).
*   **Benchmark Examples**:
    *   **Web Agents**: `MiniWob`, `WebShop`, `WebArena`.
    *   **Software Engineering Agents**: `HumanEval`, `SWE-bench`, `IT-Bench`.
    *   **Scientific Agents**: `ScienceQA`, `AAAR-1.0`, `CORE-Bench`.
    *   **Conversational Agents**: `MultiWOZ`, `ABCD`, `τ-Bench`.

### Part 4: Generalist Agent Evaluation (25 min)
*   Assessing diverse skills beyond specific applications.
*   **Benchmarks**: `GAIA`, `AgentBench`, `OSWorld`.
*   Focus on multi-step reasoning, problem-solving, and tool use.

### Part 5: Frameworks for Agent Evaluation (40 min)
*   Frameworks as tools for development, refinement, and continuous monitoring.
*   Evaluation features and capabilities in current frameworks:
    *   Multiple granularity levels.
    *   Data generation.
    *   A/B comparisons.
*   Main gaps in current capabilities.
*   Gym-like Environments: controlled, dynamic simulation environments.

### Part 6: Key Insights & Future Directions (25 min)
*   **Current Trends**: The shift towards challenging, realistic, and live benchmarks.
*   **Future Directions**:
    *   Granular evaluation with standardized metrics.
    *   Cost and efficiency metrics.
    *   Scaling and automating evaluation.
    *   Safety and compliance.
*   Applications of reliable agent evaluation in various industries.
*   Importance of responsible AI development and deployment.

### Part 7: Open Discussion (15 min)

---

## Target Audience and Prerequisites

This tutorial will present the current state-of-the-art and cutting-edge research, yet it will accommodate entry-level audiences.

**Prerequisites:**
1.  Familiarity with Large Language Models (LLMs) and their capabilities.
2.  A basic grasp of agents, including their roles and functionality.

**This tutorial is the best fit for:**
*   Researchers who are new to agent evaluation.
*   Researchers who have worked on a specific aspect of agent evaluation but are less familiar with the big picture.
*   Benchmark developers addressing evaluation challenges.
*   Practitioners deploying agents in domain-specific applications.
*   Researchers broadly studying current capabilities, risks, and limitations of LLM-based agents.

---

## Presenters

**Roy Bar-Haim** is a Senior Technical Staff Member at IBM Research, where he is currently leading research on agent evaluation. His research interests include the evaluation of language models and AI agents, large-scale analysis of opinions, and technologies for debating and persuasion. His work has been published in top journals and conferences, including AAAI, ACL, EMNLP, and JAIR. Roy received his Ph.D from Bar-Ilan University in 2010.

**Arman Cohan** is an Assistant Professor of Computer Science at Yale University. His research spans various problems at the intersection of Natural Language Processing and Machine Learning. His recent research interests include developing methods for better understanding and evaluating LLMs and improving LLMs' capabilities in specialized domains. His research has been recognized with multiple awards including a best paper at EMNLP and ACL.

**Lilach Eden** is a Research Staff Member in the Language Technologies group at IBM Research. Her areas of interest lie at the intersection of real-world applications and academic research in Natural Language Processing. Her work focuses on computational argumentation technologies, automatic opinion summarization, and generative AI evaluation, with her current research centered on agent evaluation. Lilach earned her M.Sc from The Hebrew University in 2020.

**Michal Shmueli-Scheuer** is a Principal Researcher in the Language Technologies department at IBM Research AI, leading efforts in GenAI Evaluation. Her expertise spans Natural Language Generation and Natural Language Processing, with a focus on efficient and robust evaluation. She has published in leading NLP and AI conferences and journals. Michal earned her Ph.D. from the University of California, Irvine, in 2009.

**Asaf Yehudai** is a Research Staff Member in NLP at IBM and a Ph.D. candidate at the Hebrew University. His research focuses on stress-testing and enhancing LLMs and agent capabilities, with publications in ACL, ICLR, NAACL, and EMNLP. He has also contributed to AI education and textbook development, combining academic rigor with practical advancements in NLP.

---

## Ethical Considerations

During the tutorial, we will explore the societal impacts of evaluating LLM-based agents, addressing both positive and negative implications. By promoting systematic evaluation methods, we aim to enhance AI reliability, transparency, and safety, fostering user trust and ensuring adherence to ethical guidelines. We will also examine potential unintended consequences. Evaluation tools, while designed to improve safety, could be misused to optimize deceptive models. Increased AI reliability may also accelerate workforce displacement, though it may simultaneously create new roles in AI evaluation, ethics, and governance. Additionally, high costs of evaluation frameworks could limit accessibility for smaller organizations, strain environmental resources, and widen innovation gaps. Finally, we will emphasize the importance of incorporating ethical and social dimensions, such as fairness and empathy, into the evaluation methodologies to ensure socially responsible AI development.

---

## Citation

The material in this tutorial is primarily based on our comprehensive survey paper. If you find this tutorial useful, please consider citing:

```bibtex
@misc{yehudai2025survey,
      title={Survey on Evaluation of LLM-based Agents}, 
      author={Asaf Yehudai and Lilach Eden and Alan Li and G. Uziel and Yilun Zhao and Roy Bar-Haim and Arman Cohan and Michal Shmueli-Scheuer},
      year={2025},
      eprint={2503.16416},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}