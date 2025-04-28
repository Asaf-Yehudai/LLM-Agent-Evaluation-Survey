<div align="center">
<h1>Evaluation of LLM-based Agents: A Reading List</h1>
</div>

<div align="center">
  Based on the Survey Paper: <br />
  <b>Survey on Evaluation of LLM-based Agents</b> (arXiv 2025)
</div>

<div align="center">
  <b>Asaf Yehudai¹, Lilach Eden², Alan Li³, Guy Uziel², Yilun Zhao³, Roy Bar-Haim², Arman Cohan³, Michal Shmueli-Scheuer²</b><br />
  <small>¹The Hebrew University of Jerusalem | ²IBM Research | ³Yale University</small>
</div>
<br />

<div align="center">
    <!-- === UPDATE LINKS === -->
    <a href="https://arxiv.org/abs/2503.16416"><img src="https://img.shields.io/badge/arXiv-2503.16416-b31b1b" alt="Paper"></a>
    <a href="https://github.com/YOUR_USERNAME/YOUR_REPONAME"><img src="https://img.shields.io/github/last-commit/YOUR_USERNAME/YOUR_REPONAME?color=blue" alt="Github Last Commit"></a>
    <a href="https://github.com/YOUR_USERNAME/YOUR_REPONAME/blob/main/LICENSE"> <img alt="License" src="https://img.shields.io/github/license/YOUR_USERNAME/YOUR_REPONAME?color=green"> </a>
    <!-- === UPDATE LINKS === -->
</div>

### About This Repository

This repository serves as a companion to the survey paper **"Survey on Evaluation of LLM-based Agents"**. It organizes evaluation methodologies, benchmarks, and frameworks according to the structure presented in the paper, aiming to provide a comprehensive resource for researchers and practitioners in the field of LLM-based agents.

The selection criteria focus on works discussed within the survey, covering:
- **Fundamental Agent Capabilities:** Planning, Tool Use, Self-Reflection, Memory.
- **Application-Specific Domains:** Web, Software Engineering, Scientific, Conversational Agents.
- **Generalist Agent Evaluation.**
- **Evaluation Frameworks.**

Our goal is to map the rapidly evolving landscape of agent evaluation, highlight key trends, and identify current limitations as discussed in the survey.

*(Note: The initial version is based on arXiv:2503.16416v1 dated 20 Mar 2025. It will be updated as the survey evolves or upon publication.)*

### Other Relevant Repositories

While this repository mirrors our survey's scope, other excellent repositories cover LLM Agents more broadly or from different angles:

*General LLM Agent Papers:*
* [AGI-Edgerunners/LLM-Agents-Papers](https://github.com/AGI-Edgerunners/LLM-Agents-Papers) <a href="https://github.com/AGI-Edgerunners/LLM-Agents-Papers"><img src="https://img.shields.io/github/last-commit/AGI-Edgerunners/LLM-Agents-Papers?color=blue" alt="Github"></a>
* [zjunlp/LLMAgentPapers](https://github.com/zjunlp/LLMAgentPapers) <a href="https://github.com/zjunlp/LLMAgentPapers"><img src="https://img.shields.io/github/last-commit/zjunlp/LLMAgentPapers?color=blue" alt="Github"></a>
* [Paitesanshi/LLM-Agent-Survey](https://github.com/Paitesanshi/LLM-Agent-Survey) <a href="https://github.com/Paitesanshi/LLM-Agent-Survey"><img src="https://img.shields.io/github/last-commit/Paitesanshi/LLM-Agent-Survey?color=blue" alt="Github"></a>
* [woooodyy/llm-agent-paper-list](https://github.com/woooodyy/llm-agent-paper-list) <a href="https://github.com/woooodyy/llm-agent-paper-list"><img src="https://img.shields.io/github/last-commit/woooodyy/llm-agent-paper-list?color=blue" alt="Github"></a>
* [xinzhel/llm-agent-survey](https://github.com/xinzhel/llm-agent-survey) <a href="https://github.com/xinzhel/llm-agent-survey"><img src="https://img.shields.io/github/last-commit/xinzhel/llm-agent-survey?color=blue" alt="Github"></a>

*Specific Focus Repositories:*
* [LLM-Search](https://github.com/xinzhel/LLM-Search) (Search/Inference) <a href="https://github.com/xinzhel/LLM-Search"><img src="https://img.shields.io/github/last-commit/xinzhel/LLM-Search?color=blue" alt="Github"></a>
* [nuster1128/LLM_Agent_Memory_Survey](https://github.com/nuster1128/LLM_Agent_Memory_Survey) (Memory) <a href="https://github.com/nuster1128/LLM_Agent_Memory_Survey"><img src="https://img.shields.io/github/last-commit/nuster1128/LLM_Agent_Memory_Survey?color=blue" alt="Github"></a>
* [teacherpeterpan/self-correction-llm-papers](https://github.com/teacherpeterpan/self-correction-llm-papers) (Self-Correction) <a href="https://github.com/teacherpeterpan/self-correction-llm-papers"><img src="https://img.shields.io/github/last-commit/teacherpeterpan/self-correction-llm-papers?color=blue" alt="Github"></a>
* [git-disl/awesome-LLM-game-agent-papers](https://github.com/git-disl/awesome-LLM-game-agent-papers) (Gaming) <a href="https://github.com/git-disl/awesome-LLM-game-agent-papers"><img src="https://img.shields.io/github/last-commit/git-disl/awesome-LLM-game-agent-papers?color=blue" alt="Github"></a>

## Table of Contents
- [:gift: Surveys](#gift-surveys)
- [:wrench: Agent Capabilities Evaluation (§2)](#wrench-agent-capabilities-evaluation-§2)
  - [:world_map: Planning and Multi-Step Reasoning (§2.1)](#world_map-planning-and-multi-step-reasoning-§21)
  - [:telephone_receiver: Function Calling & Tool Use (§2.2)](#telephone_receiver-function-calling--tool-use-§22)
  - [:thinking: Self-Reflection (§2.3)](#thinking-self-reflection-§23)
  - [:floppy_disk: Memory (§2.4)](#floppy_disk-memory-§24)
- [:dart: Application-Specific Agent Evaluation (§3)](#dart-application-specific-agent-evaluation-§3)
  - [:globe_with_meridians: Web Agents (§3.1)](#globe_with_meridians-web-agents-§31)
  - [:computer: Software Engineering Agents (§3.2)](#computer-software-engineering-agents-§32)
  - [:microscope: Scientific Agents (§3.3)](#microscope-scientific-agents-§33)
  - [:speech_balloon: Conversational Agents (§3.4)](#speech_balloon-conversational-agents-§34)
- [:earth_africa: Generalist Agents Evaluation (§4)](#earth_africa-generalist-agents-evaluation-§4)
- [:building_construction: Frameworks for Agent Evaluation (§5)](#building_construction-frameworks-for-agent-evaluation-§5)
- [:chart_with_upwards_trend: Discussion (§6)](#chart_with_upwards_trend-discussion-§6)
  - [Trends & Directions](#trends--directions)
- [:memo: Citation](#memo-citation)
- [:star: Star History](#star-star-history)


## :gift: Surveys
*   **Survey on Evaluation of LLM-based Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2503.16416) *(This work)*
*   **A Survey on Large Language Model based Autonomous Agents**, arXiv 2023 / FCS 2024 [[paper]](https://arxiv.org/abs/2308.11432)
*   **The Rise and Potential of Large Language Model Based Agents: A Survey**, arXiv 2023 [[paper]](https://arxiv.org/abs/2309.07864)
*   **Understanding the planning of LLM agents: A survey**, arXiv 2024 [[paper]](https://arxiv.org/abs/2402.02716)
*   **A Survey on the Memory Mechanism of Large Language Model based Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2404.13501)

## :wrench: Agent Capabilities Evaluation (§2)

### :world_map: Planning and Multi-Step Reasoning (§2.1)
*   **AQUA-RAT: An Analytics Question Answering Benchmark for Tabular Data**, arXiv 2017 [[paper]](https://arxiv.org/abs/1705.08207)
*   **HotpotQA: A Dataset for Diverse, Explainable Multi-hop Question Answering**, EMNLP 2018 [[paper]](https://arxiv.org/abs/1809.09600)
*   **Think you have Solved Question Answering? Try ARC, the AI2 Reasoning Challenge**, arXiv 2018 [[paper]](https://arxiv.org/abs/1803.05457)
*   **StrategyQA: A Question Answering Benchmark with Implicit Reasoning Strategies**, TACL 2021 [[paper]](https://aclanthology.org/2021.tacl-1.49/)
*   **Measuring Mathematical Problem Solving With the MATH Dataset**, NeurIPS 2021 [[paper]](https://arxiv.org/abs/2103.03874)
*   **GSM8K: A Dataset of Grade School Math Word Problems**, arXiv 2021 [[paper]](https://arxiv.org/abs/2110.14168)
*   **Tree of Thoughts: Deliberate Problem Solving with Large Language Models**, NeurIPS 2023 [[paper]](https://arxiv.org/abs/2305.10601)
*   **MINT: Evaluating LLMs in Multi-turn Interaction with Tools and Language Feedback**, arXiv 2023 [[paper]](https://arxiv.org/abs/2309.10691)
*   **PlanBench: An Extensible Benchmark for Evaluating Large Language Models on Planning and Reasoning about Change**, NeurIPS 2023 [[paper]](https://arxiv.org/abs/2306.08648)
*   **FlowBench: Revisiting and Benchmarking Workflow-Guided Planning for LLM-based Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.14884)
*   **FOLIO: Natural Language Reasoning with First-Order Logic**, EMNLP 2022 Findings [[paper]](https://aclanthology.org/2022.findings-emnlp.318/)
*   **P-FOLIO: Evaluating and Improving Logical Reasoning with Abundant Human-Written Reasoning Chains**, EMNLP 2024 Findings [[paper]](https://arxiv.org/abs/2404.06079)
*   **MultiRC: Reading Comprehension over Multiple Sentences**, EMNLP 2018 [[paper]](https://aclanthology.org/D18-1068/)
*   **MUSR: Testing the Limits of Chain-of-Thought with Multistep Soft Reasoning**, arXiv 2023 [[paper]](https://arxiv.org/abs/2310.16049)
*   **Challenging BIG-Bench Tasks and Whether Chain-of-Thought Can Solve Them**, arXiv 2022 [[paper]](https://arxiv.org/abs/2210.09261)
*   **ToolEmu: An Instruction-tuning Benchmark for Tool-augmented Agents**, arXiv 2023 (*Link seems missing in source PDF*)
*   **AutoPlanBench: Automatically Generating Benchmarks for LLM Planners from PDDL**, arXiv 2023 [[paper]](https://arxiv.org/abs/2311.09830)
*   **ACPBench: Reasoning about Action, Change, and Planning**, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.05669)
*   **Natural Plan: Benchmarking LLMs on Natural Language Planning**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.04520)

### :telephone_receiver: Function Calling & Tool Use (§2.2)
*   **BFCL: Berkeley Function Calling Leaderboard**, Blog Post 2024 [[link]](https://gorilla.cs.berkeley.edu/blogs/8_berkeley_function_calling_leaderboard.html)
*   **ToolLLM: Facilitating Large Language Models to Master 16000+ Real-world APIs**, arXiv 2023 [[paper]](https://arxiv.org/abs/2307.16789)
*   **ToolAlpaca: Generalized Tool Learning for Language Models with 3000 Simulated Cases**, arXiv 2023 [[paper]](https://arxiv.org/abs/2306.05301)
*   **APIBench: A Comprehensive Benchmark for Assessing Reasoning Capabilities of Large Language Models in API Interaction**, arXiv 2024 [[paper]](https://arxiv.org/abs/2408.10735) (*Note: PDF cites Patil et al. 2025, likely a newer version/publication*)
*   **API-Bank: A Benchmark for Tool-Augmented LLMs**, EMNLP 2023 [[paper]](https://arxiv.org/abs/2304.08244)
*   **NexusRaven-V2: Surpassing GPT-4 for Zero-Shot Function Calling**, Blog Post 2023 [[link]](https://nexusflow.ai/blogs/nexusravenv2)
*   **Seal-Tools: Self-Instruct Tool Learning Dataset for Agent Tuning and Detailed Benchmark**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.08747)
*   **ComplexFuncBench: Exploring Multi-step and Constrained Function Calling under Long-Context Scenario**, arXiv 2025 [[paper]](https://arxiv.org/abs/2501.10132)
*   **ToolSandbox: A Stateful, Conversational, Interactive Evaluation Benchmark for LLM Tool Use Capabilities**, arXiv 2024 [[paper]](https://arxiv.org/abs/2408.04682)
*   **RestGPT: Connecting Large Language Models with Real-World RESTful APIs**, arXiv 2023 [[paper]](https://arxiv.org/abs/2306.06624)
*   **APIGen: Automated Pipeline for Generating Verifiable and Diverse Function-Calling Datasets**, NeurIPS 2024 [[paper]](https://arxiv.org/abs/2406.07995)
*   **StableToolBench: Towards Stable Large-scale Benchmarking on Tool Learning of Large Language Models**, arXiv 2024 [[paper]](https://arxiv.org/abs/2403.07714)
*   **NESTFUL: A Benchmark for Evaluating LLMs on Nested Sequences of API Calls**, arXiv 2024 [[paper]](https://arxiv.org/abs/2409.03797)
*   **API-BLEND: A Comprehensive Corpora for Training and Benchmarking API LLMs**, arXiv 2024 [[paper]](https://arxiv.org/abs/2402.15491)

### :thinking: Self-Reflection (§2.3)
*   **LLF-Bench: Benchmark for Interactive Learning from Language Feedback**, arXiv 2023 [[paper]](https://arxiv.org/abs/2312.06853)
*   **LLM-Evolve: Evaluation for LLM's Evolving Capability on Benchmarks**, EMNLP 2024 [[paper]](https://arxiv.org/abs/2402.07083)
*   **Reflection-Bench: Probing AI Intelligence with Reflection**, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.16270)
*   **(Related Concept Papers mentioned):** AGIEval (Zhong et al., 2023), MedMCQA (Pal et al., 2022), ALFWorld (Shridhar et al., 2021), MiniWoB++ (Liu et al., 2018), Reflexion (Shinn et al., 2023), Self-correction papers (Huang et al. 2024, Liu et al. 2025)

### :floppy_disk: Memory (§2.4)
*   **The NarrativeQA Reading Comprehension Challenge**, TACL 2018 [[paper]](https://aclanthology.org/Q18-1023/)
*   **QMSum: A New Benchmark for Query-based Multi-domain Meeting Summarization**, NAACL 2021 [[paper]](https://aclanthology.org/2021.naacl-main.17/)
*   **QUALITY: Question Answering with Long Input Texts, Yes!**, NAACL 2022 Findings [[paper]](https://aclanthology.org/2022.findings-naacl.118/)
*   **RAISE: A Retriever-Augmented In-Context Learning Framework for Enhancing Large Language Models**, arXiv 2024 [[paper]](https://arxiv.org/abs/2401.02777) (*Note: PDF cites Liu et al. 2024a*)
*   **A Human-Inspired Reading Agent with Gist Memory of Very Long Contexts**, arXiv 2024 [[paper]](https://arxiv.org/abs/2402.09727)
*   **MemGPT: Towards LLMs as Operating Systems**, arXiv 2023 [[paper]](https://arxiv.org/abs/2310.08560)
*   **LoCoMo: Evaluating Very Long-Term Conversational Memory of LLM Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2402.17753)
*   **A-Mem: Agentic Memory for LLM Agents**, arXiv 2025 [[paper]](https://arxiv.org/abs/2502.12110)
*   **StreamBench: Towards Benchmarking Continuous Improvement of Language Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.08747)
*   **LTMbenchmark: Beyond Prompts: Dynamic Conversational Benchmarking of Large Language Models**, arXiv 2024 [[paper]](https://arxiv.org/abs/2409.20222)
*   **(Related Concept Papers mentioned):** Reflexion (Shinn et al., 2023), KARMA (Wang et al., 2024b)

## :dart: Application-Specific Agent Evaluation (§3)

### :globe_with_meridians: Web Agents (§3.1)
*   **MiniWob: World of Bits: An Open-Domain Platform for Web-Based Agents**, ICML 2017 [[paper]](https://arxiv.org/abs/1702.00931)
*   **MiniWoB++: Reinforcement Learning on Web Interfaces Using Workflow-Guided Exploration**, ICLR 2019 [[paper]](https://arxiv.org/abs/1802.08802)
*   **WebShop: Towards Scalable Real-World Web Interaction with Grounded Language Agents**, NeurIPS 2022 [[paper]](https://arxiv.org/abs/2207.01206)
*   **Mind2Web: Towards a Generalist Agent for the Web**, NeurIPS 2023 [[paper]](https://arxiv.org/abs/2306.06070)
*   **WebVoyager: Building an End-to-End Web Agent with Large Multimodal Models**, arXiv 2024 [[paper]](https://arxiv.org/abs/2401.13919)
*   **WebLinX: Real-World Website Navigation with Multi-Turn Dialogue**, arXiv 2024 [[paper]](https://arxiv.org/abs/2402.05930)
*   **WebArena: A Realistic Web Environment for Building Autonomous Agents**, ICLR 2024 [[paper]](https://arxiv.org/abs/2307.13854)
*   **VisualWebArena: Evaluating Multimodal Agents on Realistic Visual Web Tasks**, arXiv 2024 [[paper]](https://arxiv.org/abs/2401.13649)
*   **MMInA: Benchmarking Multihop Multimodal Internet Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2404.09992)
*   **AssistantBench: Can Web Agents Solve Realistic and Time-Consuming Tasks?**, arXiv 2024 [[paper]](https://arxiv.org/abs/2407.15711)
*   **WebCanvas: Benchmarking Web Agents in Online Environments**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.12373)
*   **ST-WebAgentBench: A Benchmark for Evaluating Safety and Trustworthiness in Web Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.06703)
*   **WorkArena: How Capable Are Web Agents at Solving Common Knowledge Work Tasks?**, arXiv 2024 [[paper]](https://arxiv.org/abs/2403.07718)
*   **WorkArena++: Towards Compositional Planning and Reasoning-Based Common Knowledge Work Tasks**, NeurIPS 2024 [[paper]](https://openreview.net/forum?id=h7P9uW2y7u)

### :computer: Software Engineering Agents (§3.2)
*   **HumanEval: Evaluating Large Language Models Trained on Code**, arXiv 2021 [[paper]](https://arxiv.org/abs/2107.03374)
*   **SWE-bench: Can Language Models Resolve Real-World GitHub Issues?**, NeurIPS 2023 [[paper]](https://arxiv.org/abs/2310.06770)
*   **SWE-bench Verified**: OpenAI Blog Post 2024 [[link]](https://openai.com/index/introducing-swe-bench-verified/)
*   **SWE-bench Lite**: SWE-bench website [[link]](https://www.swebench.com/lite.html)
*   **SWE-bench LiteS**: (Referenced as Xia et al., 2024)
*   **SWE-bench+**: Enhanced Coding Benchmark for LLMs, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.06992)
*   **SWE-bench Multimodal: Do AI Systems Generalize to Visual Software Domains?**, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.03859)
*   **TDD-Bench Verified: Can LLMs Generate Tests for Issues Before They Get Resolved?**, arXiv 2024 [[paper]](https://arxiv.org/abs/2412.02883)
*   **SWT-Bench: Testing and Validating Real-World Bug-Fixes with Code Agents**, NeurIPS 2024 [[paper]](https://arxiv.org/abs/2404.02653)
*   **IT-Bench: Evaluating AI Agents Across Diverse Real-World IT Automation Tasks**, arXiv 2025 [[paper]](https://arxiv.org/abs/2502.05352)
*   **SWELancer: Can Frontier LLMs Earn $1 Million from Real-World Freelance Software Engineering?**, arXiv 2025 [[paper]](https://arxiv.org/abs/2502.12115)
*   **(Related):** AgentBench (Liu et al., 2023b) [[paper]](https://arxiv.org/abs/2308.03688)

### :microscope: Scientific Agents (§3.3)
*   **ScienceQA: Learn to Explain: Multimodal Reasoning via Thought Chains for Science Question Answering**, NeurIPS 2022 [[paper]](https://arxiv.org/abs/2209.09513)
*   **QASPER: A Dataset of Information-Seeking Questions and Answers Anchored in Research Papers**, NAACL 2021 [[paper]](https://aclanthology.org/2021.naacl-main.80/)
*   **MS² (Multi-Document Summarization of Medical Studies)**, EMNLP 2021 Findings [[paper]](https://aclanthology.org/2021.findings-emnlp.186/)
*   **ScienceWorld: Is Your Agent Smarter Than a 5th Grader?**, EMNLP 2022 [[paper]](https://aclanthology.org/2022.emnlp-main.772/)
*   **SUPER: Evaluating Agents on Setting Up and Executing Tasks from Research Repositories**, arXiv 2024 [[paper]](https://arxiv.org/abs/2409.07440)
*   **Ideation (Can LLMs Generate Novel Research Ideas?)**: ICLR 2025 [[paper]](https://openreview.net/forum?id=cMptYf6vI7)
*   **AAAR-1.0: Assessing AI's Potential to Assist Research**, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.22394)
*   **ScienceAgentBench: Toward Rigorous Assessment of Language Agents for Data-Driven Scientific Discovery**, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.05080)
*   **CORE-Bench: Fostering the Credibility of Published Research through a Computational Reproducibility Agent Benchmark**, arXiv 2024 [[paper]](https://arxiv.org/abs/2409.11363)
*   **SciCode: A Research Coding Benchmark Curated by Scientists**, NeurIPS 2024 Datasets Track [[paper]](https://arxiv.org/abs/2407.13168)
*   **MLGym-Bench: A New Framework and Benchmark for Advancing AI Research Agents**, arXiv 2025 [[paper]](https://arxiv.org/abs/2502.14499)
*   **DiscoveryWorld: A Virtual Environment for Developing and Evaluating Automated Scientific Discovery Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.06769)
*   **LAB-Bench: Measuring Capabilities of Language Models for Biology Research**, arXiv 2024 [[paper]](https://arxiv.org/abs/2407.10362)

### :speech_balloon: Conversational Agents (§3.4)
*   **ABCD: Action-Based Conversations Dataset**, LREC 2022 [[paper]](https://aclanthology.org/2022.lrec-1.564/)
*   **MultiWOZ: A Large-Scale Multi-Domain Wizard-of-Oz Dataset for Task-Oriented Dialogue Modelling**, EMNLP 2018 [[paper]](https://aclanthology.org/D18-1547/)
*   **SMCalFlow: Task-Oriented Dialogue as Dataflow Synthesis**, TACL 2020 [[paper]](https://aclanthology.org/2020.tacl-1.34/)
*   **ALMITA: Automated test generation to evaluate tool-augmented LLMs as conversational AI agents**, GenBench @ EMNLP 2024 [[paper]](https://aclanthology.org/2024.genbench-1.6/)
*   **τ-Bench: A Benchmark for Tool-Agent-User Interaction in Real-World Domains**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.12045)
*   **IntellAgent: A Multi-Agent Framework for Evaluating Conversational AI Systems**, arXiv 2025 [[paper]](https://arxiv.org/abs/2501.11067) (*Note: PDF cites Levi and Kadar, 2025a*)
*   **LTM (Long Term Memory Benchmark)**: Referenced as Castillo-Bolado et al., 2024b

## :earth_africa: Generalist Agents Evaluation (§4)
*   **GAIA: A Benchmark for General AI Assistants**, arXiv 2023 [[paper]](https://arxiv.org/abs/2311.12983)
*   **AgentBench: Evaluating LLMs as Agents**, ICLR 2024 [[paper]](https://arxiv.org/abs/2308.03688)
*   **Galileo's Agent Leaderboard**: Hugging Face Space [[link]](https://huggingface.co/spaces/galileo-ai/agent-leaderboard)
*   **OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments**, NeurIPS 2024 Datasets Track [[paper]](https://arxiv.org/abs/2404.06775)
*   **AppWorld: A Controllable World of Apps and People for Benchmarking Interactive Coding Agents**, ACL 2024 [[paper]](https://aclanthology.org/2024.acl-long.889/)
*   **OmniACT: A Dataset and Benchmark for Enabling Multimodal Generalist Autonomous Agents for Desktop and Web**, ECCV 2024 [[paper]](https://arxiv.org/abs/2407.18160)
*   **TheAgentCompany: Benchmarking LLM Agents on Consequential Real World Tasks**, arXiv 2024 [[paper]](https://arxiv.org/abs/2412.14161)
*   **CRMArena: Understanding the Capacity of LLM Agents to Perform Professional CRM Tasks in Realistic Environments**, arXiv 2024 [[paper]](https://arxiv.org/abs/2411.02305)
*   **HAL: A Holistic Agent Leaderboard for Centralized and Reproducible Agent Evaluation**, arXiv 2025 [[paper]](https://arxiv.org/abs/2501.09208)

## :building_construction: Frameworks for Agent Evaluation (§5)
*   **Databricks Mosaic AI Agent Evaluation**: Blog Post [[link]](https://www.databricks.com/blog/announcing-mosaic-ai-agent-evaluation)
*   **Galileo Agentic Evaluation**: Product Page [[link]](https://www.rungalileo.io/agentic-evaluation)
*   **Vertex AI Gen AI Evaluation**: Google Cloud Docs [[link]](https://cloud.google.com/vertex-ai/docs/generative-ai/evaluate/agent-evaluation)
*   **LangSmith**: LangChain Docs [[link]](https://docs.smith.langchain.com/)
*   **Langfuse**: Langfuse Docs [[link]](https://langfuse.com/docs)
*   **Patronus AI**: Company Website [[link]](https://www.patronus.ai/)
*   **LangChain AgentEvals**: LangChain Docs [[link]](https://python.langchain.com/docs/guides/evaluation/agents/)
*   **Arize AI Evaluation**: (Needs specific link, Arize offers broad eval) [[link]](https://arize.com/evaluation/)
*   **(Related Frameworks/Tools Mentioned):** OpenAI Evals, OpenTelemetry, Botpress, AutoGen Studio.
*   **Gym-like Environments:** BrowserGym [[paper]](https://arxiv.org/abs/2412.05467), MLGym [[paper]](https://arxiv.org/abs/2502.14499), SWE-Gym [[paper]](https://arxiv.org/abs/2412.21139)

## :chart_with_upwards_trend: Discussion (§6)

### Trends & Directions
*(Refer to Section 6 in the paper for detailed discussion)*

*   **Realistic and Challenging Evaluation:** Shift from static/simple to dynamic/complex environments (e.g., MiniWob -> WebArena, basic coding -> SWE-bench). Increasing task difficulty.
*   **Live Benchmarks:** Need for continuously updated benchmarks (e.g., BFCL versions, SWE-bench variants, IntellAgent).
*   **Advancing Granular Evaluation:** Moving beyond end-to-end metrics to finer-grained, step-by-step analysis (e.g., WebCanvas node completion, Galileo action advancement).
*   **Cost and Efficiency Metrics:** Need for standardized metrics beyond accuracy (e.g., token usage, latency, API costs).
*   **Scaling & Automating Evaluation:** Leveraging synthetic data (IntellAgent, Mosaic AI) and Agent-as-a-Judge approaches.
*   **Safety and Compliance:** Growing need for benchmarks focusing on safety, trustworthiness, and policy adherence (e.g., AgentHarm, ST-WebAgentBench).

## :memo: Citation

If you find this survey or repository helpful, please cite the paper:

```bibtex
@misc{yehudai2025survey,
      title={Survey on Evaluation of LLM-based Agents},
      author={Asaf Yehudai and Lilach Eden and Alan Li and Guy Uziel and Yilun Zhao and Roy Bar-Haim and Arman Cohan and Michal Shmueli-Scheuer},
      year={2025},
      eprint={2503.16416},
      archivePrefix={arXiv},
      primaryClass={cs.AI},
      url={https://arxiv.org/abs/2503.16416}
}