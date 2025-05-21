<div align="center">
<h1>Evaluation of LLM-based Agents: A Reading List</h1>
</div>

<div align="center">
  Based on the Survey Paper: <br />
  <b>Survey on Evaluation of LLM-based Agents</b> (arXiv 2025)
</div>

<div align="center">
  <b>Asaf Yehudai¹², Lilach Eden², Alan Li³, Guy Uziel², Yilun Zhao³, Roy Bar-Haim², 
    Arman Cohan³, Michal Shmueli-Scheuer²</b><br />
  <small>¹The Hebrew University of Jerusalem | ²IBM Research | ³Yale University</small>
</div>
<br />

<div align="center">
    <!-- === UPDATE LINKS === -->
    <a href="https://arxiv.org/abs/2503.16416"><img src="https://img.shields.io/badge/arXiv-2503.16416-b31b1b" alt="Paper"></a>
</div>

### About This Repository

This repository serves as a companion to the survey paper **"Survey on Evaluation of LLM-based Agents"**. It organizes evaluation methodologies, benchmarks, and frameworks according to the structure presented in the paper, aiming to provide a comprehensive resource for researchers and practitioners in the field of LLM-based agents.

The selection criteria focus on works discussed within the survey, covering:
- **Fundamental Agent Capabilities:** Planning, Tool Use, Self-Reflection, Memory.
- **Application-Specific Domains:** Web, Software Engineering, Scientific, Conversational Agents.
- **Generalist Agent Evaluation.**
- **Evaluation Frameworks.**

Our goal is to map the rapidly evolving landscape of agent evaluation, highlight key trends, and identify current limitations as discussed in the survey.

[comment]: <> (*&#40;Note: The initial version is based on arXiv:2503.16416v1 dated 20 Mar 2025. It will be updated as the survey evolves or upon publication.&#41;*)


## Table of Contents
- [:gift: Surveys](#gift-surveys)
- [:wrench: Agent Capabilities Evaluation (§2)](#wrench-agent-capabilities-evaluation-2)
  - [:world_map: Planning and Multi-Step Reasoning (§2.1)](#world_map-planning-and-multi-step-reasoning-21)
  - [:telephone_receiver: Function Calling & Tool Use (§2.2)](#telephone_receiver-function-calling--tool-use-22)
  - [:thinking: Self-Reflection (§2.3)](#thinking-self-reflection-23)
  - [:floppy_disk: Memory (§2.4)](#floppy_disk-memory-24)
- [:dart: Application-Specific Agent Evaluation (§3)](#dart-application-specific-agent-evaluation-3)
  - [:globe_with_meridians: Web Agents (§3.1)](#globe_with_meridians-web-agents-31)
  - [:computer: Software Engineering Agents (§3.2)](#computer-software-engineering-agents-32)
  - [:microscope: Scientific Agents (§3.3)](#microscope-scientific-agents-33)
  - [:speech_balloon: Conversational Agents (§3.4)](#speech_balloon-conversational-agents-34)
- [:earth_africa: Generalist Agents Evaluation (§4)](#earth_africa-generalist-agents-evaluation-4)
- [:building_construction: Frameworks for Agent Evaluation (§5)](#building_construction-frameworks-for-agent-evaluation-5)
- [:video_game: Gym-like Environments (§5.1)](#gym-gym-like-environments-51)
- [:chart_with_upwards_trend: Discussion (§6)](#chart_with_upwards_trend-discussion-6)
  - [:arrow_right: Current Trends(§6.1)](#arrow_right-current-trends-61)
  - [:compass: Emergent Directions(§6.2)](#compass-emergent-directions-62)
- [:heavy_plus_sign: Adding a Benchmark / Paper](#heavy_plus_sign-adding-a-benchmark--paper)
- [:link: Other Relevant Repositories](#link-other-relevant-repositories)
- [:memo: Citation](#memo-citation)
### Other Relevant Repositories


## :gift: Surveys
*   **A Survey on the Safety and Security Threats of Computer-Using Agents:
JARVIS or Ultron?**, arXiv 2025 [[paper]](https://arxiv.org/abs/2505.10924)
*   **Survey on Evaluation of LLM-based Agents**, arXiv 2025 [[paper]](https://arxiv.org/abs/2503.16416) *(This work)*
*   **The Rise and Potential of Large Language Model Based Agents: A Survey**, arXiv 2023 [[paper]](https://arxiv.org/abs/2309.07864)
*   **A Survey on Large Language Model based Autonomous Agents**, arXiv 2023 [[paper]](https://arxiv.org/abs/2308.11432)
*   **Understanding the planning of LLM agents: A survey**, arXiv 2024 [[paper]](https://arxiv.org/abs/2402.02716)
*   **A Survey on the Memory Mechanism of Large Language Model based Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2404.13501)

## :wrench: Agent Capabilities Evaluation (§2)

### :world_map: Planning and Multi-Step Reasoning (§2.1)
*   **AQUA-RAT: Program Induction by Rationale Generation: Learning to Solve and Explain Algebraic Word Problems**, ACL 2017 [[paper]](https://aclanthology.org/P17-1015/)
*   **HotpotQA: A Dataset for Diverse, Explainable Multi-hop Question Answering**, EMNLP 2018 [[paper]](https://arxiv.org/abs/1809.09600)
*   **Think you have Solved Question Answering? Try ARC, the AI2 Reasoning Challenge**, arXiv 2018 [[paper]](https://arxiv.org/abs/1803.05457)
*   **MultiRC: Looking Beyond the Surface: A Challenge Set for Reading Comprehension over Multiple Sentences**, NAACL 2018 [[paper]](https://aclanthology.org/N18-1023/)
*   **StrategyQA: Did Aristotle Use a Laptop? A Question Answering Benchmark with Implicit Reasoning Strategies**, TACL 2021 [[paper]](https://aclanthology.org/2021.tacl-1.21/)
*   **Measuring Mathematical Problem Solving With the MATH Dataset**, NeurIPS 2021 [[paper]](https://arxiv.org/abs/2103.03874)
*   **GSM8K: Training Verifiers to Solve Math Word Problems**, arXiv 2021 [[paper]](https://arxiv.org/abs/2110.14168)
*   **FOLIO: Natural Language Reasoning with First-Order Logic**, EMNLP 2022 Findings [[paper]](https://arxiv.org/abs/2209.00840)
*   **Challenging BIG-Bench Tasks and Whether Chain-of-Thought Can Solve Them**, arXiv 2022 [[paper]](https://arxiv.org/abs/2210.09261)
*   **Game of 24: Tree of Thoughts: Deliberate Problem Solving with Large Language Models**, NeurIPS 2023 [[paper]](https://arxiv.org/abs/2305.10601)
*   **MINT: Evaluating LLMs in Multi-turn Interaction with Tools and Language Feedback**, arXiv 2023 [[paper]](https://arxiv.org/abs/2309.10691)
*   **PlanBench: An Extensible Benchmark for Evaluating Large Language Models on Planning and Reasoning about Change**, NeurIPS 2023 [[paper]](https://arxiv.org/abs/2206.10498)
*   **MUSR: Testing the Limits of Chain-of-Thought with Multistep Soft Reasoning**, arXiv 2023 [[paper]](https://arxiv.org/abs/2310.16049)
*   **ToolEmu: Identifying the Risks of LM Agents with an LM-Emulated Sandbox**, arXiv 2023 [[paper]](https://arxiv.org/abs/2309.15817)
*   **AutoPlanBench: Automating the Generation of Prompts for LLM-based Action Choice in PDDL Planning**, arXiv 2023 [[paper]](https://arxiv.org/abs/2311.09830)
*   **FlowBench: Revisiting and Benchmarking Workflow-Guided Planning for LLM-based Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.14884)
*   **P-FOLIO: Evaluating and Improving Logical Reasoning with Abundant Human-Written Reasoning Chains**, EMNLP 2024 Findings [[paper]](https://aclanthology.org/2024.findings-emnlp.966/)
*   **ACPBench: Reasoning about Action, Change, and Planning**, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.05669)
*   **Natural Plan: Benchmarking LLMs on Natural Language Planning**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.04520)
*   **LogicBench: Towards Systematic Evaluation of Logical Reasoning Ability of Large Language Models**, ACL 2024 [[paper]](https://arxiv.org/abs/2404.15522)

### :telephone_receiver: Function Calling & Tool Use (§2.2)
*   **APIBench: Revisiting, Benchmarking and Exploring API Recommendation: How Far Are We?** arXiv 2021 [[paper]](https://arxiv.org/abs/2112.12653)
*   **ToolBench: ToolLLM: Facilitating Large Language Models to Master 16000+ Real-world APIs**, arXiv 2023 [[paper]](https://arxiv.org/abs/2307.16789)
*   **ToolAlpaca: Generalized Tool Learning for Language Models with 3000 Simulated Cases**, arXiv 2023 [[paper]](https://arxiv.org/abs/2306.05301)
*   **API-Bank: A Benchmark for Tool-Augmented LLMs**, EMNLP 2023 [[paper]](https://aclanthology.org/2023.emnlp-main.187/)
*   **NexusRaven-V2: Surpassing GPT-4 for Zero-Shot Function Calling**, Blog Post 2023 [[link]](https://nexusflow.ai/blogs/ravenv2)
*   **RestGPT: Connecting Large Language Models with Real-World RESTful APIs**, arXiv 2023 [[paper]](https://arxiv.org/abs/2306.06624)
*   **BFCL: Berkeley Function Calling Leaderboard**, Blog Post 2024 [[link]](https://gorilla.cs.berkeley.edu/blogs/8_berkeley_function_calling_leaderboard.html)
*   **Seal-Tools: Self-Instruct Tool Learning Dataset for Agent Tuning and Detailed Benchmark**, arXiv 2024 [[paper]](https://arxiv.org/abs/2405.08355)
*   **ToolSandbox: A Stateful, Conversational, Interactive Evaluation Benchmark for LLM Tool Use Capabilities**, arXiv 2024 [[paper]](https://arxiv.org/abs/2408.04682)
*   **APIGen: Automated Pipeline for Generating Verifiable and Diverse Function-Calling Datasets**, NeurIPS 2024 [[paper]](https://arxiv.org/abs/2406.18518)
*   **StableToolBench: Towards Stable Large-scale Benchmarking on Tool Learning of Large Language Models**, arXiv 2024 [[paper]](https://arxiv.org/abs/2403.07714)
*   **NESTFUL: A Benchmark for Evaluating LLMs on Nested Sequences of API Calls**, arXiv 2024 [[paper]](https://arxiv.org/abs/2409.03797)
*   **API-BLEND: A Comprehensive Corpora for Training and Benchmarking API LLMs**, arXiv 2024 [[paper]](https://arxiv.org/abs/2402.15491)
*   **ComplexFuncBench: Exploring Multi-step and Constrained Function Calling under Long-Context Scenario**, arXiv 2025 [[paper]](https://arxiv.org/abs/2501.10132)

### :thinking: Self-Reflection (§2.3)
*   **MiniWoB++: Reinforcement Learning on Web Interfaces Using Workflow-Guided Exploration**, ICLR 2019 [[paper]](https://arxiv.org/abs/1802.08802)
*   **ALFWorld: Aligning Text and Embodied Environments for Interactive Learning**, ICLR 2021 [[paper]](https://arxiv.org/abs/2010.03768)
*   **MedMCQA: A Large-scale Multi-Subject Multi-Choice Dataset for Medical Domain Question Answering**, arXiv 2022 [[paper]](https://arxiv.org/abs/2203.14371)
*   **LLF-Bench: Benchmark for Interactive Learning from Language Feedback**, arXiv 2023 [[paper]](https://arxiv.org/abs/2312.06853)
*   **Reflexion: Language Agents with Verbal Reinforcement Learning**, NeurIPS 2023 [[paper]](https://arxiv.org/abs/2303.11366)
*   **AGIEval: A Human-Centric Benchmark for Evaluating Foundation Models**, arXiv 2023 [[paper]](https://arxiv.org/abs/2304.06364)
*   **Large Language Models Cannot Self-Correct Reasoning Yet**, arXiv 2023 (Huang et al.) [[paper]](https://arxiv.org/abs/2310.01798)
*   **LLM-Evolve: Evaluation for LLM's Evolving Capability on Benchmarks**, EMNLP 2024 [[paper]](https://aclanthology.org/2024.emnlp-main.940/)
*   **Reflection-Bench: Probing AI Intelligence with Reflection**, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.16270)
*   **Self-reflection makes Large Language Models safer, less biased, and ideologically neutral**, arXiv 2024 (Liu et al.) [[paper]](https://arxiv.org/abs/2406.10400)

### :floppy_disk: Memory (§2.4)
*   **ReadAgent: The NarrativeQA Reading Comprehension Challenge**, TACL 2018 [[paper]](https://aclanthology.org/Q18-1023/)
*   **QMSum: A New Benchmark for Query-based Multi-domain Meeting Summarization**, NAACL 2021 [[paper]](https://arxiv.org/abs/2104.05938)
*   **QUALITY: Question Answering with Long Input Texts, Yes!**, NAACL 2022 Findings [[paper]](https://arxiv.org/abs/2112.08608)
*   **MemGPT: Towards LLMs as Operating Systems**, arXiv 2023 [[paper]](https://arxiv.org/abs/2310.08560)
*   **Reflexion: Language Agents with Verbal Reinforcement Learning**, NeurIPS 2023 [[paper]](https://arxiv.org/abs/2303.11366)
*   **RAISE: From LLM to Conversational Agent: A Memory Enhanced Architecture with Fine-Tuning of Large Language Models**, arXiv 2024 [[paper]](https://arxiv.org/abs/2401.02777)
*   **A Human-Inspired Reading Agent with Gist Memory of Very Long Contexts**, arXiv 2024 [[paper]](https://arxiv.org/abs/2402.09727)
*   **LoCoMo: Evaluating Very Long-Term Conversational Memory of LLM Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2402.17753)
*   **StreamBench: Towards Benchmarking Continuous Improvement of Language Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.08747)
*   **LTMbenchmark: Beyond Prompts: Dynamic Conversational Benchmarking of Large Language Models**, arXiv 2024 [[paper]](https://arxiv.org/abs/2409.20222)
*   **KARMA: Augmenting Embodied AI Agents with Long-and-short Term Memory Systems**, arXiv 2024 [[paper]](https://arxiv.org/abs/2409.14908)
*   **A-Mem: Agentic Memory for LLM Agents**, arXiv 2025 [[paper]](https://arxiv.org/abs/2502.12110)

## :dart: Application-Specific Agent Evaluation (§3)

### :globe_with_meridians: Web Agents (§3.1)
*   **MiniWob: World of Bits: An Open-Domain Platform for Web-Based Agents**, ICML 2017 [[paper]](https://proceedings.mlr.press/v70/shi17a.html)
*   **MiniWoB++: Reinforcement Learning on Web Interfaces Using Workflow-Guided Exploration**, ICLR 2019 [[paper]](https://arxiv.org/abs/1802.08802)
*   **WebShop: Towards Scalable Real-World Web Interaction with Grounded Language Agents**, NeurIPS 2022 [[paper]](https://arxiv.org/abs/2207.01206)
*   **Mind2Web: Towards a Generalist Agent for the Web**, NeurIPS 2023 [[paper]](https://arxiv.org/abs/2306.06070)
*   **WebArena: A Realistic Web Environment for Building Autonomous Agents**, ICLR 2024 (arXiv 2023) [[paper]](https://arxiv.org/abs/2307.13854)
*   **WebVoyager: Building an End-to-End Web Agent with Large Multimodal Models**, arXiv 2024 [[paper]](https://arxiv.org/abs/2401.13919)
*   **VisualWebArena: Evaluating Multimodal Agents on Realistic Visual Web Tasks**, arXiv 2024 [[paper]](https://arxiv.org/abs/2401.13649)
*   **WebLinX: Real-World Website Navigation with Multi-Turn Dialogue**, arXiv 2024 [[paper]](https://arxiv.org/abs/2402.05930)
*   **WorkArena: How Capable Are Web Agents at Solving Common Knowledge Work Tasks?**, arXiv 2024 [[paper]](https://arxiv.org/abs/2403.07718)
*   **MMInA: Benchmarking Multihop Multimodal Internet Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2404.09992)
*   **WebCanvas: Benchmarking Web Agents in Online Environments**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.12373)
*   **WorkArena++: Towards Compositional Planning and Reasoning-Based Common Knowledge Work Tasks**, NeurIPS 2024 [[paper]](https://arxiv.org/abs/2407.05291)
*   **AssistantBench: Can Web Agents Solve Realistic and Time-Consuming Tasks?**, arXiv 2024 [[paper]](https://arxiv.org/abs/2407.15711)
*   **ST-WebAgentBench: A Benchmark for Evaluating Safety and Trustworthiness in Web Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.06703)
*   **VideoWebArena: Evaluating Long Context Multimodal Agents with Video Understanding Web Tasks**, arXiv 2025 [[paper]](https://arxiv.org/abs/2410.19100)
*   **BEARCUBS: A benchmark for computer-using web agents**, arXiv 2025 [[paper]](https://arxiv.org/abs/2503.07919)
*   **Online-Mind2Web:An Illusion of Progress? Assessing the Current State of Web Agents**, arXiv 2025 [[paper]](https://arxiv.org/abs/2504.01382)
*   **BrowseComp: A Simple Yet Challenging Benchmark for Browsing Agents**, arXiv 2025 [[paper]](https://arxiv.org/abs/2504.12516)

### :computer: Software Engineering Agents (§3.2)
*   **HumanEval: Evaluating Large Language Models Trained on Code**, arXiv 2021 [[paper]](https://arxiv.org/abs/2107.03374)
*   **SWE-bench: Can Language Models Resolve Real-World GitHub Issues?**, NeurIPS 2023 [[paper]](https://arxiv.org/abs/2310.06770)
*   **AgentBench: Evaluating LLMs as Agents**, ICLR 2024 (arXiv 2023) [[paper]](https://arxiv.org/abs/2308.03688)
*   **SWE-bench Verified**: OpenAI Blog Post 2024 [[link]](https://openai.com/index/introducing-swe-bench-verified/)
*   **SWE-bench Lite**: SWE-bench website (c. 2024) [[link]](https://www.swebench.com/lite.html)
*   **SWT-Bench: Testing and Validating Real-World Bug-Fixes with Code Agents**, NeurIPS 2024 [[paper]](https://arxiv.org/abs/2406.12952)
*   **SWE-bench+**: Enhanced Coding Benchmark for LLMs, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.06992)
*   **SWE-bench Multimodal: Do AI Systems Generalize to Visual Software Domains?**, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.03859)
*   **TDD-Bench Verified: Can LLMs Generate Tests for Issues Before They Get Resolved?**, arXiv 2024 [[paper]](https://arxiv.org/abs/2412.02883)
*   **Windows Agent Arena: Evaluating Multi-Modal OS Agents at Scale**, arXiv 2024 [[paper]](https://arxiv.org/abs/2409.08264)
*   **IT-Bench: Evaluating AI Agents Across Diverse Real-World IT Automation Tasks**, arXiv 2025 [[paper]](https://arxiv.org/abs/2502.05352)
*   **Cybench: A Framework for Evaluating Cybersecurity Capabilities and Risks of Language Models**, ICLR 2025 [[paper]](https://arxiv.org/abs/2408.08926)
*   **SWELancer: Can Frontier LLMs Earn $1 Million from Real-World Freelance Software Engineering?**, arXiv 2025 [[paper]](https://arxiv.org/abs/2502.12115)
*   **CodeARC: Benchmarking Reasoning Capabilities of LLM Agents for Inductive Program Synthesis**, arXiv 2025 [[paper]](https://arxiv.org/abs/2503.23145)

### :microscope: Scientific Agents (§3.3)
*   **QASPER: A Dataset of Information-Seeking Questions and Answers Anchored in Research Papers**, NAACL 2021 [[paper]](https://arxiv.org/abs/2105.03011)
*   **MS²: Multi-Document Summarization of Medical Studies**, EMNLP 2021 Findings [[paper]](https://aclanthology.org/2021.findings-emnlp.186/)
*   **ScienceQA: Learn to Explain: Multimodal Reasoning via Thought Chains for Science Question Answering**, NeurIPS 2022 [[paper]](https://arxiv.org/abs/2209.09513)
*   **ScienceWorld: Is Your Agent Smarter Than a 5th Grader?**, EMNLP 2022 [[paper]](https://arxiv.org/abs/2203.07540)
*   **DiscoveryWorld: A Virtual Environment for Developing and Evaluating Automated Scientific Discovery Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.06769)
*   **LAB-Bench: Measuring Capabilities of Language Models for Biology Research**, arXiv 2024 [[paper]](https://arxiv.org/abs/2407.10362)
*   **SciCode: A Research Coding Benchmark Curated by Scientists**, NeurIPS 2024 Datasets Track [[paper]](https://arxiv.org/abs/2407.13168)
*   **Can LLMs Generate Novel Research Ideas? A Large-Scale Human Study with 100+ NLP Researchers**: ICLR 2025 (arXiv 2024) [[paper]](https://arxiv.org/abs/2409.04109)
*   **SUPER: Evaluating Agents on Setting Up and Executing Tasks from Research Repositories**, arXiv 2024 [[paper]](https://arxiv.org/abs/2409.07440)
*   **CORE-Bench: Fostering the Credibility of Published Research through a Computational Reproducibility Agent Benchmark**, arXiv 2024 [[paper]](https://arxiv.org/abs/2409.11363)
*   **ScienceAgentBench: Toward Rigorous Assessment of Language Agents for Data-Driven Scientific Discovery**, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.05080)
*   **AAAR-1.0: Assessing AI's Potential to Assist Research**, arXiv 2024 [[paper]](https://arxiv.org/abs/2410.22394)
*   **MLGym-Bench: A New Framework and Benchmark for Advancing AI Research Agents**, arXiv 2025 [[paper]](https://arxiv.org/abs/2502.14499)
*   **PaperBench: Evaluating AI's Ability to Replicate AI Research**, arXiv 2025 [[paper]](https://arxiv.org/abs/2504.01848)


### :speech_balloon: Conversational Agents (§3.4)
*   **MultiWOZ: A Large-Scale Multi-Domain Wizard-of-Oz Dataset for Task-Oriented Dialogue Modelling**, EMNLP 2018 [[paper]](https://aclanthology.org/D18-1547/)
*   **SMCalFlow: Task-Oriented Dialogue as Dataflow Synthesis**, TACL 2020 [[paper]](https://arxiv.org/abs/2009.11423)
*   **ABCD: Action-Based Conversations Dataset: A Corpus for Building More In-Depth Task-Oriented Dialogue Systems**, LREC 2022 [[paper]](https://arxiv.org/abs/2104.00783)
*   **τ-Bench: A Benchmark for Tool-Agent-User Interaction in Real-World Domains**, arXiv 2024 [[paper]](https://arxiv.org/abs/2406.12045)
*   **ALMITA: Automated test generation to evaluate tool-augmented LLMs as conversational AI agents**, GenBench @ EMNLP 2024 [[paper]](https://arxiv.org/abs/2409.15934)
*   **LTM-Benchmark: Beyond Prompts: Dynamic Conversational Benchmarking of Large Language Models**:, arXiv 2024 [[paper]](https://arxiv.org/abs/2409.20222)
*   **IntellAgent: A Multi-Agent Framework for Evaluating Conversational AI Systems**, arXiv 2025 [[paper]](https://arxiv.org/abs/2501.11067)

## :earth_africa: Generalist Agents Evaluation (§4)
*   **GAIA: A Benchmark for General AI Assistants**, arXiv 2023 [[paper]](https://arxiv.org/abs/2311.12983)
*   **AgentBench: Evaluating LLMs as Agents**, ICLR 2024 (arXiv 2023) [[paper]](https://arxiv.org/abs/2308.03688)
*   **OmniACT: A Dataset and Benchmark for Enabling Multimodal Generalist Autonomous Agents for Desktop and Web**, ECCV 2024 [[paper]](https://arxiv.org/abs/2402.17553)
*   **OSWorld: Benchmarking Multimodal Agents for Open-Ended Tasks in Real Computer Environments**, NeurIPS 2024 Datasets Track [[paper]](https://arxiv.org/abs/2404.07972)
*   **Galileo's Agent Leaderboard**: HuggingFace Space (c. 2024) [[link]](https://huggingface.co/spaces/galileo-ai/agent-leaderboard)
*   **AppWorld: A Controllable World of Apps and People for Benchmarking Interactive Coding Agents**, ACL 2024 [[paper]](https://arxiv.org/abs/2407.18901)
*   **AndroidWorld: A Dynamic Benchmarking Environment for Autonomous Agents**, arXiv 2024 [[paper]](https://arxiv.org/abs/2405.14573)
*   **CRMArena: Understanding the Capacity of LLM Agents to Perform Professional CRM Tasks in Realistic Environments**, arXiv 2024 [[paper]](https://arxiv.org/abs/2411.02305)
*   **TheAgentCompany: Benchmarking LLM Agents on Consequential Real World Tasks**, arXiv 2024 [[paper]](https://arxiv.org/abs/2412.14161)
*   **AgentBoard: An Analytical Evaluation Board of Multi-turn LLM Agents**, NeurIPS 2024 [[paper]](https://arxiv.org/abs/2401.13178)
*   **HAL: Holistic Agent Leaderboard**, HAL leaderboard 2025 [[paper]](https://hal.cs.princeton.edu/)

## :building_construction: Frameworks for Agent Evaluation (§5)
*   **Databricks Mosaic AI Agent Evaluation**:[[link]](https://docs.databricks.com/aws/en/generative-ai/agent-evaluation)
*   **Galileo Agentic Evaluation**: [[link]](https://www.galileo.ai/blog/introducing-agentic-evaluations)
*   **Vertex AI Gen AI Evaluation**: [[link]](https://cloud.google.com/blog/products/ai-machine-learning/introducing-agent-evaluation-in-vertex-ai-gen-ai-evaluation-service)
*   **LangSmith**: [[link]](https://docs.smith.langchain.com/)
*   **Langfuse**: [[link]](https://langfuse.com/docs)
*   **Patronus AI**: [[link]](https://www.patronus.ai/)
*   **LangChain AgentEvals**: [[link]](https://github.com/langchain-ai/agentevals)
*   **Arize AI Evaluation**: [[link]](https://docs.arize.com/arize/concepts/agent-evaluation)
*   **W&B Weave**: [[link]](https://wandb.ai/site/weave/)
*   **Comet Opik** [[link]](https://github.com/comet-ml/opik)

### :video_game: Gym-like Environments (§5.1)
*   **BrowserGym: The BrowserGym Ecosystem for Web Agent Research** [[paper]](https://arxiv.org/abs/2412.05467)
*   **MLGym: A New Framework and Benchmark for Advancing AI Research Agents** [[paper]](https://arxiv.org/abs/2502.14499)
*   **SWE-Gym: Training Software Engineering Agents and Verifiers with SWE-Gym** [[paper]](https://arxiv.org/abs/2412.21139)
*   **PersonaGym: Evaluating Persona Agents and LLMs** [[paper]](https://arxiv.org/abs/2407.18416)
*   **RepoST: Scalable Repository-Level Coding Environment Construction with Sandbox Testing** [[paper]](https://arxiv.org/abs/2503.07358)

## :chart_with_upwards_trend: Discussion (§6)

### Trends & Directions
*(Refer to Section 6 in the paper for detailed discussion)*

### :arrow_right: Current Trends (§6.1)

#### Realistic and Challenging Evaluation
The field is moving beyond simplified, static environments towards benchmarks reflecting real-world complexity and increased difficulty.

#### Live Benchmarks
Static benchmarks quickly become outdated. There is a trend towards adaptive benchmarks that incorporate live data or continuous updates to maintain relevance.

### :compass: Emergent Directions (§6.2)

#### Advancing Granular Evaluation
Moving beyond coarse, end-to-end success metrics to more detailed, step-by-step analysis to diagnose failures.
*   **WebCanvas**: Benchmarking Web Agents in Online Environments (Measures key node completion) [[paper]](https://arxiv.org/abs/2406.12373)
*   **LangSmith**: LangChain Evaluation Framework (Supports trajectory tracing) [[link]](https://docs.smith.langchain.com/)
*   **Galileo Agentic Evaluation**: (Introduces action advancement metric) [[link]](https://www.galileo.ai/blog/introducing-agentic-evaluations)

#### Cost and Efficiency Metrics
Increasing focus on measuring resource consumption (tokens, time, API calls) alongside performance.
*   **AI Agents That Matter:** [[paper]](https://arxiv.org/abs/2407.01502)

#### Scaling & Automating Evaluation
Developing methods to reduce reliance on manual annotation and enable continuous, large-scale evaluation.
*   **Synthetic Data Generation:**
    *   **IntellAgent**: [[paper]](https://arxiv.org/abs/2501.11067)
    *   **Mosaic AI Agent Evaluation**: [[link]](https://docs.databricks.com/aws/en/generative-ai/agent-evaluation)
*   **Agent-as-a-Judge:**
    *   **Agent-as-a-Judge: Evaluate agents with agents** [[paper]](https://arxiv.org/abs/2410.10934)

#### Safety and Compliance
Growing need for benchmarks that specifically test safety, trustworthiness, robustness against adversarial inputs, and adherence to policies.
*   **AgentHarm: A Benchmark for Measuring Harmfulness of LLM Agents**, ICLR 2025 [[paper]](https://arxiv.org/abs/2410.09024)
*   **ST-WebAgentBench: A Benchmark for Evaluating Safety and Trustworthiness in Web Agents**, ICLR 2025 [[paper]](https://arxiv.org/abs/2410.06703)
*   **Multi-Agent Risks from Advanced AI**, arXiv 2025 [[paper]](https://arxiv.org/abs/2502.14143)
*   **Evaluating Cultural and Social Awareness of LLM Web Agents**, NAACL-findings 2025 [[paper]](https://arxiv.org/abs/2410.23252)
*   **Breaking ReAct Agents: Foot-in-the-Door Attack Will Get You In**, NAACL 2025 [[paper]](https://aclanthology.org/2025.findings-naacl.363)

## :heavy_plus_sign: Adding a Benchmark / Paper

We aim to keep this list comprehensive and up-to-date within the scope of **LLM-based Agent Evaluation**, as covered in our survey. If you know of a relevant benchmark, evaluation framework, or significant paper that fits this focus and is missing from the list, we welcome your suggestions!

**Contribution Guidelines:**

1.  **Relevance:** Please ensure the work is directly related to the *evaluation* methodologies, benchmarks, frameworks, or core capabilities/applications *as they pertain to assessing LLM-based agents*.
2.  **Information:** Provide the full paper title, authors, publication venue/year (or arXiv link), and a direct link to the paper (DOI, arXiv, etc.).
3.  **Justification (Optional but helpful):** Briefly explain why the paper is relevant and where it might fit within the existing structure.

**How to Suggest:**

*   **Preferred Method: Open a GitHub Issue:**
    *   Click on the "Issues" tab of this repository.
    *   Create a "New Issue".
    *   Use a descriptive title (e.g., "Suggestion: Add [Benchmark/Paper Name]").
    *   Include the information requested above in the issue description.
*   **Alternative: Submit a Pull Request:**
    *   If you are comfortable editing the `README.md` file directly, you can fork the repository, add the paper following the existing format, and submit a Pull Request. Please ensure your addition is placed in the appropriate section.

We appreciate your contributions to making this a valuable resource for the community!

## :link: Other Relevant Repositories

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
