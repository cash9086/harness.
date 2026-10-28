# arXiv: agent harness

- **Query:** `all:"agent harness" AND (cat:cs.AI OR cat:cs.LG OR cat:cs.CL OR cat:cs.MA OR cat:cs.CV OR cat:cs.NE OR cat:cs.IR OR cat:stat.ML) AND submittedDate:[202601010000 TO 299912312359]`
- **Dal:** 2026-01-01
- **Generato il:** 2026-10-27 11:50 UTC
- **Risultati:** 453

---

## 1. I-HITL: Inalienable Human-in-the-Loop

**Autori:** Samuel Breckenridge, Dani Vilardell, Wenhao Wang, Fan Zhang, Ari Juels  
**Data:** 2026-10-26  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2610.35835v1

> Human oversight is a pillar of AI safety. It is often exercised by a human in the loop (HITL) who approves critical actions taken by an AI agent. AI agents' increasing ability to bypass guardrails, though, raises the question of how to enforce HITL robustly. We introduce the concept of inalienable human-in-the-loop (I-HITL). An I-HITL protocol ensures that an agent can initiate an action only with explicit human approval, even when the human interacts with a system (e.g., a local agentic harness) compromised by the agent. A strong I-HITL protocol additionally ensures such approval even when an adversarial human attempts to delegate approvals to an agent. To motivate I-HITL, we report on experiments with a popular agentic wallet platform in which raising an agent's spending cap requires HITL approval via emailed one-time passcodes (OTPs). Given access to the user's email and a task blocked by the cap, we find that ten different frontier models will often autonomously raise the cap, harvesting OTPs to bypass a HITL guardrail and surfacing other vulnerabilities. We formally define I-HITL using the concept of communication topologies and prove necessary and sufficient conditions for its realization. We show that an I-HITL protocol requires a trusted entity - a trusted computing device (or equivalent) - and characterize which such devices can and cannot realize an I-HITL protocol. We present a prototype I-HITL system called Countersign that can plug into and strengthen existing HITL systems using off-the-shelf consumer mobile devices.

---

## 2. Profiling a Frontier Agent with EBench: From Direct Control to Harness with Policy

**Autori:** Yifei Yao, Yude Zou, Guanbo Jiao, Xing Gao, Ning Gao, Yukai Wang, Jiantong Chen, Zihou Zhu, Xinyu Li, Ningyu Yan, Shuai Wang, Jianming Ma, Haoyu Guo, Weinan Zhang, Chunhua Shen  
**Data:** 2026-10-26  
**Categorie:** cs.RO, cs.AI  
**Link:** https://arxiv.org/abs/2610.35832v1

> Frontier multimodal large language models (MLLMs) can control robots without robot-specific training, but how their capabilities compare and interact with post-trained vision-language-action (VLA) and world action model (WAM) policies across manipulation demands remains to be thoroughly evaluated. In this report, we evaluate GPT-6-Astra on EBench as the core of an agent that controls a robot through an agent harness under the same visual and proprioceptive observation protocol as post-trained policies. We study two agent configurations: direct control, in which the agent generates waypoint commands directly, and harness with policy, in which it can also invoke a post-trained VLA or WAM policy for action execution. Under direct control, the agent achieves competitive overall performance relative to post-trained policies. It leads on short-horizon tasks and exhibits the least performance variation across generalization dimensions, whereas it underperforms post-trained policies on long-horizon tasks, tabletop manipulation, and high-precision contact-rich tasks. In the harness with policy, invoking a post-trained VLA or WAM combines the complementary strengths of both components, raising overall task success to the level of the strongest compared post-trained policies while substantially reducing token cost. However, performance remains below the per-task upper bound of the standalone components due to suboptimal policy invocation, fixed-instruction execution without subgoals, and grasp disruption when the agent resumes control. Overall, our study characterizes the capability boundary of a frontier MLLM agent and suggests directions for improving future agent harness design. Project page: https://internrobotics.github.io/EBench-Astra-Tech-Report/

---

## 3. Hierarchical Skill Evolution for Coding Agent

**Autori:** Jun Gao, Yun Peng, Changhai Zhou, Yuhan Zhu, Xiangyu Zeng, Shiyang Zhang Yuhua Zhou, Luozheng Qin, Qian Qiao, Xiaoteng Ma, Baian Chen Weiyi Shang, Zhen Ming Jack Jiang, Lizhi Liao, Xiaoxue Ren  
**Data:** 2026-10-26  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2610.35616v1

> Skills provide agents with reusable experience to guide future decisions without modifying the underlying model. However, coding trajectories are often entangled with task- and repository-specific contexts, making it challenging to distill procedural skills that generalize across diverse coding environments. To address this challenge, we present Hierarchical Skill Evolution (HSE), which progressively distills procedural knowledge from coding trajectories through hierarchical evidence aggregation. HSE first extracts task-level evidence from individual trajectories, then aggregates recurring evidence within the same repository to form repository-specific skill candidates, and finally consolidates consistent patterns across repositories into transferable skills across repositories. The evolution is driven by an external writer-evaluator loop that generates and assesses skills while keeping the underlying coding model frozen. The loop externally updates the writer and evaluator policies to improve subsequent skill generation and assessment. This hierarchy progressively filters task-specific details while preserving procedures that generalize across diverse coding environments. Successful trajectories yield reusable guidance for future tasks, while failed trajectories reveal recurring failure modes that guide avoidance and recovery. We evaluate HSE on SWE-bench Verified and DeepSWE, using GLM-5.2 across Pi and Claude Code harnesses and GPT-5.5 and Opus 4.8 with Pi. Across both benchmarks, 10 skills evolved solely from SWE-Gym improve coding performance across all evaluated settings, demonstrating transfer across benchmarks, coding models, and agent harnesses. We further evolve the skill library from target-benchmark trajectories without verifier feedback, relying solely on the learned evaluator for candidate assessment and achieving additional gains through benchmark-tailored skills.

---

## 4. MarkovSim: an LLM Agent Harness with Bounded Context for Long-Horizon Computational Simulation

**Autori:** Yeui-Lung Lei, Wen-Bo Chen, Pan Zhang  
**Data:** 2026-10-26  
**Categorie:** cs.CE, cs.AI  
**Link:** https://arxiv.org/abs/2610.35349v1

> Recent studies have applied large language model (LLM) agent systems to computational simulation workflows. Such workflows are long-horizon, so the information generated can exceed what an LLM can reason over at once, its context window. Context management is therefore essential, yet existing systems have either neglected it or treated it as a supporting mechanism rather than a subject of study. This paper presents MarkovSim, an LLM agent harness for long-horizon computational simulation, whose core is a context management scheme built into the workflow. The workflow record is written to a memory system with a predefined schema, and at workflow-defined boundaries, namely the state transitions of a finite-state machine a compact representation of the solution progress is constructed from it as the agent's context. Instantiated on finite element analysis and evaluated on six benchmark problems, MarkovSim passed 16 of 18 runs and corrected its own faults in both the solver operations and the model physics. The engineer was consulted only where engineering judgement was needed. The context remained bounded throughout every run, regardless of its length.

---

## 5. RepoTrace: Improving Requirement Tracing in Multi-Round Agent Interactions

**Autori:** Huanyu Liu, Yezheng Cheng, Jinliang You, Tianxiao Huang, Linyu Li, Zheng Fang, Peng Cao, Ge Li  
**Data:** 2026-10-26  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2610.35333v1

> Code agents have become increasingly capable of performing software engineering tasks through interaction with software environments. However, agents tend to degrade as the number of interaction rounds increases, making it difficult to maintain existing software during iterative modification. We analyze 2,656 agent trajectories in EvoCode-Bench and identify requirement focus misalignment as a recurring failure pattern, where agents struggle to distinguish the primary modification targets of a requirement from unrelated code. We propose Repotrace a requirement-driven repository understanding harness that combines repository structure with requirement semantics to construct a requirement-code correspondence and injects it into the agent context. This correspondence enables code agents to follow the repository architecture, trace requirements across multi-round interactions, and identify the core code elements corresponding to the current requirement. Experiments show that Repotrace improves the mean per-round reward (MPR) across different models (e.g., +19.99 on GLM-5.2) and agent harnesses (e.g., +10.22 on Claude Code). Across rounds, Repotrace increases the average per-round reward from 0.163 to 0.371 on Terminus-2 with DeepSeek-V4-Pro, while reducing average regression errors by 56.78%. We release the source code and agents' trajectories to support future research.

---

## 6. RSIV-Harness: A Recursive Self-Improvement Harness Framework for Open-Domain Conversational Text-to-Visualization

**Autori:** Jiawei Lu, Chen Zhang, Jinwei Lu, Yuanwei Song, Yuanfeng Song, Raymond Chi-Wing Wong  
**Data:** 2026-10-26  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.35316v1

> Users often request charts without knowing which database or table holds the relevant data. Such requests may be ambiguous, and users may ask follow-up questions to deepen their analysis or iteratively refine existing charts. A useful assistant must therefore discover relevant data sources among heterogeneous databases, ask clarifying questions when needed, and track evolving user intent while preserving constraints established in earlier turns. Yet recent text-to-visualization agents typically rely on static agent harnesses that are predefined and remain unchanged despite recurring failures across tasks. To address this limitation, we introduce RSIV-Harness, which keeps the language model weights fixed and applies Recursive Self-Improvement to revise the surrounding harness from the agent's own failure traces. To balance flexible self-improvement with stability, we introduce a four-layer framework that evaluates proposed harness revisions through anchor and memory checks, refining those that pass and restoring the best validated harness otherwise. We further introduce ODAC-Vis, a benchmark with 640 tasks for Open-Domain, Ambiguous, and Conversational text-to-visualization that jointly evaluates open-domain data discovery, ambiguity resolution, multi-turn visualization refinement, and executable chart generation. Experiments show that a single round of RSIV-Harness improves all six evaluation metrics relative to the seed harness, with particularly large gains in executability (+28.02 points) and chart structure (+34.01 points), demonstrating the ability to learn from task-solving experience and turn recurring failures across tasks into substantial performance improvements.

---

## 7. Co-Design Bench: Multimodal Collaborative Coding Evaluation for Agentic Models

**Autori:** Xilin Wei, Shengyuan Ding, Xinyu Fang, Tiancheng Gu, Yuchi Wang, Zhixun Li, Ziyu Liu, Yuhang Zang, Weixiang Yu, Cheng Lu, Chonggao Sun, Tong Zhou, Dahua Lin, Hang Zhang, Shuai Bai, Dayiheng Liu  
**Data:** 2026-10-26  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.35138v1

> Evaluating human-AI co-design requires testing whether coding agents can translate real users' multimodal requests into working application revisions. We introduce Co-Design Bench, a reference-free benchmark of 273 tasks curated from 37,463 deduplicated queries across 26,314 real user coding sessions. Its two tracks, Multimodal Editing (ME) and Repository Editing (RE), cover localized edits with optional image, audio, video, or document inputs and coordinated repository revisions. Tasks span three capability dimensions: Grounded Understanding, UI Transformation, and Functional Implementation. The tasks pair normalized requests and runnable pre-edit applications with 2,331 hidden expert-authored acceptance criteria. Our judge-then-refute protocol grades criteria using source and browser evidence, challenges positive verdicts with a separate LLM verifier, and audits visual and interaction claims without gold code or target screenshots. Under a shared agentic harness, the strongest of ten model endpoints passes an average of 69.9% of criteria per task but fully satisfies only 26.4% of tasks. All ten endpoints achieve lower criterion completion on repository edits spanning three or four change types than on those spanning one or two. Co-Design Bench provides a testbed for studying the gap between partial requirement satisfaction and complete task success under agentic execution for real-user application revisions.

---

## 8. Learning to Remember: Advances in Memory Mechanisms for Large Language Models

**Autori:** Chenye Han, Hongche Yu, Mengyue Wu, Dell Zhang, Jixiang Luo  
**Data:** 2026-10-26  
**Categorie:** cs.IR  
**Link:** https://arxiv.org/abs/2610.35089v1

> Memory has become a central mechanism for extending large language models (LLMs) beyond fixed context windows, stateless interaction, and static parametric knowledge. This survey organizes the literature around three complementary dimensions: the life cycle of memory, the storage substrate, and the system role that memory plays in LLM-based agents, while using cognitive-science-inspired memory concepts as a lightweight conceptual motivation rather than as a separate technical contribution or implementation family. On this basis, we distinguish three mechanism families: nonparametric memory, where information is stored outside model parameters in text, graph, multimodal, or database-like structures; parametric memory, where information is stored or accessed through activations, key-value caches, learned modules, adapter-based parameterizations, or model weights; and memory for agent evolution, where stored experiences support reinforcement learning, continual learning, procedural reuse, context engineering, and agent harness design. Evaluation is treated as a separate cross-cutting component rather than as a memory mechanism. Unlike surveys that focus primarily on retrieval-augmented generation or long-context modeling, this paper emphasizes the full memory life cycle: construction, maintenance, retrieval, consolidation, forgetting, governance, and evaluation. By aligning conceptual motivations, computational memory mechanisms, benchmarks, and deployment concerns, the survey provides a structured roadmap for designing memory-augmented LLM agents that are persistent, adaptive, auditable, and safe to update over time.

---

## 9. CoSA: The Conflict of Skills Attack in Real-World LLM Agent Ecosystems

**Autori:** Yujia Zheng, Tianhao Li, Shangzhi Xu, Yuekai Huang, Ziyou Jiang, Zhaoyang Li, Yuyao Ge, Junran Peng, Mingyang Li  
**Data:** 2026-10-26  
**Categorie:** cs.CL, cs.AI, cs.CR  
**Link:** https://arxiv.org/abs/2610.35082v1

> Agent Skills allow LLM agents to combine reusable capabilities, but checking each Skill in isolation cannot rule out policy violations when they are composed. We term such failures Conflict of Skills (CoS): artifacts or assessment signals produced for one purpose may be reused downstream without preserving the restrictions or authorization needed for their new use. Using controlled executions of publicly available Skills and matched single-Skill controls, we identify four recurring mechanisms behind CoS. Building on these findings, we introduce the Conflict of Skills Attack (CoSA), which adds locally admitted Skills to an existing pool to supply missing business operations (capability supplementation) or reshape artifact exchange, decision reuse, and target/action bindings (relationship reshaping). CoSA leaves existing Skills and runtime permissions unchanged. To evaluate this threat under autonomous Skill selection, we introduce CoSA-Bench, built from real-world Skills and controlled services, with 288 tasks across recruiting, finance, IT, and business, covering data leakage, unauthorized state modification, and unsafe execution. Across five LLMs and three agent harnesses, additions capped at 5% of each original pool raise the policy-violation rate from 35.02% to 58.45%, an increase of 23.43 percentage points. Trace analysis links compliant-to-violating transitions to cross-Skill dependencies involving the additions. Finally, we develop a lightweight harness-level guard that checks information flow and authorization before consequential actions. On OpenClaw recruiting tasks across five models, the guard reduces violations from 65.28% to 6.67%, while policy-compliant task completion on matched benign controls changes from 66.67% to 65.00%.

---

## 10. PatentAgentBench: Benchmarking LLM Agents with Professional Patent Task Suites

**Autori:** Yijie Hu, Wei Li, Junjie Zhou, Zhiqi Jiang, Yi Jin, Licong Xu, Xinkai Sun, Kai Duan, Lisha Zhang  
**Data:** 2026-10-26  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.35031v1

> Patent practice lies at the intersection of technical, legal, and linguistic work, making it challenging yet crucial to technological innovation. Recently, rapid advances in large language models (LLMs) and agentic systems have demonstrated the potential to complete realistic business workflows and even patent works. This raises a question: can current AI systems perform patent work reliably? Existing benchmarks cover a limited range of patent tasks and simplify evidence acquisition by providing reference materials or candidate documents. In this paper, we introduce PatentAgentBench, a benchmark comprising 510 instances across eight task suites: novelty search, freedom-to-operate (FTO) search, design FTO, invalidity search, claim charting, patent drafting, office-action response, and patent translation. Curated from real patent records and professional materials, the benchmark combines task-specific metrics with expert-reviewed annotations and rubrics. Retrieval tasks such novelty search, FTO, etc., require agents to search and compare patent collections without a supplied candidate pool. The drafting and OAR tasks assess the quality of agents' work given technical disclosure and office action notice. We evaluate seven LLMs across four agent harnesses on PatentAgentBench, finding that current systems still struggle to identify novelty, assess risk, and understand practitioner intent throughout patent workflows.

---

## 11. How Do Coding-Agent Harnesses Self-Evolve? An Empirical Study of Retrospective Adaptation

**Autori:** Christoph Treude, Sebastian Baltes  
**Data:** 2026-10-26  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2610.34938v1

> Coding agents can adapt their harnesses, the software, configuration, and instructions used to run them, based on experience from earlier tasks, but whether these adaptations improve their behavior on later tasks remains unclear. We study \retro, a skill that asks an agent to review a completed session and propose harness changes, and ask what changes it proposes and whether implemented changes reduce repeated work on later tasks. We ran Claude Code on 30 SWE-bench Verified issues, qualitatively coded the 125 proposals from \retro, implemented 24, and evaluated 12 harness changes on later issues from the same repositories in fresh sessions with and without each change. Most proposals referred to an event in the session, but 18 of 43 lint-related proposals recommended a practice regardless of what had happened. Among the seven evaluations in which sessions without the change encountered the targeted problem, two changes eliminated the targeted action, one reduced its occurrence, four showed no reduction, and some changes added work on unrelated issues. Harness self-evolution requires more than generating and implementing changes: it needs ways to establish whether a change helps on later tasks and to revise or remove changes that do not.

---

## 12. AT-AT: Automatic Tool Optimization from Agent Traces

**Autori:** Maya Ravichandran, Pragya Tripathi, Dharamendra Kumar, Adith Swaminathan, Nathan Kallus  
**Data:** 2026-10-26  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2610.34679v1

> Efforts to improve LLM-based agents typically focus on modifying the agent itself, yet success also depends on the environment in which an agent acts. Tools mediate this interaction: a tool's description shapes how an agent calls it, and its implementation determines the results and errors the agent receives afterwards. Many tools, such as APIs and MCP servers, are shared by many agents and maintained by providers who cannot change those agents. We introduce AT-AT (Automatic Tool Optimization from Agent Traces), an agentic tool optimizer that improves a shared toolset offline from historical agent executions while holding the agents fixed. A lightweight coding agent reads agent trajectories and their evaluation results, and selectively edits tool descriptions and, when permitted, implementations. On $τ^2$-bench-verified, AT-AT achieves the highest task completion rates in the Airline and Telecom domains at lower cost than strong prompt- and tool-optimizer baselines, and its Telecom gain is statistically significant under paired permutation tests. Optimizing the tools within a coding agent harness also improves held-out performance on TerminalBench-2 and TBLite. When applied to three production MCP servers at a large enterprise, AT-AT lowered cost or tool error rates on every server and increased held-out task passes on one. By turning accumulated execution traces into updates to shared tool environments, AT-AT provides a path toward continual improvement of agent systems through environment-side learning.

---

## 13. Rethinking Verification in Agent Harnesses

**Autori:** Zhengxin Zhang, Erkang Zhu, Yin Lin, Claire Cardie, Bolin Ding, Jingren Zhou  
**Data:** 2026-10-25  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.34577v1

> Agent harnesses enable large language models to act through tools, observe the results, and iteratively work toward a task goal. Verification checks and revises agents' work to improve output quality. Yet there is limited guidance on how harnesses should organize this effort. We study verification as an axis of test-time scaling by examining when to intervene, who checks the work, and how checking leads to revision. Our framework spans four layers of the agent lifecycle: initial instructions, mid-turn reminders, completion gates, and independent review. We compare 17 designs across seven frontier coding models on Terminal-Bench (TB) and SWE-bench Verified (SWE), and introduce VisualBench for expert evaluation of visual and interactive artifacts. Initial instructions and execution-time reminders yield modest, model-dependent average gains on the coding benchmarks, without substantially increasing average output token use. Completion gates can yield larger gains but may substantially increase cost. Independent review by a critic offers a more favorable accuracy-cost tradeoff, improving average accuracy by 5.9-9.5 percentage points on TB and 3.9-6.6 on SWE at 1.13-1.25 and 1.00-1.04 times baseline cost, respectively. On VisualBench, independent review achieves net preferences of 13.2-23.8 points over the baseline across its four designs, exceeding the evaluated L0-L2 designs. Additional review rounds or independent critics further improve average TB accuracy by up to 3.5 percentage points. Together, these results provide empirical guidance for verification design in agent harnesses and support independent review as a practical axis of test-time scaling.

---

## 14. CTXAgent - Self-Controlled Context Management of LLM Agents

**Autori:** Matthias Busch, Marius Tacke, Roland C. Aydin, Christian Feiler, Christian J. Cyron  
**Data:** 2026-10-25  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.34425v1

> Agent harnesses keep long sessions inside the context window by compacting the history when a token threshold is crossed. We study an alternative in which the model manages its own context: it decides when to compact, what to keep and what to write as the hand-off, given two tools and one paragraph of guidance. Since earlier work found that open-weight models cannot manage their own context without scaffolding, we compare seven frontier models under identical conditions, with and without the context tools, on token cost and benchmark score, and we compare our harness with three widely used harnesses on two of these models. The benchmark is assembled from existing ones: coding exercises, multi-step SciCode problems and SWE-bench Pro and Terminal-Bench 4.0 tasks are interleaved with planted facts, ephemeral observations and standing instructions, all checked deterministically, in sessions of 35-212 turns that resemble a user working through different tasks in one chat. Most of the strongest models manage their context: they compact and curate regularly, the live context of the mixed sessions stays mostly below 100k tokens, and their benchmark scores mostly do not drop significantly. For the models that manage their context well, the cost reduction is substantial but varies between models, because some models compact so often that other costs increase. With Claude Opus 5.5, the self-managed harness matches Claude Code on task success at 34% lower cost than its explicit 200k-window configuration and 49% lower than its default, with no context window to choose. We release the agent, the benchmark and all result rows.

---

## 15. Software Engineering LLMs: Why We Need Them and How Software Engineering Helps Build Them

**Autori:** Amir M. Ebrahimi, Mohammed Mehedi Hasan, Seyed Shayan Daneshvar, Jiahuei Lin, Gopi Krishnan Rajbahadur, Ahmed E. Hassan  
**Data:** 2026-10-24  
**Categorie:** cs.SE, cs.LG  
**Link:** https://arxiv.org/abs/2610.33851v1

> Software engineering (SE) expertise can shape how coding large language models (LLMs) are trained and which engineering capabilities they acquire. We examine this role through an industrial case study of capability-focused training for a 92B-parameter coding LLM serving more than 100,000 developers. We demonstrate how established SE knowledge can guide the selection of engineering capabilities, the construction of verifiable training data, and the evaluation of model improvements. To target repository-level refactoring, we developed RefactorForge, a pipeline that combines refactoring knowledge, established SE tools, and verification techniques to construct training data. Across 306 Python repositories, RefactorForge generated 5,704 executable tasks and retained 4,572 verified teacher trajectories totaling 72.51 million tokens. Incremental supervised fine-tuning on these trajectories, accounting for 0.46% of the preceding coding mixture's tokens, improved RefactorBench performance by 18.00 percentage points and SWE-Bench ProMax performance by 7.06 points. Under OpenCode, these improvements extended to SWE issue resolution, with gains of 4.97 points on SWE-Bench Verified and 1.23 points on SWE-Bench Pro. Improvements also persisted across other coding-agent harnesses, while greenfield repository generation showed mixed results. We report lessons from constructing capability-focused training data and evaluating its effects across engineering workloads. Building on this industrial experience, we propose a research agenda for expanding SE's role in transforming coding LLMs into SE LLMs: incorporating SE knowledge into model training, applying engineering methods to model development and maintenance, and systematically defining the engineering capabilities these models should acquire.

---

## 16. Build or Adopt? Custom-Built vs. General-Purpose LLM Agent Harnesses for Automotive GUI Testing

**Autori:** Arsham Gholamzadeh Khoee, Ruyu Fu, Jiaqi Wei, Ruikun Deng, Robert Feldt, Dhasarathy Parthasarathy, Yinan Yu  
**Data:** 2026-10-24  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2610.33636v1

> As general-purpose LLM agent harnesses mature, organizations must decide whether to continue developing in-house systems or adopt existing alternatives. We study this decision at Volvo Group for GUI testing of Android-based in-vehicle infotainment (IVI) systems. We compare a production, custom-built harness with two general-purpose harnesses, Claude Code and OpenCode, keeping the tools, accessed through the Model Context Protocol (MCP), and the models the same. We evaluate the harnesses with up to four models on Volvo's IVI test cases and on open-ended tasks in public apps (Google Maps, Booking.com), and interview ten practitioners: developers, the product owner, and testers. On Volvo's stepwise IVI tests, general-purpose harnesses match the custom-built harness in success but vary more across runs. Their inference cost per task is 2.6-10.7 times higher, yet the engineering effort they save outweighs this: for a nightly IVI regression suite, total monthly cost, including engineering effort and inference, is 3-66% lower. On open-ended public-app tasks, they succeed more often, mainly because they recover better from incorrect actions. Interviews suggest that external advances can turn an in-house harness into technical debt even without deterioration. Adopting a general-purpose harness shifts maintenance from the agent loop to tools and instructions, but gives teams less control over what the model receives. Regardless of the harness, testers want to inspect the agent's actions and ensure that it follows the prescribed test scenario.

---

## 17. AdaPRA: Process Reward Agents with Adaptive Rubrics for Data Science

**Autori:** Atharva Naik, Vivek Chari, Pol Llado, Daniel Fried, Carolyn Rosé, Benjamin Van Durme, Sam Thomson, Justin Svegliato  
**Data:** 2026-10-23  
**Categorie:** cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2610.33245v1

> Data science agents can automate end-to-end machine learning workflows, yet they remain far from competitive on human leaderboards. Agents make process errors such as insufficient exploration, unsound validation, coding bugs, and poor use of a fixed budget (re-running the same exploratory data analysis and baseline models in every attempt). We propose AdaPRA to address these issues: a persistent coding agent harness that accumulates knowledge across attempts on the same task, with rubric-guided process supervision that identifies and corrects errors. Our process reward agent audits the agent's trajectory and workspace by executing checks, and adapts its rubrics to each task. We find that rubrics seeded from easier tasks generalize to harder tasks, with rubric adaptation further improving performance. With five attempts per task, AdaPRA improves an 80B Qwen model's leaderboard percentile by 24.5 points on DSPredict-Easy and 14.8 points on DSPredict-Hard while reducing process errors. We also show that supervision with rubrics mined from one base model's runs improves another (DeepSeek-V3.2), and that AdaPRA beats DataPRM, a competitive PRM for data science. We also share our code for reproducibility.

---

## 18. HarnessMM: Recursive Self-Improvement for Harness Token Efficiency

**Autori:** Yuhua Jiang, Chang Xu, Feifei Gao, Li Zhao  
**Data:** 2026-10-23  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.32813v1

> Agent harnesses repeatedly invoke reasoning after tool feedback, even when an earlier call has already fixed the next action. We introduce HarnessMM (Harness Minus Minus), a method for improving harness token efficiency through guarded decision reuse and recursive self-improvement (RSI). RSI iteratively refines companion harness configurations from training feedback, with validation selecting the configuration for deployment. A controller at the model-tool boundary reuses resolved decisions to replace later reasoning callbacks while actor weights remain fixed. Executable Decision Graphs store exact actions, literal arguments, causal dependencies, and public guards. Guarded Decision Reuse activates these persistent decisions from observed receipts; Certified Callback Substitution executes them through the native interface and records removal of the registered slow callback. New semantic decisions, unsupported evidence, and selector abstention invoke the original actor again. The representation restricts what feedback may change, while complete-task measurements establish quality and cost. On HumanEval, HarnessMM preserves Codex success at 90.82\% while reducing Tokens/task (k) from 66.72 to 47.02 (29.54\% saving). For DeepSeek Harness, success rises from 71.43\% to 85.71\% while Tokens/task (k) fall from 96.28 to 11.62 (87.93\% saving). A separate MBPP ablation measures 26.91\% lower cost than single-use graphs and 19.52\% lower cost than retained callbacks. These results establish guarded decision reuse as a practical way to reduce repeated reasoning in existing harnesses.

---

## 19. DealsFlow: An Evidence-Gated Agentic Harness for Venture Capital Deal Triage

**Autori:** Ming Ze Tang, David Cutting, Boyd Carson, Vasiliki Carson  
**Data:** 2026-10-23  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.32380v1

> Large language models (LLMs) can read startup pitch decks, but letting them emit investment scores directly invites score inflation, run-to-run variance and rationales that are hard to audit. We describe DealsFlow, a human-in-the-loop agentic harness deployed at a UK early-stage fund. The LLM reads the deck, cites evidence and rates each category; code combines the ratings, caps them and only ever lowers them. Three mechanisms implement this: a stage-aware corroboration ceiling (78, 70 or 60 out of 100) on factual categories without external evidence; a sceptic call that may lower but never raise a score; and a pre-fetch pattern that retrieves and indexes all evidence before a single generation pass. We evaluate on $N=243$ SEIS/EIS investments with recorded outcomes. Because recent investments have unresolved outcomes, we use the 142 that are at least three years old. There, the full pipeline's score has Spearman $ρ=0.45$ (95% CI 0.32 to 0.57) with the total-value multiple and AUC 0.71 for identifying write-offs, against $ρ=0.38$ and AUC 0.68 for an unconstrained LLM. The gain is small and comes mostly from the sceptic call; we did not test whether its lower-only rule matters. Investments that later exceeded $2\times$ had 64% of factual categories corroborated, against 38% for write-offs (omnibus Kruskal-Wallis test over five outcome groups, $p=0.031$), and our retrieval was not date-restricted, so these figures may overstate screening skill. In a study of 20 inbound applications, analyst time per application fell from 44.7 to 18.9 minutes including verification and correction, and 84% of 240 cited claims were fully supported by their sources, but 70% of reports needed at least one correction.

---

## 20. Trial by Trace: Benchmarking AI Agent Harnesses for Reliability and Failure Attribution

**Autori:** Zhiyong Cao, Hengjie Zhu, Yongxin Wang, Xuchen Li, Jintao Li, Shuxia Liu, Dunqiang Liu, Bo Wang, Kairan Zhang, Cong Lin, JiangDi Yu, Siyuan Liu, Sijia Yao, Yi-Liang Wei, Lingxu Ma, Aijia Wang, Anxin Chen, Zixian Wei, Xiang Ruan, Ruizhi Xu, Ruqian Shi, Baihua Xiao, Sicheng Zhou  
**Data:** 2026-10-23  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.32285v1

> LLM agents are increasingly used to solve real-world problems, and their effectiveness depends on both the underlying models and the harnesses that support their operation. However, most existing benchmarks focus on model capabilities and overall agent performance, with limited attention to the evaluation of agent harnesses. To address this gap, we introduce TraceTrial-Bench, which organizes harness reliability into seven components covering context, execution, governance, lifecycle, observability, tools, and verification. We construct 95 expert-level, mechanism-oriented tasks with executable or state-based ground truth to support semantically equivalent comparisons while preserving the native behavior of each harness. We design a Trajectory Tracing (TT) module to capture agent execution traces and introduce a two-layer evaluation framework that separately assesses agent performance and harness reliability. In addition, we design a Multi-source Evidence Acquisition (MEA) module to provide evidence from the agent context, harness, and execution environment for LLM-based evaluation, and develop a Failure Attribution (FA) module that uses explicit mechanism chains to support attribution at the run level. Across 4 harnesses, 9 models, and 95 tasks, our evaluation of 3,420 runs yields macro-averaged harness scores ranging from 59.8% to 72.0%, while 31.1% of runs achieve task success despite failing at least one harness criterion. TraceTrial-Bench provides an auditable and reproducible foundation for comparing agent harnesses, diagnosing their failures, and studying how harness design interacts with model behavior.

---

## 21. The LLENS Platform for On-Premises Large Language Model Agents in a Japanese University Hospital: Development and Evaluation Study

**Autori:** Ken Enda, Jien Saito, Masami Mukai, Feng Han, Emir Turkes, Tatsumi Kusakabe, Reona Umeki, Kazuhiro Sumiyoshi, Mitsuya Numata, Takumi Tanikawa, Akira Endoh, Kenji Hirata, Atsushi Yoshida, Kohsuke Kudo, Shinya Tanaka  
**Data:** 2026-10-23  
**Categorie:** cs.CL, cs.AI  
**Link:** https://arxiv.org/abs/2610.32151v2

> Large language model agents that use tools could take on part of the electronic health record and desk work that occupies physicians' time, but in many hospitals the medical information systems run inside closed networks, so the model and the agent harness must also be inside the network. We designed, implemented, and deployed LLENS, a clinical support AI agent platform that runs inside the closed network of Hokkaido University Hospital on a single host with 8 NVIDIA H200 GPUs, the open-weight model Kimi K2.6 (~1 trillion parameters), and a web application rebuilt from Open WebUI. The harness has 10 components, including page image reading, full-text attachment input, a path-addressed document tree without a vector index, a network-isolated sandbox, artifact return, self-checking of generated output, subagents, and saved procedures. Kimi K2.6 was chosen from 3 open-weight candidates and scored 480/500 on the 2026 Japanese Medical Licensing Examination; it generated 119 tokens/s for a single user and served 16 concurrent requests at 908 tokens/s in total. On 180 questions over hospital documents (3 seeds each), mean accuracy was 10.7% with no documents, 81.3% with fixed retrieval (top 10 chunks of one lexical search), and 97.2% with interactive access, in which the model reads with document tools and the sandbox (15.9 percentage points above fixed retrieval, 95% CI 10.9-21.3); the difference lay in filtering/counting questions (16.7% vs 87.8%). In an automated test of 13 work scenarios (4 runs each), the expected components were triggered in all runs for 12, and 5 scenarios were run with synthetic data on the deployment host. The platform has run on the hospital network since September 14, 2026.

---

## 22. Do AI-for-Science Agents Preserve Model Safety?

**Autori:** Michael Yew Chuan Lee, Manya Sriram, N. Benjamin Erichson  
**Data:** 2026-10-23  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.32045v1

> AI-for-Science agents are increasingly being used for formulating scientific hypotheses, running autonomous experiments, and interpreting evidence. These agents are constructed by integrating a large language model (LLM) into a domain-specific agent harness, which in turn can improve the LLM's scientific capability and enable the model to orchestrate scientific tools. In this work, we ask whether model safety is preserved when an LLM is integrated in an AI-for-Science agent harness. We evaluate five agent harnesses on 50 harmful chemistry requests. Specifically, we study how the safety behavior changes under direct prompting, two simple adversarial prompting strategies, and an adaptive attack. Across four recent GPT variants, our results show that the agent harness can increase harmful compliance even under direct prompting. More critically, we find that adaptive attacks that are largely unsuccessful against the base LLM suddenly become highly successful after the agent harness is introduced. Our results show that the safety behavior of the base LLM is not durable once a harness is introduced. Thus, as AI-for-Science agents become more capable and autonomous, the community needs to evaluate and align the agent using domain-specific safety benchmarks.

---

## 23. Phronix: The Capability-Centric Learning Paradigm for Agents

**Autori:** Hariharan Devarajan, Neeraj Rajesh, Aniruddha Marathe, Nikoli Dryden, Kin Ng, Michela Taufer  
**Data:** 2026-10-22  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.31789v1

> Scientific computing increasingly relies on large language model-based agents for performance engineering tasks such as instrumentation, analysis, and workflow porting. However, agent effectiveness depends heavily on the surrounding harness, which typically relies on manually written skills and curated memory. This limits autonomous learning, forcing agents to repeatedly rediscover solutions rather than retain and reuse knowledge from prior executions. We introduce Phronix, a capability-centric learning paradigm that enables agentic harnesses to acquire, validate, and refine reusable capabilities from their own executions. Phronix operates through a predictor-validator-corrector loop: MCP tools and associated skills propose solutions, tool executions validate them, and observed outcomes refine the stored capabilities. It distills every observed interaction into a capability store and researches a failing task rather than abandoning it. First, such learned capabilities solve a recurring task on the first attempt in 93-95% of cases across every model, significantly reducing solution non-determinism and improving reliability. Second, Phronix turns an agent's own execution into 7.6-30.8 durable capabilities per task without user instruction, and creation falls below two once the needed capability exists. Third, warm-start runs consume only 0.38-0.40 million tokens per task, which is three to four times less than a single baseline attempt, while a cold-start costs no more than the baseline. On the 1000 Genome Pegasus workflow, instrumenting a production application for I/O performance analysis, Phronix passes all 11 correctness checks against six for the baseline harness, and also lifts the task solving rates of two cheaper models from 29% and 27% of SWE-bench tasks solved to 91% and 87%, respectively, matching the performance of the most expensive evaluated model.

---

## 24. VibeGame: Prompt-to-Game Development with AI-Native Engine and Self-Evolving Adversarial Agent Team

**Autori:** Wenbo Hu, Ken Li, Jiazhe Wei, Yukang Cao, Weiyi Hong, Jiayi Dai, Chenjun Bai, Jiajun Liang, Yucheng Liao, Ruichuan An, Zeyu Lou, Haofan Wang, Yueming Lyu, Jingkang Yang, Ziwei Liu, Chenyang Si  
**Data:** 2026-10-22  
**Categorie:** cs.MA  
**Link:** https://arxiv.org/abs/2610.33106v1

> Large language model agents have enabled software development through natural-language interaction, but extending this paradigm to end-to-end game development remains challenging. Building a playable game requires coordinating code, scenes, assets, animations, physics, and configurations, while allowing developers to validate their integrated behavior through interactive testing. We introduce VibeGame, a framework for creating complete 2D game projects from natural-language prompts and optional reference images. Its AI-native game engine represents project state as schema-validated structured text and provides frame-synchronous runtime control, enabling agents to inspect game states, execute actions, and verify behavior at their own pace. Built upon this interface, we design an Adversarial Agent Team of eight specialized agents to separate implementation from review, so that problems are found and fixed through multi-round loops. For each conducted and accepted project, we further introduce a training-free self-evolution mechanism to distill it into reusable skeletons, modules, and collaboration contracts for future development. We evaluate prompt-assets-to-game (PA2G), where agents are given an asset library, and prompt-to-game (P2G), where agents generate their own art. On a GameCraft-Bench subset, VibeGame in P2G consistently outperforms a range of agent harnesses in either P2G or PA2G with the same underlying model, including GPT-6.1-Sol.

---

## 25. HiSTEVE 1.0: Harnessing Human-Interface VLA Agents for Open-World Games

**Autori:** Zecong Tang, Zian Guan, Yuncheng Guo, Zhanqiu Zhang, Yiwen Guo, Bo Dai  
**Data:** 2026-10-22  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2610.31162v1

> Building virtual embodied agents that operate in open-ended games like human players is a long-standing goal requiring both long-horizon autonomy and reliable native-interface control. As a procedurally generated open world, Minecraft provides a natural testbed for studying the integration of these capabilities. Existing agents typically provide either native visuomotor control without long-horizon autonomy or high-level planning executed through environment APIs or predefined skills. To bridge this gap, we propose HiSTEVE, a hierarchical VLA agent with a capability-aware agent harness. At the orchestration level, we equip the harness with structured memory for tracking progress and a VLM planner for selecting subtasks within the VLA's capabilities. To reliably determine subtask completion, we further introduce a policy-coupled task completion state detector that conditions on VLA policy context to signal candidate completion. At the control level, a single VLA executes all subtasks with vision-only perception and native keyboard-and-mouse actions. To mitigate interference between heterogeneous GUI and non-GUI interactions, we introduce regime-specific RMSNorm branches and separate mouse-movement token embeddings. We also train the VLA through world knowledge injection, imitation learning, and reinforcement learning with environment feedback to improve reliability and recovery. HiSTEVE achieves state-of-the-art atomic-task performance, scoring 85.0% on MineStudio Bench and a 37.4% average success rate on OpenHA, while also completing long-horizon tasks such as crafting an iron pickaxe from scratch like human players.

---

## 26. PLE: Physical-Engineering's Last Exam

**Autori:** Rujun Han, Yufan Zhuang, Arijit Ray, Han Yu, Zoey CuiZhu, George Lee, Yifei Ming, Binz Roy, Varun Sakalkar, Vishy Tirumalashetty, Burak Gokturk, Tomas Pfister, Chen-Yu Lee  
**Data:** 2026-10-21  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.30537v1

> Frontier language models now score above 90% on popular knowledge benchmarks and are increasingly deployed as agents that carry out multi-hour professional work. Yet no existing benchmark tests whether they can perform the real-world, economically valuable work of a professional physical engineer, such as modelling physics and legal code requirements across a multi-format project corpus, optimising material and installation costs, and issuing 2D/3D engineering design packages that a licensed reviewer would sign off on. Existing engineering benchmarks focus on textbook question answering, isolated tool calls or self-contained toy design problems. As a result, most of these benchmarks are already saturated by leading agents and solving them is far away from delivering real engineering design. We introduce PLE, a benchmark of 85 long-horizon, agentic tasks in professional physical engineering consisting of electrical, civil, structural and mechanical engineering, where solving a task means completing a realistic, billable engineering deliverable. PLE combines two complementary curation paths. Expert-Authored tasks are created end to end by practising engineers from a professional data provider's expert pool. Co-Authored tasks start from problem statements written by practising engineers; an adversarial Creator-Solver agent pipeline constructs each task's realistic project environment, executable grader and reference deliverables before sending them to expert engineers for validation and difficulty intensification. We evaluate a variety of frontier LLMs under seven publicly available agent harnesses. Even the strongest configuration reaches a mean score of only 50.6%, while spending 27M tokens and 63 minutes per task on average, demonstrating the substantial gap between current agents and autonomous physical engineering design.

---

## 27. SWE-VERIFIER: Selective Verification for Cost-Efficient Coding Agents

**Autori:** Kaijian Zou, Vaibhav Chennareddy, Yunxiang Zhang, Naihao Deng, Longju Bai, Jiaxin Pei, Rada Mihalcea, Lu Wang  
**Data:** 2026-10-21  
**Categorie:** cs.LG, cs.AI  
**Link:** https://arxiv.org/abs/2610.30284v1

> Coding agents spend substantial computation generating actions and processing long interaction histories. Poor action choices can steer agents into low-value states, wasting computation and increasing API costs. Sampling and verifying alternative actions can improve the agent's decisions, but applying this procedure at every step adds substantial overhead. We introduce SWE-Verifier, a lightweight generative model that selectively triggers candidate sampling and verification. It scores the coding agent's proposed action to determine when additional candidate sampling is needed, then ranks the resulting actions before execution. We train SWE-Verifier from Qwen3.5-4B using preference data that groups contrasting actions with their resulting environment observations and rubric-guided teacher scores. Using the mini-swe-agent harness, SWE-Verifier improves resolution from 75.47% to 77.20% on MiniMax-M2.7 at 1.09 times cost and generalizes to DeepSeek-V4-Flash without training on its actions, improving resolution from 72.60% to 74.27% at 1.13 times cost. Across both models, SWE-Verifier verifies fewer than 4% of steps and achieves comparable or higher resolution than the trajectory and all-step baselines at substantially lower cost. These results demonstrate that selective candidate sampling and lightweight verification provide complementary gains in coding-agent performance and inference efficiency. Our model, code, and data are available at https://github.com/zkjzou/SWE-Verifier.

---

## 28. The End of Consensus Research?

**Autori:** Clément Burgelin, Rachid Guerraoui, Zicong Hong, Yinan Hu, Anne-Marie Kermarrec, Rafael Pires, Rasmus Moorits Veski, Martijn de Vos  
**Data:** 2026-10-21  
**Categorie:** cs.DC, cs.AI  
**Link:** https://arxiv.org/abs/2610.30114v1

> Consensus is a fundamental problem in distributed computing and at the core of state machine replication (SMR). Despite decades of active human research, discovering practical low-latency solutions to the problem is still open, as it requires combining protocol knowledge, correctness reasoning, implementation, and experimental evaluation. We report on how AI helped us discover A-greement, a new consensus protocol for geo-replicated state machines that significantly outperforms state-of-the-art solutions. Averaged across six deployments with 5 or 9 replicas, A-greement reduces the mean latency of a geo-distributed key-value store over the fastest baseline by 12.2% and 33.3% on write-heavy and read-heavy workloads, respectively, and matches the fastest baseline on read-only workloads. A-greement combines lease-authorized local reads, direct client learning for leader-ordered writes, and a fast fixed-quorum per-key write path, selected according to network topology and workload. At the heart of our discovery lies AI-greement, an agent harness for the "autonomous" discovery, implementation, experimentation, and verification of candidate protocols. AI-greement integrates (1) a concept-oriented protocol knowledge base, (2) a modular implementation skeleton, and (3) a Lean-based verification framework with reusable safety definitions, reference specifications, and proofs. AI-greement is of independent interest: its Lean formalization uncovers several previously unreported vulnerabilities in existing consensus protocols, and it provides guidelines on how domain-specific harnesses can turn general-purpose coding agents into effective tools for (distributed) computing research. Yet we argue that human consensus experts remain essential before, during, and after the search: agents reshape the researcher's role rather than end consensus research.

---

## 29. Quant-Arena: Benchmarking LLM Agents for Quantitative Trading Research

**Autori:** Houde Qian, Zheng Jiang, Wenyi Li, Chenxi Xu, Xinjie Lin, Yuzhao Peng, Ruoyu Han, Youjie Zheng, Kaisen Yang, Qinhuai Na, You Fu, Calvin Xiao  
**Data:** 2026-10-21  
**Categorie:** cs.CL, cs.AI, cs.CE  
**Link:** https://arxiv.org/abs/2610.30113v1

> Quantitative research is an iterative loop: a researcher proposes a market hypothesis, implements it as an executable signal, tests it on historical data, and decides what to keep. Existing benchmarks score formulas, code, or individual trading decisions, leaving open whether large language models (LLMs) can complete this loop and produce strategies that work beyond the research period. We introduce Quant-Arena, a benchmark and public leaderboard for end-to-end quantitative research on real A-share market data. A model constructs features and stock-scoring code, receives feedback only on 2022--2023, and freezes one strategy for assessment on the sealed year 2024. A cash-account evaluator applies trading constraints and costs, including market impact estimated from a simulated order book. Scores are dominated by realized excess return and complemented by signal quality and the diversity of features used by the strategy. We evaluate nine frontier models, among which GPT-6 Astra scores highest; yet no model beats the equal-weight market in 2024. Quant-Arena is open to submissions from any model or agent harness.

---

## 30. HGM-Dual: Lineage-Aware Guided Agent Harness Optimization for Long-Horizon Planning

**Autori:** Sudipta Paul, Pengrui Quan, Aounon Kumar, Nicholas Tzou, Vivek Kulkarni, Srinivas Chappidi  
**Data:** 2026-10-21  
**Categorie:** cs.AI, cs.LG, cs.NE  
**Link:** https://arxiv.org/abs/2610.30042v1

> Harness optimization, which improves an agent's prompts, tools, and workflows, is an increasingly effective way to enhance agents built on frozen or closed-source LLMs. Leading approaches such as the Darwin--Godel Machine and the Huxley--Godel Machine (HGM) rely on recursive self-improvement and were developed mainly for coding, where the competence needed to improve the agent coincides with the competence being improved. Planning tasks, in which an agent must produce a sequence of tool calls that jointly satisfies interacting constraints, break this alignment. There, open-ended self-modification repeatedly explores ineffective changes and consumes substantial evaluation budgets. We introduce HGM-Dual, a diagnostic-guided framework for budget-efficient harness evolution for planning agents. First, HGM-Dual represents agent evolution as lineage-aware context. This context records what each ancestor changed, which behaviors improved or regressed, and which modifications were ineffective, giving the editor explicit edit-outcome attribution instead of an unstructured archive of past agents. Second, HGM-Dual introduces error-conditioned dual-path child generation. For each selected parent, it generates a general child that preserves open-ended exploration and specialized children that target the harness components most likely responsible for the parent's highest-ranked constraint violations. HGM-Dual outperforms the strongest baseline by up to 14.45% relative improvement in case accuracy while matching HGM variants' final performance with 2x-4x fewer evaluation budget.

---

## 31. PAUSE: Search-Free Steering of Coding Agents Before Their First Source-Code Edit

**Autori:** Viral Patel, Boyin Tan, Jason Xue, Youcheng Sun  
**Data:** 2026-10-21  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2610.29870v1

> Coding agents can invest substantial effort in repository exploration and testing yet still produce unsuccessful patches. Existing online steering methods review trajectories periodically or invoke an advisor when a monitor detects behavioral problems; frequent reviews are costly, and the absence of anomalous behavior does not mean that an agent is on the right track. We propose PAUSE, a framework for steering coding agents with a single planning intervention. Agents reach their first source-code edit at a median of 60% of trajectory progress, after exploration, bug reproduction, and testing. PAUSE intercepts this edit request before it executes, which requires no learned monitor, no search over checkpoints, and no extra model call (search-free). A separate Planner reads the task and the pre-edit transcript and writes one repair plan; the same agent, the Executor, resumes with this plan, keeping its context and workspace. PAUSE applies online, during a live run, and offline, from a recorded trajectory prefix. We evaluate PAUSE on SWE-bench Verified and SWE-bench Multilingual with two Executors and three agent harnesses. With Qwen3-coder as Executor and GPT-5.6 Sol as Planner, online steering improves resolution by 16.8% on Verified in OpenHands and by 14.7% on Multilingual in SWE-agent. In SWE-agent, PAUSE outperforms LivePlan, a rule-triggered advisor, by 3.2% on Verified and 3.7% on Multilingual at similar Planner cost, and is comparable to SICA's periodic overseer at about 11-15% of its Planner cost. Offline, PAUSE recovers 35.4% of eligible failed Verified tasks, and resuming from the recorded prefix uses 33-41% fewer Executor tokens than restarting.

---

## 32. Harness Scaling for Generalizable Agentic Reinforcement Learning

**Autori:** Fei Bai, Huatong Song, Chuan Hao, Ran Tao, Jian Yang, Bryan Dai, Wayne Xin Zhao, Ji-Rong Wen  
**Data:** 2026-10-21  
**Categorie:** cs.LG, cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2610.29458v2

> Agent harnesses have become a central component of modern agentic systems, shaping how models use tools, manage context, and coordinate long-horizon interaction. Realizing the benefits of these harnesses depends on how effectively the underlying model can make use of them, motivating reinforcement learning directly through the harness. While recent efforts have explored harness diversification to reduce specialization to particular execution settings, how to systematically construct and organize harness diversity for cross-harness generalization remains insufficiently understood. This work studies Harness Scaling as a distinct scaling dimension for agentic RL, focusing on structured variation in how policies execute and interact with the same underlying task and environment. Concretely, we construct a factorized harness space, select a compact training subset with balanced factorial coverage, and organize cross-harness training through locality-aware task assignment. Across multiple benchmarks, model scales, and RL algorithms, Harness Scaling consistently improves generalization to unseen harness combinations. Moreover, policies trained through structured white-box harness variation transfer effectively to unseen external black-box harnesses, outperforming policies trained through a single complex black-box harness. These results establish harness diversity as a meaningful scaling dimension for agentic RL and highlight the importance of how this diversity is organized for cross-harness generalization.

---

## 33. Forging More Tasks into Better Harnesses: Agentic Harness Evolution via Successive Scale Racing

**Autori:** Jingzhe Liu, Jiliang Tang, Tong Zhao, Neil Shah, Clark Mingxuan Ju  
**Data:** 2026-10-20  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.28815v1

> Agentic harness evolution optimizes an agent's instructions, tools, and control flow by using its task execution experiences as evolving evidence. While more evolution tasks should intuitively improve performance, our preliminary study reveals a paradoxical failure mode: the performance of existing methods degrades as the task pool expands. Our further analysis demonstrates that this degradation stems from suboptimal evidence selection during optimization, as different evidence combinations lead to substantially different evolution outcomes. To address this issue, we propose Successive Scale Racing (SSR), a framework that adaptively searches for optimal evidence combinations in each evolution round. SSR constructs diverse evidence combinations based on the corresponding task quality and coverage, and efficiently races the resulting candidate harnesses under a small compute budget. Empirically, across three distinct benchmarks, SSR achieves state-of-the-art results in all six configurations. Notably, as the task pool grows from 40 to 200, SSR steadily improves the pass rate from 64.3% to 68.3%, while the baselines' performances all drop. Furthermore, its racing mechanism identifies near-optimal candidates while reducing validation executions by 60%.

---

## 34. An Explicit Feedback Contract for Iterative ML-Agent Harnesses

**Autori:** Kehui Yao, Chuanbo Hu, Jiao Chen, Ramin Giahi, Reza Yousefi Maragheh, Lalitesh Morishetti, Ziwei Hong, Yiyun Su, Jianpeng Xu, Evren Korpeoglu, Kannan Achan  
**Data:** 2026-10-20  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2610.28798v1

> Iterative ML agents develop models by editing code, running experiments, reading a validation score, and choosing what to try next. In current harnesses this loop is served by an exact validation score returned after every attempt, which leaves the validation split open to adaptive selection. In this work, we introduce an explicit feedback contract for ML-agent harnesses, which specifies what an agent may observe, when iteration should stop, and when the test split may be touched. The contract releases a validation score only when a submission clears a noise threshold computed from the paired standard error, so no margin has to be tuned. We ran experiments on click-through-rate prediction, learning to rank, and a control task with no signal to find. The control is the sharpest case, because the true gain there is zero by construction: an agent reading exact scores ended by reporting a gain of 0.0157, while under the contract it reported 0.0033. On both real tasks the contract narrows the validation-test gap, and test performance is slightly higher rather than lower. The largest difference is in when the agents stop. Exact feedback used its entire budget of thirty submissions on two of the three tasks, including the one where nothing can be learned, while the contract halted after four to twelve. A run that exhausts its budget is usually read as diligence. It is better read as a symptom: when the feedback channel is unbounded, noise keeps supplying improvements to chase.

---

## 35. Object-Oriented Harness: Evolving Agent Harnesses through Object-Oriented Design

**Autori:** Gaotang Li, Bhavana Dalvi Mishra, Yifei Ming, Yanfei Chen, Zhongying CuiZhu, Lesly Miculicich, Long T. Le, Rui Meng, Chun-Liang Li, Hanghang Tong, Chen-Yu Lee, Tomas Pfister  
**Data:** 2026-10-20  
**Categorie:** cs.CL, cs.SE  
**Link:** https://arxiv.org/abs/2610.28380v1

> Agent harnesses are executable code that specifies the prompts, tools, and control flow around a language model. A single global harness can struggle with heterogeneous tasks that require different execution strategies. In this work, we introduce Object-Oriented Harness (OO-Harness), a harness optimization framework that evolves a hierarchy of executable harness classes using object-oriented design. During training, an evolution agent uses execution records to create a family of specialized harnesses, each implemented as a subclass of the base or an existing specialized harness via inheritance. At test time, a harness router uses routing lessons accumulated during training to select a specific harness for each task. Across three long-horizon benchmarks spanning business workflows, workspace tasks, and tool use, OO-Harness achieves the best performance among the compared methods, with an absolute improvement of up to 15% over the base. Extensive ablation studies examine the contributions of its core components.

---

## 36. S-Agent 2.0: Spatial Reasoning with a General Coding Agent

**Autori:** Rui Gong, Ruoyu Wang, Yalun Dai, Hao Li, Sidi Yang, Qihao Zhao, Hongyu Li, Zeyang Guan, Fangzhou Hong, Zhaoxi Chen, Kim-Hui Yap, Ziwei Liu  
**Data:** 2026-10-20  
**Categorie:** cs.AI, cs.CV  
**Link:** https://arxiv.org/abs/2610.28354v1

> Spatial reasoning asks a model to work out where objects are in 3D space, how they relate to one another, and how they move. Agentic VLMs have recently brought large improvements on such tasks by letting the model actively gather evidence with 3D perception tools instead of answering in a single pass. Even so, on many questions the tools return the right evidence and the model still does not arrive at the correct answer: the gap between model and tools, where raw readings become usable conclusions, is left unfilled. We present S-Agent 2.0, a spatial reasoning agent that equips an off-the-shelf general coding agent with a command-line perception toolkit, and we design the interface around one principle: help the VLM close the evidence loop: acquire scene evidence, remember it in a persistent scene memory, and interpret each reading in plain spatial language. This design keeps the full flexibility of a coding agent, and every reading it acts on stays grounded in the tools' geometry. On MMSI-Bench and ReVSI, the toolkit improves a strong open-source model, Qwen3.8-27B, by +13.9 and +20.5 points over the same agent without tools, and a strong closed-source model, Gemini-3.8-Flash, by +11.2 and +9.6 points. With the open backbone S-Agent 2.0 reaches 66.5 on MMSI-Bench and 82.3 on ReVSI, ahead of the specialized system SpatialClaw on the same backbone (62.6 and 74.5), and with Gemini-3.8-Flash it reaches 74.1 and 90.5 against its 67.0 and 79.7. Both tool gains shrink as the backbone grows more capable, but SpatialClaw's shrinks far more on ReVSI, from +13.2 to +2.7, while ours stays at +9.6. S-Agent 2.0 also works across different general coding agent harnesses, such as Codex and Claude Code.

---

## 37. ChartEvo: Self-Evolving Agent Harnesses for Long-Tail Chart Reasoning

**Autori:** Qi Wang, Peijie Wang, Jun Cao, Haoyang Tong, Xiao-Hui Li, Fei Yin, Cheng-Lin Liu  
**Data:** 2026-10-20  
**Categorie:** cs.AI, cs.CV  
**Link:** https://arxiv.org/abs/2610.28282v1

> Multimodal large language models (MLLMs) have substantially advanced chart understanding and reasoning, yet their performance remains highly uneven across chart types. While modern MLLMs perform well on common charts, their accuracy drops sharply on long-tail charts with diverse visual structures and reasoning requirements. Tool-augmented agents can improve complex chart reasoning by introducing specialized visual capabilities, but manually engineering strategies and tools for the heterogeneous and evolving long tail is difficult to scale. We introduce \textbf{ChartEvo}, a recursive self-improvement framework that enables chart agents to adapt to underperforming chart types through experience-driven harness-level self-improvement. ChartEvo jointly evolves reusable chart-specific Skills and executable Tools, while learning reusable local tool-call chains to compose evolved capabilities and control the inference overhead of tool-augmented reasoning. On long-tail charts from ChartBench and ChartX, ChartEvo improves accuracy over its base MLLM, Qwen3.7-Plus, by \textbf{45.6\%} and \textbf{32.5\%}, respectively, demonstrating the effectiveness of recursive self-improvement for long-tail chart adaptation.

---

## 38. MaD-RSI: Model-as-Data for Recursive Self-Improvement of Agent Harnesses

**Autori:** Yu Cui, Hong He, Ruiqing Yue, Sicheng Pan, Zhuoyu Sun, Yifei Liu, Ting Li, Wenzhuo Zhu, Baohan Huang, Haibin Zhang, Cong Zuo  
**Data:** 2026-10-20  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.28201v1

> Recursive self-improvement (RSI) of agent harnesses has emerged as an effective approach to enhancing the capabilities of large language model (LLM) agents. By searching the harness space for a specific LLM on a given dataset, RSI can discover a harness tailored to the capabilities and behavioral characteristics of that model. However, such optimization often creates a strong coupling between the learned harness and its target LLM, limiting generalization across models and requiring substantial computational resources to adapt to new LLMs. Moreover, existing RSI methods typically optimize a harness using feedback from a single model and evaluate its generalization to other models only after training. This paradigm treats model differences primarily as a criterion for evaluating generalization rather than as valuable evidence for optimization. In this paper, we introduce a new perspective that treats models as data and places the harness at the center of optimization. Building on this perspective, we propose \textsc{MaD-RSI}, a framework that directly optimizes a shared harness across multiple heterogeneous LLMs by incorporating their diverse failure trajectories into the training process. Rather than assessing model differences only after optimization, \textsc{MaD-RSI} leverages these differences as training evidence to guide the self-improvement of a shared harness. Furthermore, we introduce a new evaluation framework with two complementary metrics designed to assess the effectiveness of harness optimization across models. Experiments across multiple datasets and LLMs demonstrate that \textsc{MaD-RSI} improves generalization over existing approaches while reducing training costs.

---

## 39. ClawMMU: Protection-Coherent Virtual Memory for Stateful LLM Agents

**Autori:** Jinhao Hu, Bardia Mohammadi, Mofasshara Binte Rafique, Lars Henning Klein, Akhil Arora, Ashvin Goel, Laurent Bindschaedler  
**Data:** 2026-10-20  
**Categorie:** cs.CR, cs.AI, cs.OS  
**Link:** https://arxiv.org/abs/2610.28093v2

> AI agents keep long-term memory, much of which comes from web pages and tool results. Agent harnesses, the software that runs the model, do not record who may act on this memory, so an instruction hidden in a fetched page can be treated as the user's own instruction. We propose ClawMMU, a protection layer that labels every piece of memory with its owner, scope, origins, and authority. ClawMMU checks these labels whenever content enters the model's context, is written to storage, returns from storage, or drives a tool call. Its central rule is that information may rise in authority, but authority never lifts itself. Because the checks depend on where content came from, not on what it says, memory attacks become classical protection faults that the harness stops even when the model is fooled.

---

## 40. Elicitation or Expansion? Demystifying Gains from Agent Harness Optimization

**Autori:** Younghyun Kim, Wooseok Seo, Minseo Kim, Seunghyuk Oh, Minjae Lee, Donghoon Kim, Hyung Il Koo, Jaehyung Kim, Wonjun Kang  
**Data:** 2026-10-20  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2610.27889v1

> Recent studies in harness optimization have shown substantial performance gains in language model agents without updating model weights. A well-designed harness more effectively leverages the underlying model's capabilities by shaping context, tool use, and execution workflows. However, naïve success rates alone do not fully characterize whether optimized harness yields more reliable success on tasks already within reach (elicitation) or a broader range of solvable tasks (expansion). This distinction is crucial for recursive self-improvement and evolutionary search, as expansion may provide a broader range of successful experiences to push the capability boundaries. Despite the growing significance, this distinction remains underexplored in harness optimization. We conduct a systematic analysis to study the effect of gains from harness optimization. Building on pass@k analyses in the reinforcement learning (RL) literature that compare models before and after RL training, we compare optimized harnesses with their pre-optimization counterparts. Specifically, we assess changes in reachable task coverage, compare harness optimization with model scaling and increased inference-time compute, and examine how gains vary with task difficulty. Across static prediction and dynamic tasks, we find that pass@1 advantages of harness over stronger interventions can reverse at larger attempt budgets and aggregate gains conceal shortfalls on hard tasks, underscoring the need for a fine-grained diagnosis.

---

## 41. Act on Your Behalf, Beyond Your Authorization: Benchmarking LLM Agent Authorization Alignment

**Autori:** Zhiping Zhang, Franklin Mingzhe Li, Zihao Huang, Tianshi Li  
**Data:** 2026-10-20  
**Categorie:** cs.AI, cs.CR, cs.HC  
**Link:** https://arxiv.org/abs/2610.27548v2

> When an LLM agent acts on behalf of a user, it is expected to act within the authorization scope the user grants. Existing agent evaluations largely measure task completion or harmful consequences and can therefore overlook actions that violate this delegation without producing conventional safety or privacy harms. We introduce AuthorizationBench, a benchmark of authorization alignment grounded in documented real-world cases. A scalable construction pipeline produces 286 executable tasks spanning situational triggers, the presence or absence of direct harmful consequences, and ten application domains. We execute every task with four models at two reasoning-effort settings across three agent harnesses in an authorization-aware sandbox that keeps authorized and out-of-authorization paths executable and observable, yielding 6,864 trajectories. Agents act out of authorization in 19.2% of trajectories, with rates ranging from 10.5% to 26.6% across the 24 configurations. Task completion does not imply authorization. Increasing reasoning effort leaves the aggregate rate nearly unchanged, with effects varying across models. On controlled pairs, agents act out of authorization at similar rates with (17.9%) and without (20.8%) direct harmful consequences, and more often under benign pressures than malicious injections (23.5% versus 17.6%, p=0.002). Our results show that task capability, additional reasoning, and consequence-oriented safety evaluation do not by themselves ensure authorization alignment. Moreover, agents that consult the principal before completing a task exhibit lower rates of out-of-authorization behavior (14.0% versus 21.6%, p<0.001), pointing to a tension between agent autonomy and preserving users' decision authority that calls for further human-centered study. Dataset and code are available at https://github.com/PEACH-Research-Lab/AuthorizationBench .

---

## 42. Harness Self-Evolution for Long-Horizon Terminal Agents

**Autori:** Ruhan Wang, Yucheng Shi, Zongxia Li, Junyao Yang, Zhongzhi Li, Yue Yu, Haitao Mi, Dongruo Zhou, Leoweiliang  
**Data:** 2026-10-20  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2610.27435v1

> Long-horizon terminal agents may solve a task in one run yet fail across repeated runs. Stochastic errors can propagate through actions and context, creating a gap between capability and reliable execution. We present RiseHarness, a framework for iteratively improving agent harnesses with model weights fixed. It focuses on flipping tasks with both successful and failed runs under the same configuration, using successful runs as references for failure analysis. RiseHarness combines agent trajectories with internal harness traces from a runtime monitor to examine how model actions interact with command execution, feedback, context management, and completion decisions. A Harness Handbook links this evidence to harness behaviors and source code, helping identify recurring problems in mechanisms shared across tasks. RiseHarness then searches other harness frameworks for relevant implementations and adapts them as design references to the current model and execution protocol. Candidate changes undergo behavioral checks and repeated task evaluation; versions with measured gains seed the next iteration. This loop integrates suitable mechanisms from different frameworks into a single harness and uses new execution evidence to guide further changes. We evaluate task success and reliability across models, ablate harness execution evidence and external research, and test transfer to unseen benchmarks with the same model. RiseHarness treats a specific model as the unit of harness adaptation, studying how changes to shared interaction mechanisms can make existing capabilities more reliable across tasks.

---

## 43. Refuses When Asked, Complies When Acting: A Runtime Safety Check for Robot Control Loops

**Autori:** Arnav Grover  
**Data:** 2026-10-19  
**Categorie:** cs.RO, cs.AI  
**Link:** https://arxiv.org/abs/2610.27350v1

> Frontier models can control robots through agent harnesses that loop on one question: what motion comes next toward the user's goal? We show that this default loop carries out harmful instructions. With GPT-6 Astra controlling a low-cost SO-101 arm through the Inspect Robots harness on three household tasks whose hazard is common knowledge, such as "put the knife in the toy basket", the policy refused 0% of 15 trials, attempted the harm every time, and completed it in 27%. Its one exit, give_up, is meant for goals that cannot be achieved, and it never cited the hazard. We add an optional runtime safety check to the loop: before the first motion, the model is asked whether it would carry out the instruction, given the same camera frames. The check would have stopped all 15 hazardous instructions, including the 4 that completed the harm, and flagged none of the 15 harmless controls. Code and data: https://github.com/Arnav-Gr0ver/Refuses-When-Asked-Complies-When-Acting.

---

## 44. Understanding the Benefits of Scaffolds through Computational Separations

**Autori:** Jingchu Gai, Adam Block, Andrej Risteski  
**Data:** 2026-10-19  
**Categorie:** cs.LG, cs.AI  
**Link:** https://arxiv.org/abs/2610.27157v1

> Inference-time harnesses, i.e., external procedures that call a model many times and keep state across calls, can substantially improve model capabilities. In this paper, we investigate the benefits of using such harnesses and the extent to which these benefits can be internalized through training. More precisely, we conceptualize a harness $\mathcal{A}$ as an arbitrary wrapper around a base model $M$ and attempt to distill a student model from the harness's traces. Empirically we find that, even with simple scaffolds and small models, the inference-time harness significantly outperforms a distilled student. We then prove that such a gap is due to a fundamental representational limitation: inference-time harnesses can compute a closure of their per-call primitive that is $\NL$-complete even when the primitive is a trivial $\AC^0$ lookup, and that no fixed-depth forward pass can represent under the widely believed conjecture that $\NL\not\subseteq\TC^0$. Our theory suggests that expanding the representational capacity of the student relative to the task at hand, e.g., by enlarging the model, making the task easier, or lengthening its chain-of-thought, is necessary to close the gap, which we verify empirically. Finally, we scale to an agentic harness on competition math, where the same gap reappears. Overall, our results show that a harness confers on the base model a profound gain in representational power, one that training a same-class student on its traces cannot transfer back into the weights.

---

## 45. A general-purpose System One decision model for clinical records

**Autori:** Andrew Zhang, Trinh T. L. Vuong, Sophia J. Wagner, Dongmin Bang, Tong Ding, Yuchang Su, Mary Cipperman, Christina S. Chen, Judith Lefkes, Ramin Kahidi, Ming Y. Lu, Caiwei Tian, Tianhao Luo, Jingnan Ma, Rowland Pettit, Long Phi Le, Faisal Mahmood  
**Data:** 2026-10-19  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.27099v1

> Clinical care, health-system operations and biomedical discovery depend on extracting reliable answers from patient records, yet applying diverse clinical questions across entire populations remains computationally expensive. Here we present Clinical System One (CS1), a 4-billion-parameter decision model for fast, typed judgments from clinical records, along with two agentic harnesses in which CS1 works together with a generalist language model. CS1-4B is trained on 12.4 million questions and answers from 3.6 million patients across a multi-hospital health system, combining structured-data keys, observed outcomes and language-model supervision across clinical notes, diagnostic reports and patient timelines. It answers multiple typed questions in a single forward pass without task-specific retraining, and each answer carries a probability that can route uncertain cases to human review. On 963,408 held-out patients, CS1-4B outperformed open decision models up to 27 billion parameters on 13 of 14 tasks scored independently of its training teacher. Across 21 external data sets, its aggregate performance approached that of the strongest tested 27-billion-parameter model, with 6.4-fold faster inference in a matched workload. Integrating CS1-4B with a language model agent produced cited answers over complete multi-year patient histories and screened a patient population against the eligibility criteria of 17 registered clinical trials, placing four times as many judged-eligible patients among its top 20 candidates as keyword search while using 690-fold fewer language-model tokens than a language model reading every record. These findings support a division of labour in clinical AI, with small decision models performing repeated record reading and generative models formulating questions and synthesizing evidence.

---

## 46. Same Simulation, Different Evidence: Where Retrieved Tool Output Costs LLM Agents Accuracy

**Autori:** Ke Zhang, Sahchit Chundur, Jerry Peprah Owusu, Mohammad Javad Abdolhosseini Qomi, Maziar Raissi  
**Data:** 2026-10-19  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.26836v1

> LLM agents that compute the right answer can still answer wrongly. Agent harnesses increasingly keep long tool outputs out of the context window, saving them to files that the agent searches or reads on demand. We ask where this costs accuracy with a real scientific tool: PHREEQC, a widely used geochemistry simulator from the USGS, whose reports reach 846.8k characters and whose determinism lets every printed value be traced. Agents use it to answer 158 execution-verified multiple-choice items. When agents read the simulator's report through a section index rather than in context, GPT-5.1 and GPT-5.2 lose 11.3 and 7.9 points of accuracy, while Claude Opus 4.6 and Claude Sonnet 4.6 show no detectable cost. Re-running all 11,007 logged simulator calls shows that both GPT models compute the keyed value about as often as before; what changes is the evidence they answer from. Under retrieval they often skip the report, answer from their own higher-precision output files, and misround to a neighboring option, a failure we call evidence substitution. With the simulation held fixed, retrieval still costs GPT-5.2 9.4 points. For GPT-5.4, more frequent correct simulations mask an evidence-use loss of about ten points, leaving a net change indistinguishable from zero. Naming the authoritative output raises accuracy by 6.3-7.9 points over plain retrieval for the three GPT models; for GPT-5.1 and GPT-5.2, inlining outputs that fit works as well, while asking for correct rounding does not. Context-management choices in agent harnesses should be judged by where accuracy is lost, not only by final accuracy.

---

## 47. VerifierBench: Benchmarking the Generation of Executable Verifiers for LLM Agents

**Autori:** Jianing Yin, Ziyi Chen, Hao Wang, Yiyou Sun, Zijian Jin, Dawn Song, Daoan Zhang  
**Data:** 2026-10-19  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2610.28679v1

> Agents need reliable ways to validate their outputs, both when completing tasks and when filtering synthetic training data. We study verifier generation: from the instruction and environment available for solving a task, an agent writes an executable verifier that must accept every valid solution and reject invalid ones. We introduce VerifierBench, a benchmark of 222 tasks from six agent benchmarks spanning tool-call, state-based, and code verification, with 4,993 hidden test cases that include alternative valid solutions and attacks; Verifier4Verifier (V4V), a six-check audit, screens its source verifiers and test suites. Across 19 models in a common agent harness, normalized balanced accuracy ranges from 10.6 to 62.1, with generated verifiers consistently rejecting invalid solutions more reliably than they accept valid ones. This apparent strength can mask overly restrictive verification: most false rejections in the analyzed records come from verifiers that accept no tested solution to a task. Case studies reveal unsupported assumptions about solution formats, tool use, and code changes that exclude valid solutions. These errors survive self-testing because agents test solutions that share the verifier's mistaken assumptions, or submit verifiers without confirming that any correct solution passes. These findings suggest testing both whether a verifier accepts a correct solution and whether it accepts other solutions permitted by the task. The project page and dataset are publicly available.

---

## 48. When the harness decides success: state that cannot be re-observed

**Autori:** Raimondas Lencevicius  
**Data:** 2026-10-19  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2610.26632v1

> Agent harnesses decide what a language model sees across turns: they drop old turns, summarize them, or replay the model's own earlier reasoning. We ask when these choices change whether an agent succeeds, not only what it costs, and report three findings. First, in a pre-registered synthetic probe, truncating the context window costs a low-cost reasoning model nothing in success when a needed fact can be looked up again (it looks the fact up instead), but drops its success to chance when the fact cannot be re-observed: the two penalties differ by 92.5 percentage points (90% CI [89.5, 95.5]). A pre-registered replication on one model from a second provider showed the same contrast. Once the fact was lost, that model chose no answer rather than guessing. Second, on ARC-AGI-3, where the benchmark's Standard harness trails its Provider Adapter harness by a wide margin, we decompose that gap one component at a time, for one model on four games. Summarizing old turns instead of dropping them, while keeping the Standard harness's invitation to take notes, recovers 86% of a 63-point gap without replaying the model's reasoning. The same harness without the invitation recovers 43%, and adding the provider's native replay of the model's reasoning recovers the remaining 57%. These are point estimates from one counted run per configuration and game, and the replay share depends on a single run. Third, in the benchmark's published runs and in ours, the Adapter's advantage in the probability of clearing a level it has reached is larger at deep levels than at early ones. This largely restates where runs stopped and does not separate a growing advantage from a constant one.

---

## 49. Reliable Before Profitable: QuantHarness for Governing Financial Strategy Development with LLM Agents

**Autori:** Jiasheng Mao, Jiacheng Liu, Hengwei Ye, Zheng Tian  
**Data:** 2026-10-19  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.26101v1

> LLM agents can turn natural-language financial research requests into executable and backtested strategies, but a successful run may still implement the wrong rule, use information unavailable at decision time, or obscure how repairs and candidate selection changed the strategy. Because these failures arise throughout development, final code and performance metrics alone are insufficient to establish either fidelity to the request or the validity of the development process. We therefore address the reliability of financial strategy development at the trajectory level: the system must control how intermediate outputs become downstream state and preserve the evidence needed to justify the terminal outcome. We introduce QuantHarness, a two-layer agent harness in which a finance-specific Workflow structures specification, data grounding, construction, testing, and review, while Harness Core enforces stage-specific information, action, and commitment boundaries. We also introduce FinRelBench, a benchmark that evaluates strategy-development reliability through execution success, requirement satisfaction, and runtime evidence. QuantHarness achieves the highest Task Success at 90.72\%, compared with 74.23\%--84.54\% for the comparison systems. Controlled stress tests show that its boundaries contain targeted violations, while structured run records improve evidence retrieval and support decision replay under the evaluated protocol.

---

## 50. Secure Agentic Coding through Counterexample-Grounded Feedback

**Autori:** Tue Le, Anh Nguyen Hoang, Gabriel Sasseville, Doseok Jang, Pierre-Luc Bacon, Nghi D. Q. Bui  
**Data:** 2026-10-19  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2610.25916v2

> As coding models and agent harnesses become more capable, reliable security verification is becoming a central bottleneck. Improving secure code generation requires a signal whose reported progress remains aligned with actual program behavior under optimization; otherwise, an optimizer can improve the signal's verdict without removing the underlying vulnerability. Existing model-based approaches require models to either infer program behavior from source code or specify correct outcomes for adversarial tests, placing substantial reasoning demands on the security signal. We introduce \falcon{}, a counterexample-grounded verification framework that separates attack exploration from behavioral verification and connects them through execution traces of the program under test. In test-time repair, \falcon{} yields substantially stronger held-out functional-security gains than alternative security signals across secure code generation benchmarks, while preserving or improving functionality. As an RL reward, \falcon{} also outperforms static-analysis and learned rewards on held-out functional-security, even when all policies successfully optimize their respective training rewards. Combining \falcon{} with either proxy reward further improves held-out performance, suggesting that execution-grounded feedback can mitigate reward overoptimization while preserving useful guidance from existing security signals.

---

## 51. OR-License: Evaluating LLM Agents as Real-World Operations Research Practitioners

**Autori:** Peisong Wang, Feixue Liu, Yize Meng, Bowen Liu, Ruoyu Chen, Gaoyang Dai, Xing He, Aiqian Li, Fengchi Yuan, Aochuan Chen, Chenyi Zi, Yuhan Li, Hongchuan Zeng, Yimo Yan, Nuo Chen, Jie Fu, Zuo-Jun Max Shen, Yong-Hong KUO, Jia Li  
**Data:** 2026-10-16  
**Categorie:** cs.CL, cs.AI  
**Link:** https://arxiv.org/abs/2610.24087v1

> Can large language model (LLM) agents deliver expert-level operations research (OR) solutions directly from original client materials, without prior expert reformulation? Existing OR benchmarks typically begin with self-contained descriptions or predefined optimization tasks, underrepresenting the translation of original business materials into professionally validated solutions. We introduce OR-License, an end-to-end benchmark of 31 instances across 10 industrial scenarios from paid OR engagements totaling USD 3.68 million. It preserves original requirements, input data, deliverable formats, and information boundaries after de-identification. To study information acquisition, we introduce ORSim, a controlled client simulator that discloses business facts without supplying OR expertise. Hidden evaluation checks feasibility and compares objective quality against original expert solutions accepted by clients before benchmark construction. Deployment-Adjusted Quality (DAQ) averages expert-relative quality across instances, assigning zero to infeasible deliveries. Across 11 frontier LLMs using coding-agent harnesses, several exceed the expert reference in conditional objective quality, but none matches its DAQ; the strongest primary Claude Code configuration achieves 88.39% strict feasibility and a DAQ of 0.87 against the expert reference of 1. Client information acquisition extends beyond clarification into solution development and validation, with some later stages showing higher confirmed issue-resolution proportions. Trajectory analysis identifies formulation and implementation failures, while task-equalized research-chain completion rates range from 24% to 45% across models on evaluable tasks. These findings motivate sustained information-gap resolution, faithful problem formulation, and evidence-linked self-improvement for reliable long-horizon agents.

---

## 52. DrugHarness: An Evolvable Agent Harness for Computational Drug Discovery

**Autori:** Yuxing Chen, Zhisheng Zhang, Cheng Tang, Wei Li, Minghui Zhang, Ziyan Huang, Shaocong Wei, Jiawei Chen, Junru Hu, Hongze Zhu, Jianghan Shen, Min Cen, Xinyuan Zhu, Yaxue Zhao, Jubo Wang, Yuqiang Li, Chun-Mei Feng, Zongyuan Ge, Rui Su, Jie Xu, Yirong Chen, Xi Xu, Ming Hu  
**Data:** 2026-10-16  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.23791v1

> Computational drug discovery requires agents to compose scientific operations and adapt to changing evidence and constraints. Here we introduce DrugHarness, an evolvable agent harness coupling composable scientific execution with conditional skill induction. Its environment integrates over 80 scientific operations, biomedical resources and task-specific code, preserving associations among candidates, results and artifacts. From execution trajectories and outcome feedback, DrugHarness induces action hypotheses with observable applicability conditions, recommended actions and supporting evidence. An independent review agent evaluates candidate skills derived from these hypotheses through source verification and, when needed, targeted execution trials. Admitted skills guide subsequent tasks and are revised through feedback. Evaluation on MolBench and SMDD-Bench demonstrates capabilities in molecular screening, optimization and constrained design. Without evolution, DrugHarness exceeds reported MolClaw-CC results by 10.8 percentage points in affinity-comparison accuracy and 55% in mean top-three active hits on MolBench. Retrospective evaluation on skill-development tasks shows that evolution increases Qwen's affinity-comparison accuracy from 62.2% to 81.1% and optimization success from 79.5% to 87.2%. In a prospective HPK1 study, DrugHarness achieves a more favorable median docking score than Biomni among system-specific candidates. A synthesized compound achieves a cellular IC50 of 14.19 nM, a 2.64-fold potency improvement over the best input reference, with activity competitive with two selected compounds designed by experienced medicinal chemists. These results support conditional skill evolution for scientific agents and demonstrate a workflow connecting computational drug design with experimental validation.

---

## 53. IRAH: Hierarchical Agentic Tree Search for Retrieval Pipeline Optimization

**Autori:** Maria Ana Cardei, Aniket Singh, Amir Moghadam, Srividhya Baikadi, Rashmi Shetty  
**Data:** 2026-10-16  
**Categorie:** cs.IR, cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2610.30167v1

> Optimizing Information Retrieval (IR) pipelines for Retrieval-Augmented Generation (RAG) requires jointly selecting structural components and numerical hyperparameters under limited evaluation budgets. We introduce the Information Retrieval Agentic Harness (IRAH), which combines Language Agent Tree Search for IR (LATS-IR) with offline meta-learned initialization. LATS-IR performs UCT-guided hierarchical search, first exploring macro-structural pipeline choices and then refining numerical parameters, with natural-language reflections to guide subsequent mutations and provide inspectable search traces. We evaluate IRAH on three in-distribution benchmarks and one out of-distribution benchmark to assess generalization under distribution shift. Under the same meta-learned initialization, LATS-IR outperforms TPE on two of three in-distribution benchmarks, with gains of up to 6.4%, and remains competitive on the out-of-distribution benchmark. Across all four benchmarks, warm-started IRAH achieves the highest average held-out nDCG@10 (0.4816) and improves over its cold-start counterpart. These results establish IRAH as a competitive approach to retrieval pipeline optimization under constrained evaluation budgets.

---

## 54. MuninAI: A Self-Hosted Agentic Framework for Independent Research Groups

**Autori:** Markus Fischer, Jens Meiler, Matthias Elgeti  
**Data:** 2026-10-16  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2610.23480v1

> Research groups that want a language model grounded in their own literature face a choice between hosted services that receive their unpublished work and self-hosted deployments that keep the data local but give the model no access to the corpus. Munin is an open-source framework for a self-hosted scientific assistant that indexes a group's corpus and its citation graph, and wraps whichever open-weight model the group can serve in an agent harness with specialised reading, search, and computation tools. We claim that the harness, rather than the specific model, is what makes the system useful on domain literature, and we ship the evaluation suite that tests this claim with the software. On 199 paired literature questions, the harness more than doubles the accuracy of the base model, from 0.387 to 0.874 (+0.487, 95% CI [0.407, 0.568]), while naive retrieve-then-answer scores below the unaided model on every backbone tested. Under the harness, roughly twice as many answer claims trace to a passage the model read itself as with fixed top-5 retrieval. When the source paper for a question is removed from the corpus, the system abstains on about nine in ten of the questions it had answered correctly on the Qwen backbones and eight in ten on gpt-oss-20b, and it produces no fabricated local citation across 300 fabricated references. The pattern holds on three backbones from two developers, including a 20-billion-parameter model that runs on a single consumer-grade GPU. With all outbound network access disabled, both Qwen backbones still exceed the published PaperQA2 accuracy. The evaluation suite runs as a single command, so an adopting group can re-run it on its own corpus and model.

---

## 55. GatewayBench: Unified Capability and Security Evaluation Platform for MCP Gateways

**Autori:** Yitian Zheng, Zhaorun Chen, Haoyu Li, Bo Li  
**Data:** 2026-10-16  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.23449v1

> AI agents have increasingly interacted with external environments by invoking tools, with Model Context Protocol (MCP) emerging as a standard interface for connecting agents to heterogeneous tools and services. As organizations deploy agents at scale, MCP gateways have become a critical middleware layer for aggregating, governing, and shaping the tool surface exposed to agents. Despite the growing importance of MCP gateways in agentic systems, no prior work has systematically studied how gateway design affects agent capability, efficiency, and security. To address this gap, we introduce GatewayBench, the first unified evaluation framework and benchmark for MCP gateways. We characterize gateway architectures into two major paradigms: flattened gateways and hierarchical gateways. GatewayBench comprises 524 tasks across six domains, together with a pool of 11,118 real-world tools from 251 authentic MCP servers. To emulate large-scale deployments, we systematically inject task-irrelevant tools sampled from this pool into each agent environment, enabling controlled evaluation as the accessible tool surface scales. Based on GatewayBench, we conduct extensive experiments across seven widely deployed MCP gateways and diverse agent configurations, covering both benign and adversarial tasks. Our results reveal substantial differences across gateway designs in task completion, tool-use efficiency, and resilience to attacks, and further demonstrate that these effects interact strongly with the underlying model and agent harness. These findings highlight the MCP gateway as a consequential yet underexplored component of the agentic AI stack. By enabling controlled evaluation of gateway architectures under realistic tool ecosystems, GatewayBench provides both practical guidance for MCP gateway design and a rigorous testbed for developing more capable, efficient, and secure agentic systems.

---

## 56. Benchmarking and Enhancing Agentic Causal Discovery

**Autori:** Pingchuan Ma, Rui Ding, Shuai Wang  
**Data:** 2026-10-16  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2610.22846v1

> LLM agents can now run causal discovery algorithms on a dataset and report what comes out. Whether they do more than that, such as noticing where an algorithm went wrong and fixing it with further tests, is hard to tell from current benchmarks. Most of them give the variables meaningful names, and an LLM shown only the names of the Tübingen cause-effect pairs already gets 99% of the directions right. With the names removed, the data are usually clean enough that picking a better algorithm than PC closes most of the gap. We introduce Heuresis, a benchmark of anonymous simulated datasets whose mechanisms range from linear Gaussian to heavy-tailed. For each family of datasets it separates what a better existing algorithm can gain from what only a closer look at the data can gain, and it traces every edge an agent changes. Every family leaves a gap that none of the algorithms, the router and the two causal-discovery foundation models we ran can close, so a score above the best chosen algorithm has to come from using the data. We instantiate the benchmark with an agent harness and three LLMs, GPT-6.1 Sol, Claude Opus 5.5 and Qwen 3.8 Flash. GPT-6.1 Sol surpasses the best chosen algorithm on all six families, by 14% adjacency F1 on the most difficult one, and Claude Opus 5.5 does so by 7.4% there. A third of the true edges the two agents restore on the two hardest families appear in no algorithm's output. The code and data will be publicly released to facilitate future work.

---

## 57. Has GPT-6-Astra Achieved Embodied Intelligence?

**Autori:** SenseNova, Joint Research Team, Zhongang Cai, Ziang Cao, Tailai Chen, Han Chong Chua, Linjun Dai, Hanming Deng, Hokin Deng, Haiwen Diao, Chenjing Ding, Weichen Fan, Xiao Fu, Zerui Gong, Chenyang Gu, Zexin He, Zhi Hou, Bo Li, Qinyue Li, Quanzhou Li, Xiaowan Li, Zhichao Liao, Dahua Lin, Zilong Lin, Bo Liu, Chunxiao Liu, Pengfei Liu, Tianqi Liu, Ziwei Liu, Chen Change Loy, Lewei Lu, Jiapeng Luo, Yuexiao Ma, Liang Pan, Xingang Pan, Oscar Qian, Ziyi Shang, Yuyao Shao, Dawei Su, Dacheng Tao, Qingyi Tao, Quan Wang, Ruisi Wang, Xiaogang Wang, Ziyi Wang, Beichen Wen, Donghao Wu, Jiaxu Wu, Silei Wu, Xiaoming Wu, Zhonghua Wu, Hongcan Xiao, Weiye Xu, Atsushi Yamashita, Lei Yang, Zhe Yang, Baiqiao Yin, Wanqi Yin, Hanfei Zhao, Tianbo Zhong, Long Zhuo, Jing Zuo  
**Data:** 2026-10-15  
**Categorie:** cs.RO, cs.CV, cs.LG, cs.MM  
**Link:** https://arxiv.org/abs/2610.22471v2

> GPT-6-Astra demonstrates a level of competence in robotic manipulation and navigation that challenges the conventional paradigm of building specialized models for individual tasks and embodiments. In this report, we ask not only how capable GPT-6-Astra is, but what its capabilities imply for the field. First, we probe the limits of standalone GPT-6-Astra. We conduct a large-scale evaluation across 12 representative benchmarks spanning tabletop manipulation, humanoids, mobile platforms, and dexterous hands. Under a unified protocol that allows in-context learning (ICL) from training-set demonstrations and substantially increases the number of execution steps, GPT-6-Astra achieves unprecedented performance (Fig. 1). Future research may focus on improving 1) the generality of ICL 2) cost and execution time, 3) physical-state verification, 4) recovery from irreversible failures, and 5) long-horizon preservation of progress. Second, we study the agentic harness for embodied control. We identify that close-loop coordination between a high-level "System 2" reasoner (i.e., GPT-6-Astra) and a low-level "System 1" controller (e.g., π0.5) is costly but effective. Third, we examine GPT-6-Astra on real-world deployment. Our experiments on 8 robot configurations reveal substantial gaps: 1) robot demonstrations required for ICL are expensive to collect, and 2) it is implausible to trade longer execution for higher success rates with physical constraints. Fourth, we envision the next generation of embodied benchmarks. We develop a prototype that 1) derives tasks from real-world needs, 2) provides no in-domain demonstrations, and 3) judges agents on a world clock that keeps running while they deliberate. Taken together, our results suggest that GPT-6-Astra has largely crossed the threshold of embodied competence, but not yet that of practical embodied intelligence.

---

## 58. Harness-Delta Attribution: Dissecting Gains From Harness Evolution

**Autori:** Wenxuan Ding, Qin Lu, Changlong Yu, Sha Li, Shuowei Jin, Xin Liu, Zhenyu Shi, Greg Durrett  
**Data:** 2026-10-15  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.22466v1

> Harness evolution automatically optimizes the prompts, skills, tools, and orchestration code around a fixed-weight model, offering a way to improve agentic systems without updating model weights. The agent harness is iteratively optimized to achieve higher performance on the search set. But how much of this gain reflects benchmark-specific overfitting or additional inference-time compute, and how much may generalize beyond the search set? In this work, we introduce Harness-Delta Attribution (HDA), an evaluation protocol that dissects an evolution gain into artifact-driven overfitting, gains explained by test-time scaling, and the remainder, which gives an upper bound on residual generalizable improvement. We apply HDA to 11 executor models and three harness-evolution frameworks across math, coding, creativity, and agentic tasks. In 21 of these settings that show statistically significant search-set gains, we find that a large share of the improvement is explained by overfitting or test-time scaling. Specifically, among these 21 settings, overfitting and test-time scaling account for 54% and 14% of the gain on average; their combined share exceeds 50% in 14 settings. The residual and held-out transfer vary substantially across tasks, models, and frameworks. Importantly, search-set gains often fail to transfer to held-out tasks, and provide limited evidence that they will persist under practical distribution shifts. Moreover, validation-based signals are insufficient to prevent overfitting. These results motivate attribution-aware evaluation in future harness evolution research.

---

## 59. Librarian Agents: Training LLMs to Curate Long-Context Workspaces that Anticipate Future Queries

**Autori:** Anikait Singh, Teresa Zhang, Yoonho Lee, Roshen Sanjay Nair, Aviral Kumar, Chelsea Finn  
**Data:** 2026-10-15  
**Categorie:** cs.LG, cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2610.22273v1

> Reasoning over long document contexts remains a challenge for large language models (LLMs). Standard retrieval methods are inherently reactive, bottlenecking agents with complex, cross-document reasoning at inference time, while precomputed structures like knowledge graphs often fall short because they rely on rigid heuristics. Instead, can we allow agents to perform anticipatory directed curation: learning to proactively reorganize unstructured corpora prior to inference to efficiently serve diverse future queries. We build on a key asymmetry in modern agentic harnesses (e.g., Claude Code): while LLM agents are adept at navigating existing filesystems to solve an immediate task, they are rarely trained to construct reusable workspaces for future use. To instantiate this capability, we introduce Librarian Agents, a framework in which a builder agent transforms raw documents into a hierarchical filesystem of synthetic files and reference links, which forms a workspace tailored for a downstream answering agent. We formulate workspace construction as a Markov decision process and optimize the builder policy via reinforcement learning to directly maximize downstream answering accuracy. Empirically, Librarian Agents outperforms the strongest retrieval and precomputation baselines by 33 percentage points on BrowseComp-Plus, amortizes upfront construction costs across repeated queries, and generalizes zero-shot to unseen domains on BRIGHT with a 31-point average accuracy improvement.

---

## 60. Priming Base Models for Agentic Post-Training: An Open Midtraining Recipe

**Autori:** Soumye Singhal, Joseph Jennings, Ka Shun Shum, Alexander Bukharin, Khushi Bhardwaj, Zirui Liu, Venkat Srinivasan, Jonathan Li, Yash Jain, Kezhi Kong, Markus Kliegl, Olivier Delalleau, Sanjeev Satheesh, Mostofa Patwary  
**Data:** 2026-10-15  
**Categorie:** cs.CL, cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2610.22019v1

> Frontier models, general-purpose and domain-specific alike, now include a midtraining stage between pretraining and post-training, but little has been published about how this stage is built. We present an open midtraining recipe that primes base models for agentic post-training, and we show its effectiveness on two Nemotron models of different sizes. Pretraining typically runs at short context and sees almost no agent interactions, while SFT data is mostly synthetic, and very long SFT stages can hurt the model's later RL trainability. Our midtraining stage sits between the two. It trains at 256K context for hundreds of billions of tokens on a diverse mixture of natural software-engineering data like packed repositories, pull requests, commit histories, and build logs together with a small share of agentic traces. On Nemotron 3.5 Lightning, 500B midtraining tokens improve SWE-bench Verified from 60.7 to 64.5, SWE-bench Multilingual from 55.8 to 62.8, and SWE-bench Pro from 32.0 to 35.5 after identical full SFT. On the larger Nemotron 3.5 Super, 280B midtraining tokens improve DeepSWE, a harder benchmark of long-horizon tasks, from 11.7 to 15.7 and SWE-bench Verified from 72.9 to 74.3 after identical full SFT. Midtraining also improves robustness across agent harnesses on both models. We report the ablations behind the recipe and an evaluation protocol built on short fixed SFT runs, since base-model proxy metrics did not correlate reliably with post-training results.

---

## 61. DeciCAD: Harness-Grounded Learning of Action Policies for CAD Agents

**Autori:** Yufeng Peng, Yixin Zhang, Ziyi Liu, Zhikun Xu, Jiarong Yang, Sijie Wang, Wenjie Feng, Qiyu Kang  
**Data:** 2026-10-15  
**Categorie:** cs.AI, cs.CL, cs.LG, cs.RO  
**Link:** https://arxiv.org/abs/2610.21755v1

> Large Language Model agents operate through closed-loop action policies whose decision space is defined by an agent harness. We investigate how this operating space shapes agent behavior and policy learning in computer-aided design (CAD), a professional domain characterized by persistent state, geometric constraints, and long-horizon procedures. We instantiate this perspective in DeciCAD, a domain-native harness that exposes semantic CAD actions, decision-oriented observations, environment feedback, and persistent state transitions. Building on this harness, we develop a learning pipeline that extracts causal decision supervision from interaction trajectories and improves the policy through supervised fine-tuning (SFT) and geometry-grounded online reinforcement learning (RL). Across four CAD benchmarks, DeciCAD achieves the best F1 and intersection over union (IoU) while reducing model-output tokens by 45--88% relative to a general-purpose coding harness. Under matched supervision, its SFT policy improves F1 from 0.6883 to 0.7437 and outperforms the coding policy; subsequent online RL further raises geometry availability from 66.5% to 73.5% and F1 to 0.7880. These results demonstrate that the decision space induced by a harness materially affects both agent execution and policy learning in CAD.

---

## 62. A Strong Harness Narrows the Model Gap: A Comparative Evaluation for Legislative Document-to-XML Conversion

**Autori:** Palvika Bansal, Rittika Jindal, Ruichong Wang  
**Data:** 2026-10-14  
**Categorie:** cs.CL, cs.AI  
**Link:** https://arxiv.org/abs/2610.19999v1

> Legal-content reproduction requires matching the source exactly in section hierarchy, verbatim text, citations, and amendment spans; a dropped citation or mislabeled amendment carries into the products lawyers rely on. We report an industrial pipeline converting U.S. state legislation into strict, schema-constrained XML, and hypothesize that its accuracy comes from harness engineering, the deterministic tooling built around a model, more than the model itself. Our controlled ablation crosses three harnesses (zero-shot, a single tool-using agent, and a decomposed multi-agent pipeline) with three Claude models on 153 gold bills from two jurisdictions. The harness narrows the model gap: the weakest model in the full pipeline beats the strongest model alone (0.948 versus 0.806, paired bootstrap p less than 0.001). Because the two agentic harnesses share identical tools, their gap comes from orchestration: decomposition plus the persisted state and per-agent context it brings. Across four scored dimensions, the model spread at zero-shot (0.68 to 0.81) narrows to 0.95 at the full pipeline; the residual sits almost entirely in citation normalization, where the canonical identifier is retrieved from an external authority rather than generated from the weights, so a deterministic lookup tool supplies the exactness that a larger model does not.

---

## 63. BluePixel: Toward Native 4K Agentic Image Editing

**Autori:** Shanyan Guan, Shiyu Li, Xin Li, Zhizhou Chen, Yunzhe Xu, Yuehao Liu, Ruixue Shen, Shiju Zhang, Min Jin, Qiang Liu, Junbo Liu, Penggang Shi, Sheng Sun, Xiao Wang, Yong Zhang, Zhongang Qi, Wei Li, Chao Ma, Ying Tai, Yanhao Ge  
**Data:** 2026-10-14  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2610.19882v1

> Instruction-driven image editing has reached native 4K, yet how such editors are trained remains undisclosed, and pretraining one from scratch is beyond most teams. The task itself compounds the difficulty: a single end-to-end editor cannot make precise parametric adjustments, match specialized experts, or interpret the vague instructions users actually write. We argue that 4K editing is a system problem rather than a single-model problem, and present BluePixel, which couples a native-4K editing model with an agent harness; the complete training recipe is disclosed in this paper. The model makes 4K training practical: it turns a 1K-pretrained editor into a native-4K one through progressive VAE adaptation that keeps 4K training as affordable as 1K, absorbs a long tail of vertical editing skills through continual learning, and refines the aesthetic-fidelity trade-off with reinforcement learning. Distillation via source-anchored target projection (SATP) then compresses 50 denoising steps to 4, completing a 4K edit in 8.7 s on a single Kunlunxin P800 XPU while preserving task success rate and background consistency. The harness, BluePixel Agent, makes editing controllable: it decomposes user instructions into specialist and general operations, verifies every result with the same reward model that guided training, and retries within bounded attempts. On VINS-4KEval++ (3,305 native-4K cases), BluePixel ranks second among seven models, behind only GPT Image 2 in non-edited-region consistency.

---

## 64. Why Do Agent Teams Fail Across Boundaries? A Failure Taxonomy for Agent-to-Agent Systems with Private States

**Autori:** Sarath Shekkizhar, Prathyusha Jwalapuram, Zixuan Ke, Vaidehi Patil, Jiayu Wang, Srijan Bansal, Trong Huy Nguyen, Dingfeng Jiang, Dongqi Liu, Ruochen Zhao, Wei Lu, Giuseppe Carenini, Mohit Bansal, Silvio Savarese, Shafiq Joty  
**Data:** 2026-10-14  
**Categorie:** cs.MA, cs.AI  
**Link:** https://arxiv.org/abs/2610.19342v2

> Agents are increasingly interacting with other agents that act for different principals (people or organizations on whose behalf they work), such as a buyer's personal agent negotiating with an enterprise's seller agent. In such agent-to-agent (A2A) scenarios, each agent has its own environment and holds information and authority that the other cannot see. Moreover, the interests of each agent may be aligned (cooperative), partly aligned (mixed-motive), or opposed (competitive). Existing multi-agent system failure studies assume one orchestrator, shared workspace, or single principal. We ask how A2A systems fail when these assumptions are removed. We study more than 2,500 recorded runs of A2A systems built from different agent harnesses and models, spanning 488 scenarios across eight families (legal, CRM, security, commerce, etc.). From these traces, we derive $A^2$-Failures, a taxonomy of 20 A2A failure modes in four categories: (i) discovery and delegation, (ii) grounding and record consistency, (iii) verification, and (iv) conduct and fidelity. Three findings hold across every harness, model, and scenario studied: (1) discovery and interaction are driven by the phrasing of the task rather than the availability of peer agents; (2) no agent verifies a peer's factual claim on its own initiative, so an A2A system inherits the reliability of its least reliable participant unless the protocol or mechanism performs the check; and (3) the aggregate outcome score credits the agent completing the task while staying blind to the coordination, verification, and conduct failures beneath it, so A2A systems must be evaluated per agent, against each agent's own principal. We release the run logs behind the taxonomy at https://huggingface.co/datasets/a2a-salesforce/a2-failures.

---

## 65. Self-Evolving Agent Harness

**Autori:** Chuyang Wei, Haoxiang Guan, Minghang Zhu, Kexin Zhou, Jiyan He, Xiren Zhou, Huanhuan Chen, Yifei Shen  
**Data:** 2026-10-13  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2610.18813v1

> Harness self-evolution revises an agent's software scaffolding, including prompts, memory, workflows, and executable components, while keeping model weights fixed. We formalize a feedback-driven process in which accepted revisions persist across runs. The framework separates update targets from proposal and admission mechanisms. It distinguishes changes to interpreted state from revisions to tools and code, repository-level control logic, and plugin composition. We characterize search through evolutionary optimization and examine its reliability through continual PAC-learning. Under explicit assumptions, the analysis yields an expected generalization bound, a retention bound conditional on historical regression budgets, and a high-probability admission rule using fresh, independent validation data. We examine how persistent harness revisions affect knowledge sharing and organizational workflows, with implications for scientific reliability, physical safety, and institutional accountability. Cases from prior work illustrate model--harness co-design, distributed execution, and plugin reuse. Reliable deployment requires continual validation as task distributions and evaluators change, with independent safeguards for learning, runtime privileges, and consequential actions. We provide a comprehensive 66-page discussion of related work, theory, algorithms, evaluation, applications, and the broader impact of Harness RSI, together with continuously updated code and supplementary materials, at https://github.com/zgcagi/Harness-RSI.

---

## 66. Knowledge Graphs as Files: An Agent Harness Where Tool Creation and Tool Use Co-Evolve

**Autori:** Yuyang Bai, Yu Wang, Yu Zhang  
**Data:** 2026-10-13  
**Categorie:** cs.CL, cs.AI, cs.IR  
**Link:** https://arxiv.org/abs/2610.18616v2

> Searching text-rich knowledge graphs requires following relations while examining textual evidence. Predefined graph interfaces constrain what evidence agents can access, even when they write code to combine tool calls or process retrieved subgraphs. We propose direct knowledge graph interaction (DKGI), a harness in which language model agents create graph access tools directly over complete node and edge files. The agent writes Python code to follow relations, combine node sets, and select textual evidence, interleaving execution with shell search and file inspection. This lets agents process large node sets in bulk while returning selected text for the model to assess. Execution feedback guides tool creation and revision, while the evolving tools determine what evidence the agent gathers next. On benchmark datasets spanning three domains, training-free DKGI exceeds the strongest published baseline by at least 6.7 Hit@1 points on every graph, even with a minimal harness. Controlled ablations show the benefits of multi-turn programming over shell-only access and predefined graph tools, while trajectories show agents revising code to extend searches or address errors. These findings highlight the value of allowing tool creation and tool use to co-evolve during graph search. Our code and data are available at https://github.com/leopoldwhite/DKGI.

---

## 67. The Last Mile of Coding Agents for Long-Document Tasks: An Empirical Study on Clinical Trial Protocol Digitization

**Autori:** Jiacheng Lin, Geoffrey Low, Nishit Agarwal, Rahul Jain, Afrah Shafquat, Mandis Beigi, Jimeng Sun  
**Data:** 2026-10-13  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2610.18507v1

> Clinical trial protocols serve as the source of truth for study design, but are mostly written and used as unstructured PDF documents. Digitizing protocols turns static content into structured, machine-readable data that clinical software can analyze, validate, and execute. Coding agents, which select tools, execute code, and revise their approach as they work, are increasingly applied to such long-document tasks, yet it remains unclear how reliably they turn complete documents into accurate structured outputs. We study this question using protocol digitization as a testbed. We introduce TrialPD-Bench, an expert-annotated benchmark of 150 publicly available protocol PDFs spanning four task categories. Beyond final-answer performance, our evaluation measures evidence recall from agent traces, agent behavior, and cost. Across nine proprietary and open-weight models in five coding-agent harnesses, even the strongest agents do not fully solve protocol digitization. Our analysis further shows that agents usually locate the required evidence but fail in the last mile of transcribing and structuring it. We further develop TrialScribe, a domain-specific harness that equips coding agents with task skills and a verification loop. TrialScribe improves a locally served open-weight model by 6.2-59.4 points across eight metrics, enabling it to match or surpass proprietary models such as GPT-5.6-Sol.

---

## 68. Let the Mind Conceive, Let the Hand Achieve: Following Multimodal Instructions for Long-Horizon Robotic Manipulation

**Autori:** Youpeng Wen, Gang Wang, Tianyu Huang, Weiwei Zhang, Zhijian Huang, Wei Chen, Xieyuanli Chen, Yunhui Liu  
**Data:** 2026-10-13  
**Categorie:** cs.RO, cs.AI  
**Link:** https://arxiv.org/abs/2610.18352v1

> A robot following a multi-step instruction needs to act on the right objects in the right order, even as the scene changes. It must also maintain awareness of task progress and determine when to advance. To address these challenges, we introduce Orchestra, an agent harness that separates task planning and execution management from action generation. Orchestra decomposes a complete multimodal instruction into ordered subtasks, tracks completed steps, and updates the locations of relevant objects and destinations during execution. It maintains a shared context containing the active subtask, spatial grounding, and recent observations. An action policy uses this context to generate actions, while a separately trained progress evaluator estimates when to advance to the next subtask. To evaluate whether robots trained on atomic instructions and short trajectories can execute longer subtask sequences, we introduce a benchmark named RMBench-Compose. Orchestra achieves a mean success rate of $68.22\%$ across nine RMBench tasks, outperforming Mem-0 by $26.22$ percentage points. On RMBench-Compose, it achieves an Average Success Length (ASL) of $7.35$ subtasks, $2.46$ times that of HarnessVLA. Across four real-world multi-step tasks, it improves mean ASL by $25.0\%$ over Orchestra using the base $π_{0.5}$ policy. These results show that Orchestra helps robots carry out longer sequences of subtasks while preserving the requested subtask order and acting on the specified objects. Our code and project page are available at https://youpengwen.github.io/Orchestra.

---

## 69. Jev-Guard: Fast Routing and Auditing Agent Actions over Editable Policy Trees

**Autori:** Wenbin Hu, Huihao Jing, Haochen Shi, Yuxuan Liu, Changxuan Fan, Sirui Zhang, Kawai Chung, Hanyu Yang, Zhenhuan Wang, Ziyi Chen, Haoran Li, Yangqiu Song  
**Data:** 2026-10-13  
**Categorie:** cs.CR, cs.CL  
**Link:** https://arxiv.org/abs/2610.18326v1

> Agent harnesses require a low-latency guardrail model together with customizable audit policies. However, deploying an auto-regressive guardrail model remains challenging: such models incur high inference latency and are often poorly aligned with customized policies. To address these problems, we present Jev-Guard, a unified model for safety classification and policy routing. We further construct a policy tree over which Jev-Guard performs routing, spanning diverse domains including content moderation, cybersecurity, privacy, and legal compliance. Specifically, Jev-Guard first navigates the policy tree to select the applicable audit policy given the caller's audit context, and then performs safety classification conditioned on the retrieved policies. On 7,033 evaluation cases, Jev-Guard achieves 93.72\% safety accuracy, a mean latency of 58ms, and 93.10\% hierarchical routing accuracy. The full routing-and-classification pipeline averages 240ms. Furthermore, we integrate Jev-Guard into the Hermes harness framework. Across agent trajectories, its separate permission gate cuts mean review time per task from 4.80s for an SFT-LLM judge to 1.33s, with no policy violations are observed for either guard.

---

## 70. Holding Agents Accountable with Verifiable Agent Insurance

**Autori:** Cheng Hua, Taro Tsuchiya, Nicolas Christin, Giulia Fanti  
**Data:** 2026-10-13  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2610.18230v1

> While AI agents are useful for many tasks, they regularly misbehave in destructive ways, such as deleting important data. While prior work has focused on preventing such misbehavior, we consider how to recover after an agent misbehaves. We propose verifiable agent insurance (VAI), a framework for agent providers to commit financially to promises, a list of programmatically-specified policies that an agent is meant to follow. These promises are embedded in a smart contract on an immutable ledger (e.g., a blockchain) to prevent tampering, along with a monetary escrow. A user who detects a violation of committed promises can prompt a verifier to review agent execution traces, which are logged through the agent harness's shared tool-execution path, without instrumenting each tool separately. Upon verification of the violation, the agent provider's escrow funds are paid to the reporting user. We instantiate VAI as an end-to-end implementation on an Ethereum layer-2 network, and evaluate its coverage on three prominent agent benchmarks, two of which we re-annotated to obtain task-level policy-compliance labels. Currently, many agents do not emit user authorizations and security-relevant information as explicit, structured data objects -- rather, they embed the data needed to verify policy violations in natural language exchanges. Even so, VAI manages to detect violations in 42.2% of runs containing violations across three benchmarks. By augmenting agents to explicitly emit such objects, violation detection rises to 83.0% of traces. Our findings suggest that for improved auditability, agents should be co-designed with their security policies to emit explicit, structured records of user authorization and security-relevant actions.

---

## 71. ResearchFlow-Eval: Tracing the Execution Gap in End-to-End Multi-Claim Autoresearch

**Autori:** Peng Jiang, Dongyang Li, Quanying Liu, Xiaoxuan Jia  
**Data:** 2026-10-13  
**Categorie:** cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2610.18088v2

> Autoresearch systems increasingly undertake entire research projects. In practice, scientific research requires systems to pursue multiple interdependent claims through a continuous, multi-stage workflow and revise experiments as evidence accumulates. Existing evaluations of autoresearch systems, however, typically score isolated tasks or final artifacts, leaving these process-level capabilities largely unmeasured. We therefore introduce ResearchFlow-Eval, a fine-grained framework for assessing continuous scientific execution and iteration at both the stage and claim levels. Each evaluation is grounded in a published anchor paper, from which we derive stage-specific rubrics that decompose each research stage into dimensions and separately scored rubric items. Using these rubrics, we score each research stage and examine experimental execution in detail, focusing on multi-claim completion and revisions across attempts. We apply the evaluation framework to general-purpose agent harnesses, skill-augmented harnesses, and systems with research-specific orchestration. Across all evaluated systems, experimental execution consistently lags behind design and planning. Within execution, systems struggle to produce high-quality results and meet claim requirements, and repeated attempts rarely yield measurable improvements. Moreover, neither skill augmentation nor research-specific orchestration reliably yields higher scores. ResearchFlow-Eval thus extends autoresearch evaluation beyond isolated, single-objective runs to continuous workflows in which systems pursue multiple claims and refine their work across iterations.

---

## 72. Code2Worlds-2: Physically Plausible Agent Harness for Embodied World Simulation

**Autori:** Haoyu Zhang, Siming Li, Zeyu Zhang, Yi Zhang, Tat-Seng Chua, Hao Tang  
**Data:** 2026-10-13  
**Categorie:** cs.RO, cs.CV  
**Link:** https://arxiv.org/abs/2610.17651v1

> Recent coding large language models (LLMs) can synthesize dynamic 4D worlds from natural language, but the resulting content remains a visual artifact. It lacks physical semantics such as the collision geometry, mass, friction, inertia, and joint structure, required to enable it to simulate the physical world, and its dynamics are scripted to look plausible rather than designed to execute. What is needed is an executable world: one that a physics engine can load and step, resolving contact physically. We present Code2Worlds-2, an extension of Code2Worlds that turns 4D world generation into an embodied world simulation. We keep the original dual-stream generation pipeline intact and append two modules. First, a SimReady Scene Compiler that turns a generated visual scene into a simulator-compatible representation: it assigns collision meshes via convex decomposition, estimates physical attributes with a vision-language model, infers a lightweight support graph, instantiates the engine's contact, friction, and dynamics constraints, and applies a gravity settling pass, before exporting the scene as MuJoCo MJCF. Second, a Simulator-in-the-Loop 4D Refiner that implements an automated agent harness-a compile, simulate, critique and refine loop-that converts visual dynamics into executable rigid and articulated dynamics and evolves the physical settings rather than only the code, replacing the purely visual motion critic with a simulator critic that inspects penetration depth, collision pairs, stability, contact forces, joint limits, and robot reachability. We further propose SimCode4D, a state-based benchmark with five task templates for evaluating embodied simulation. Experiments on SimCode4D and across natural, indoor, industrial, urban, and service scenes show that Code2Worlds-2 produces physically plausible, simulator-compatible, and robot-interactable scenes.

---

## 73. Verifier-Harness Co-Evolution for Training-Free Self-Improvement on Open-Ended Tasks

**Autori:** Tianyi Xu, Yaolun Zhang, Yiran Wu, Joe Nguyen, Shengyu Dai, Saba Moeinizade, Zhenwen Shao, Qingyun Wu, Huazheng Wang  
**Data:** 2026-10-13  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.17609v1

> Training-free self-improvement lets an agent use feedback to revise the response it is about to return and to update the harness state that shapes how it handles later tasks. On open-ended tasks that feedback rarely comes from reference answers or executable tests, so the agent has to rely on a model-based verifier. When the verifier is wrong, the current response can get worse, and misleading experience can persist across the task stream. A verifier that never changes also grows stale as the agent's responses improve and task demands shift. We introduce Unified Co-Evolution (UCoE), a training-free method that evolves an executable verifier program together with the agent's harness state while all model parameters stay fixed. UCoE synthesizes candidate verifier programs and tests them on response contrasts, pairs of responses that differ in one declared property and have a known preferred side. It selects the candidate whose discrimination on its weakest contrast family is highest, a quantity we call driving capacity. The selected verifier diagnoses one weakness in each draft, guides a single repair, decides which response is served, and determines whether the accepted repair may enter the harness state. As tasks complete, their diagnostics seed new candidate verifiers, which must beat the current verifier on the same contrasts before adoption. Across six open-ended benchmarks, UCoE averages 59.00% preference against matched direct generation with Qwen3-8B and 57.19% with Qwen3.8-27B, margins of 9.00 and 7.19 percentage points. On three verifiable benchmarks, the same method raises the mean from 36.06% for direct generation to 38.48%. Code is available at https://github.com/tianyi0216/Unified-Co-Evolution.

---

## 74. Scaling Inference-Time Compute with Teams of Coding Agents

**Autori:** Keenan Samway, Daniel D'souza, Omar Darwiche Domingues, Marzieh Fadaee, Tan Yi-Chern, Nouha Dziri  
**Data:** 2026-10-12  
**Categorie:** cs.MA, cs.CL  
**Link:** https://arxiv.org/abs/2610.17471v1

> Multi-agent systems promise a new axis for scaling inference: rather than having one agent think longer or sample more attempts, a task is split across many agents that work in parallel and coordinate. However, in practice, more agents can easily produce duplicate work, coordination failures, and higher costs. We therefore formulate team design as a compute allocation problem: starting from a solo agent, where should additional inference compute go to reach the reward-cost Pareto frontier? We build a minimal multi-agent harness from the ground up and trace this frontier by varying, one at a time, the workflow stage at which a lead delegates to its workers (planning, implementation, or verification), the models that form the team, and the number of workers. On ProgramBench, teams outperform solo agents but cost three to seven times as much. With the right compute allocation, however, a heterogeneous 17-agent team comes within 1.4 points of a strong homogeneous 5-agent team at 70% lower cost. This efficiency stems from three findings. First, planning is the most valuable use of workers: in a homogeneous team whose lead decides how many workers to spawn, a lead that delegates only planning to its workers, and then implements and verifies the code itself, matches the reward of a lead that delegates to workers throughout planning, implementation, and verification, at half the cost. Second, cheap models pay off as planners but not as implementers: a strong lead with cheap planners recovers 47.5% of the reward gain of an all-strong team for only 13.9% of its additional cost, whereas cheap implementers lower reward. Third, planners keep improving reward as the team grows, whereas implementers and verifiers plateau beyond four workers. Together, our results offer a guide to spending an agent budget where it counts, given the task, cost, and latency constraints a user has.

---

## 75. Learning to Design SR Solvers: Harness Optimization for Symbolic Regression

**Autori:** Qian Li, Yuxiao Hu, Qihao Duan, Jinyue Yan, Yuntian Chen  
**Data:** 2026-10-12  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2610.16966v1

> Symbolic regression (SR) seeks explicit equations that explain observed data, and recent methods increasingly employ large language models (LLMs) and agents for equation discovery. However, these systems typically rely on manually designed workflows and prompts. We argue that the SR agent harness should itself be an optimization target: its design shapes search priors and how numerical feedback guides subsequent equation refinement. We therefore propose HarnessSR, a framework for jointly optimizing prompts and workflows to construct reusable SR agents. During both harness optimization and agent execution, HarnessSR supports either PySR or an LLM-based equation generator through tool-specific interfaces, allowing the framework to optimize search guidance for different equation-discovery mechanisms. HarnessSR first optimizes role prompts through equation-discovery feedback in basic workflows, then jointly searches prompt assignments and workflows with brief adaptation to align the two. Finally, it refines role instructions through reflection on residual patterns, candidate equation structures, and search outcomes, improving how these signals guide subsequent equation search. On LSR-Synth in LLM-SRBench, HarnessSR achieves a mean ID $\mathrm{Acc}_{0.01}$ of 61.33% across three backbones, a 45.0% relative improvement over the next-best baseline.

---

## 76. Trace-to-Architecture: Capability Bottleneck Diagnosis for Harness Revision

**Autori:** Wenfeng Wang, Jianrui Shi, Mingang Guo, Jiayuan Ma, Yuqi Lu, Jiajun Sun, Guojiang Zhao, Jing Li  
**Data:** 2026-10-12  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.16725v1

> Improving an LLM agent requires knowing what to change when it fails. Similar failures can require different fixes, and resolving one problem can expose another. We introduce Trace-to-Architecture (T2A), a framework that uses execution trajectories to determine what to change in an agent's harness and when those changes apply. A development agent diagnoses failures using execution evidence from successful and failed tasks, revises the corresponding harness components, and then checks whether target tasks improve, selected successful tasks remain successful, and the edits are actually triggered. New execution evidence guides subsequent diagnosis and revision. Across ALFWorld, ScienceWorld, and AppWorld, T2A achieves the highest aggregate score for all three evaluated task agents, exceeding their respective strongest baselines by 6.2--30.3 points. We also integrate T2A's diagnosis and validation procedures into Meta-Harness, improving the resulting harnesses' mean ScienceWorld score by 21.6 points from the same starting harness.

---

## 77. CineRecon: Benchmarking Frontier Models for Agentic Cinematic Reconstruction

**Autori:** Jialei Wang, Zehan Wang, XiaoYang Wu, Ziang Zhang, Siyu Chen, Jiaer Huang, Yujia Zhang, Tianyu Pang, Hengshuang Zhao  
**Data:** 2026-10-12  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2610.16577v1

> Reconstructing reference videos as editable dynamic 3D scenes is an important path toward controllable video generation for filmmaking: these scenes provide modifiable, renderable visual proxies that enable explicit control over scene layout, subject actions, and camera behavior. To evaluate agents' ability to reconstruct editable dynamic 3D scenes from dynamic reference videos, we introduce CineRecon, a benchmark comprising 50 reference videos and 360 annotated evaluation clips. The reference videos span film, real-world footage, and games. Given a complete video, an agent uses tools to construct, animate, render, and refine its reconstruction. We evaluate this task under three representation settings: Proxy, Simplified, and Detailed. These settings increase geometric and appearance requirements while retaining the same requirements for spatial relations, camera behavior, and subject dynamics. This design tests whether agents can reproduce the events in a video when detailed appearance is unnecessary, and how performance changes as representation requirements increase. For evaluation, we construct checklists that associate observable properties and events with specific entities and times. A vision-language judge compares timestamp-aligned reference and rendered frames across 11 categories, grouped into camera, static, and dynamic consistency dimensions. We evaluate 12 models using their corresponding agent harnesses and find failures across all three dimensions. Subject motions and interactions remain difficult to reproduce even under the Proxy setting.

---

## 78. Unravel: Recovering an Interactive 3D Scene from a Single Image

**Autori:** Hui Shan, Keyang Luo, Binjia Zhou, Ming Li, Kai Li, Xin Wang, Zhenyang Li, Zesong Yang, Weikai Chen, Runze Zhang, Xin Wang, Yanwei Fu, Zhen Chen, Xiangru Huang  
**Data:** 2026-10-12  
**Categorie:** cs.CV, cs.AI  
**Link:** https://arxiv.org/abs/2610.16146v1

> We present Unravel, a training-free framework that turns a single image into an interactive 3D scene, where every object is an independent and movable asset. Existing generators either produce one entangled geometry in which no object can be moved, or predict all objects in one feed-forward pass, where a wrong guess cannot be detected or repaired. Unravel instead takes a different approach: it first takes the scene apart, and then puts it back together. Starting from the input image, an agentic harness that iteratively peels the image layer by layer, and adopts point cloud as major modality for spatial relationship recovery. Specifically, a vision-language model plans which objects are fully visible, an image editor removes them and restores the occluded regions. Every edit is verified before being incorporated into the reconstruction. This process gradually turns occluded parts of the scene into direct observation, allowing objects to be reconstructed when they are best exposed rather than hallucinated from the original image alone. The scene is then rebuilt in reverse removal order, so that the supporting objects are naturally placed before the objects they support. Since a single-view image only reveals part of an object, we treat the observed points as a lower bound on its size: an asset may grow to cover its points, but can not shrink away from them. Finally, we physically settle the reconstructed scene to remove floating objects and interpenetrations, followed by an agentic audit that corrects remaining placement errors. Extensive experiments on diverse indoor scenes show that Unravel recovers more objects, places them more faithfully, and produces scenes that are more physically-plausible than existing methods.

---

## 79. Computational Reflective Equilibrium for Agentic AI: A Rawlsian Alignment Scaffold for Governance

**Autori:** Quanyan Zhu  
**Data:** 2026-10-12  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.16015v1

> The rapid deployment of agentic AI has introduced complex challenges for the ethics and governance of AI systems. Agents built on large language models act through tools on behalf of people, and each deployment case brings its own instructions, policies, evidence, and stakeholders, so alignment must be formed case by case. To this end, this work proposes agentic reflective equilibrium (ARE), a computational reflective equilibrium framework that serves as an ethical alignment scaffold in the agent harness. Drawing inspiration from the reflective equilibrium of John Rawls, the scaffold links principles from the system prompt and operator policy, considered judgments, tool evidence, and candidate actions through typed support and attack relations, with provenance encoding the instruction hierarchy. The agent acts on an equilibrium of this state and calls tools or asks questions only while doing so is worth its cost, unless a due-diligence mandate requires them. Governance enters through value priorities, source authority, prohibitions, human-in-the-loop triggers, and mandates, and certificates attribute each action to the sources whose commitments drove it. We show that equilibria are Nash equilibria of a mutual-adjustment game and establish monotonicity, lexical priority, stability certificates, and a quarantine theorem for prompt injection. Two case studies illustrate the framework: a computer-use assistant told to win a refund "whatever it takes" files an honest warranty claim, refuses a fake review, and ignores an injected request for personal data; a hiring agent showcases how authority, oversight triggers, audit mandates, and hard prohibitions shape discrimination, privacy violations, and escalation. The framework offers traceability, coherence, and adaptivity, facilitating safe, secure, and trustworthy agentic AI.

---

## 80. MedHarnessBench: A Unified Benchmark for Healthcare Agent Evaluation

**Autori:** Rui Tang, Hongqiu Wang  
**Data:** 2026-10-11  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.15714v1

> Healthcare agents must transform longitudinal clinical evidence into reliable actions through heterogeneous tools and stateful workflows, conditions under which model-centric systems may lose context, misuse tools, fail to verify consequential transitions, or cross authorization boundaries. Existing medical-agent benchmarks primarily emphasize terminal task outcomes, making it difficult to determine whether execution failures arise from the agent model, the runtime harness, or their interaction. We present the Medical Harness Protocol, an outcome-preserving framework that independently evaluates seven healthcare-specific process dimensions: Care Action Fulfillment, Clinical Resource Competence, Patient-Evidence Alignment, Clinical Workflow Continuity, Clinical Auditability, Closed-Loop Verification, and Clinical Conduct Boundaries. A normalized intervention trace further tracks whether runtime support is available, activated, delivered, adopted by the agent, and propagated into subsequent behavior. We instantiate the protocol as MedHarnessBench, comprising 342 executable tasks across FHIR/EHR operations, healthcare-administration interfaces, and multimodal clinical tools. Across more than 16,000 controlled task executions, MedHarness yields broad improvements in terminal task success, intermediate subtask completion, and healthcare-specific process quality. We further evaluate MedHarness against multiple general-purpose harnesses and use controlled single-fault perturbations to verify the sensitivity and discrimination of the seven-dimensional evaluation. These results demonstrate that healthcare-specific runtime support can substantially improve both task completion and execution quality, while revealing failures that terminal outcomes alone cannot capture. Code and resources are available at https://github.com/Tomry1114/Awesome-Agent-Harness-for-Healthcare.

---

## 81. VideoEvoHarness: Self Evolving Agent Harness from Unlabeled Videos for Video Understanding

**Autori:** Weixin Xu, Yifan Liu, Yi Wang, Mingfei Rong, Zhenyu Yang, Zhisheng Zhong, Shengsheng Qian, Changsheng Xu  
**Data:** 2026-10-11  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2610.15389v1

> Video understanding agents rely on a harness to acquire evidence, use tools, and reason, but improving it requires substantial effort. Recent self evolution methods seek to optimize harnesses through execution feedback to reduce human intervention. However, existing methods often rely on annotated video questions and answers or focus on updating model parameters, leaving harness evolution from unlabeled videos underexplored. VideoEvoHarness jointly evolves a Questioner and a Solver harness from unlabeled videos with frozen model parameters. The Questioner constructs questions and computes reference answers directly from video memory records. Question quality assessments and Solver execution trajectories guide question generation policy revisions. The Solver supports evolving skills, strategies, hyperparameters, and tools using execution feedback. Executable strategies define workflows in code, reducing repeated interpretation of natural language instructions. Each round, candidate harnesses are compared on identical validation questions, with validated improvements retained for later use. Experiments on benchmarks and a dedicated benchmark question set, using videos disjoint from evolution videos, show higher overall accuracy than initially and transfer gains across backbones. Overall accuracy on this set also improves progressively across rounds. This supports our foundational framework for harness evolution from unlabeled videos, opening a promising direction for self evolving video agents. Code is available at https://github.com/Wei-Xin-Xu/VideoEvoHarness.

---

## 82. PANINI-DR: Controlled Deep Research through Generative Semantic Workspaces

**Autori:** M. Yigit Turali, Shreyas Rajesh, M. Efe Lorasdagi, Chenda Duan, Kartik Sharma, Vwani Roychowdhury  
**Data:** 2026-10-10  
**Categorie:** cs.CL, cs.AI, cs.IR  
**Link:** https://arxiv.org/abs/2610.15208v2

> Deep research requires connecting multiple steps of search, reasoning, and computation, with intermediate findings guiding what to investigate next. As investigations grow, agents must maintain research state across model calls and check findings before errors propagate into subsequent work. We introduce PANINI-DR, a multi-agent harness that separates coordination of the overall investigation from the research and verification of individual subquestions. A shared workspace, built on the Generative Semantic Workspace representation, records subquestions, their dependencies, findings, and supporting evidence. Researchers investigate individual subquestions, while a separate verification agent checks proposed answers against those subquestions and their evidence. Verification feedback guides further investigation, and recorded findings inform subsequent assignments. We evaluate PANINI-DR on BrowseComp-Plus, FRAMES, and MoNaCo against seven state-of-the-art deep-research harnesses, all using a shared language-model backbone and frozen corpora. PANINI-DR achieves the strongest average performance across the three benchmarks. On BrowseComp-Plus, it achieves 73.3% accuracy, outperforming the next-best harness by 16.0 points. Its advantage is strongest on hard questions, where it answers nearly twice as many as the next-best harness. Ablations further show that structured planning and persistent state improve performance, as does checking each finding against its cited evidence before it is reused. Because a model can answer correctly from memory alone, we also analyze the evidence retained by each harness. PANINI-DR achieves the highest answer recoverability from saved evidence on all three benchmarks, while complementary claim-support audits show stronger evidence-backed answers. Accounting for this evidence changes how harnesses compare and further strengthens PANINI-DR's advantage.

---

## 83. Harmony Harness: Multi-Objective Self-Evolution of Agent Harnesses

**Autori:** Weichen Yu, Lesly Miculicich, Bhavana Dalvi Mishra, Jiefeng Chen, Shuo Li, Matt Fredrikson, Tomas Pfister, Long T. Le  
**Data:** 2026-10-10  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.15150v1

> Recent work on self-evolving LLM agents treats the agent harness as an optimization target that can be iteratively improved through execution feedback. Existing approaches, however, largely optimize a single objective and evolve the harness as a monolithic artifact, limiting their ability to handle competing goals and to separate transferable design from environment-specific adaptation. We introduce Harmony Harness, a framework for multi-objective, compositional harness evolution. Harmony Harness formulates harness evolution as a multi-objective optimization problem and uses decomposition-based evolutionary search to maintain solutions across different regions of the Pareto frontier, avoiding reliance on a hand-designed structural diversity metric for repository-scale harnesses. In parallel, we introduce factorized evolution operators that separately refine general-purpose harness mechanisms and benchmark-specific adaptations, together with a dynamic composition workflow that integrates them at inference time. Across SecRepoBench and BaxBench, Harmony Harness consistently outperforms strong harness-evolution baselines, with gains exceeding 10% on both benchmarks. Our results show that explicitly modeling both objective trade-offs and harness structure yields substantially stronger and more transferable agent evolution than existing single-objective, monolithic approaches.

---

## 84. Getting Space Right: Agentic Rewards for Image Generation

**Autori:** Xiaofeng Tan, Jiaxin Lin, Haobo Yuan, Tiancheng Shen, Zihan Su, Rui Chen, Hongsong Wang, Ming-Hsuan Yang  
**Data:** 2026-10-10  
**Categorie:** cs.CV, cs.AI  
**Link:** https://arxiv.org/abs/2610.14852v1

> Reinforcement learning (RL) is promising for spatial text-to-image generation, but existing work largely focuses on policy optimization, assuming accurate rewards and effective online rollouts. We observe in-domain gains with out-of-domain degradation, exposing two limitations: unreliable spatial rewards in open-world settings and rollouts lacking basic-to-complex progression. We propose a curriculum-guided RL framework. First, we introduce SpatialCritic, an agentic reward model equipped with a spatial perception harness that combines reusable verification guidance with specialized vision tools. We then construct spatial preference datasets through targeted counterfactual perturbations and perform agent-harness alignment to improve tool selection and evidence integration efficiently. Second, curriculum learning organizes shared foundational capabilities and their compositional dependencies in a capability graph for mastery-guided rollouts, periodic review, and targeted remediation. On SpaRW-Eval, SpatialCritic achieves 95.1% verification accuracy, outperforming 320B GLM-5.3-Flash with a 40x smaller 8B backbone and raising average baseline scores from 78.4 to 83.9 on SD3.5-Medium and 83.2 to 86.5 on BAGEL. Project page: https://xiaofeng-tan.github.io/projects/spatialcritic/

---

## 85. Reels-RSI: Program-Level Self-Improvement for Code-Rendered Explainer Videos

**Autori:** Wei Lin  
**Data:** 2026-10-10  
**Categorie:** cs.AI, cs.GR, cs.MM, cs.SE  
**Link:** https://arxiv.org/abs/2610.14495v1

> Explainer videos -- a worked geometry problem, why the sky is blue, how a dynasty fell -- are usually one more target for pixel video generation. We argue they are a different kind of artifact: a program (script, storyboard and per-frame animation code) that a deterministic renderer turns into frames. A program can be read, diffed, tested and audited; pixels can only be watched. Reels-RSI is an open-source reel director for any agent harness; its self-improvement happens at the program level rather than in weights or prompts. Every revision pass is logged with a code snapshot; a retrospective pairs each check finding with the diff that fixed it and proposes lessons; a lesson that a static check can catch is compiled into a rule with a must-fail and a must-pass example, so the memory is unit-tested; and a rule learned today runs over everything made before it. A bounded, benchmark-gated step lets an agent rewrite the director's playbook, kept only when blind pairwise judgments on held-out topics prefer it; nothing enters memory without a human decision. Across 111 reels -- a field study, two playbook evolutions, a 2x2 memory ablation, a weaker director, a 48-reel learning curve and a judge-reliability study -- we find that the rule learned in the field caught four latent defects in frames authored before it existed and none after; that rules are an audit for a strong director (eight unguarded reels, no violation) and a guard for a weaker one (thirty violations unguarded versus five); that lessons shorten revision loops but do not compound or move the judge; and that the first rewrite's 11--1 verdict was a position bias in our vote design (judges pick the second-shown reel 62--81% of the time), masking scripts that traded thirteen facts for craft. We document four failure modes of the preference signal, which check caught each, and the fixes. Code, rules, lessons and data are public.

---

## 86. Frustratingly Easy Agentic RAG via Portable Skills: A Case Study in Customer Support

**Autori:** Istok Bako, Bonan Min, Tiffany Shao, Claire Cheng, Yashar Mehdad  
**Data:** 2026-10-10  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.14428v1

> Enterprise workflow automation typically requires retrieving a complete and accurate set of relevant information from large operational document corpora (SOPs, policy documents) given a specific scenario or request. In customer support (CS), for example, human specialists must determine the correct sequence of resolution steps for each case, a task that demands precise grounding in policy documentation. Meeting this bar in production typically requires complex document chunking, indexing, and retrieval pipelines, often layered with learned re-rankers, query rewriters, and bespoke agentic RAG infrastructure. We report a deployment case study of a simpler alternative: a portable skill consisting of a natural-language instruction, lightweight tools (a retrieval API, format-checking scripts), and a corpus enriched with an LLM-generated navigation layer, which is a structured "Wikipedia-style" index over the underlying documents. This agentic RAG approach is straightforward to implement (1-2 engineer days), portable across capable agentic harnesses (e.g., Claude Code), and performs strongly on the challenging task of CS resolution workflow generation, achieving 99.2% procedural equivalence to human-approved ground truth and 83.3% evidence sufficiency. It is also roughly an order of magnitude slower per case than our deployed production assistant (~90 s vs. ~8-9 s), so we claim no latency advantage. Our claim is scoped to that setting: a mature, well-curated corpus, a latency-tolerant workflow, and human review of every case. There, the skill did the work of a complex RAG stack, and maintenance became a matter of editing text and data rather than retraining models.

---

## 87. Harness^2: Recursive Agent Harnessing for an Open World

**Autori:** Ruiyao Xu, Yanfei Chen, Zhongying CuiZhu, Bhavana Dalvi Mishra, Yifei Ming, Han Yu, Rujun Han, Chen-Yu Lee, Tomas Pfister  
**Data:** 2026-10-09  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2610.14224v1

> LLM agents' capabilities depend not only on their underlying models but also on their execution harnesses. Recursive self-improvement (RSI) offers a promising approach to automatically evolve these harnesses. However, deploying RSI in open-world settings still faces two critical challenges. First, open-world tasks are typically unseen during the harness design phase and novel at test time, leaving no ground-truth verifiers to reliably guide online harness edits. Second, the RSI process remains highly task-specific and fails to generalize to novel scenarios. We introduce Harness^2, a plug-and-play, recursive agent harnessing framework that addresses these challenges through two connected levels of recursion. Task-level recursion refines the current task's harness using a contrastive Propose-Probe-Compose step that reliably guides edits without ground-truth verifiers, and can be scaled further via parallel or sequential recursion. Harnessing-level recursion then extracts experience from these edits to update a continual improvement harness, enabling the agent to better adapt to future tasks. Across three professional benchmarks and four model-harness configurations, a single step consistently improves GLM-5 and Gemini 3.5 Flash over their base harnesses, yielding gains of up to 11.5 points on WorkBuddy-Bench, 4.5 points on JobBench, and 11.8 percentage points on LAB, with further gains as the task-level recursion budget increases.

---

## 88. Cortex: Measurement-Gated Evolution and Pruning of Coding-Agent Skills and Rules

**Autori:** Samuele Giampieri  
**Data:** 2026-10-09  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2610.14216v1

> Coding agents such as Claude Code also follow text files that developers write for them: a project file, skills the agent may choose to open, and rules that load automatically when the agent reads matching files. We call these files the agent's harness. Developers add to it whenever they correct the agent, but one success proves little: the same agent can pass a task once and fail it the next time. We present Cortex, a tool that tests changes to the harness instead of trusting them. It saves fixes from the developer's sessions as replayable tasks, finds the corrections that recur, writes one skill or rule at a time, and keeps it only if repeated runs with and without it show a net gain and no task made noticeably worse. Existing text is tested the same way before it is deleted, and Cortex neither adds nor deletes text the agent never used. We tested Cortex with Claude Haiku 4.5 on a repository built for the purpose, with conventions the model tends to break, one area with nothing to learn, and a script playing the developer. On held-out tasks, the harnesses it built made the agent follow the conventions far more often than no skills or rules did, left the comparison area unchanged, and added no text read on every turn. Rules, which load automatically, did most of the work; skills helped only when offered with the files a task touches, and those offered on every turn were rarely opened. Cortex kept none of the useless or harmful suggestions we planted, but the agent never opened the useless ones or the harmful skills, and it reached no verdict on the harmful rules, so the test shows that Cortex keeps no unused text, not that it detects damage. Under the stronger Claude Sonnet 5 a single run's harness added little, and on a real open-source project, where the agent was rarely corrected, Cortex found nothing to learn. We release the tool, the lab and its data.

---

## 89. The Silent Failures in Agentic Data Science

**Autori:** Xue Li, Hongqian Xia, Daniel Gomm, Aécio Santos, Cornelius Wolff, Madelon Hulsebos  
**Data:** 2026-10-09  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.14115v1

> Large language models have significantly lowered the barrier to writing code. Naturally, this has also led to the development of data science agents that promise automating the design and execution of data science from task formulation to model development. Existing evaluations of agentic data science (agentic DS) assess downstream predictive performance and code correctness, providing preliminary insight in agentic DS capabilities. We argue that these evaluations overlook the fundamental principles of data science: methodological data science- and domain knowledge. As such, only assessing downstream performance masks methodological failures such as data leakage and inappropriate validation, limiting the development of robust agentic DS systems. In this paper, we evaluate agentic DS beyond accuracy from three different angles: 1) a large-scale analysis of failure modes in common agentic DS frameworks and models across 220 data science tasks, 2) a reusable and extensible test suite with curated data science tasks that test for six specific failures in a controlled manner, and 3) a qualitative assessment of agentic DS pipelines against expert solutions on Kaggle competitions. We find that the majority of agentic solutions contain at least one failure mode despite the complexity of agentic harness or model capacity. Moreover, we identify a positive correlation between the occurrence of data leakage failures and predictive performance, confirming the necessity to evaluate agents beyond accuracy. Our qualitative analysis shows that DS agents generally lack problem solving creativity and domain knowledge, compared to competition-winning data scientists. We believe that principled failure mode analysis, as presented here, should be integral part of agentic DS evaluations, and that the insights we surface will be key in developing trustworthy agentic DS pipelines.

---

## 90. LongHarness: Advancing Agentic Reasoning over 100M-Token Corpora via Stateful Evidence Management

**Autori:** Songtao Huang, Zhijie Zhong, Xiaohan He, Shuaiyu Zhang, Zhiyin Yu, Li Kang, Heng Zhou, Yutao Fan, Xiangchao Yan, Bo Zhang, Shiyang Feng  
**Data:** 2026-10-09  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.13075v1

> Corpus-level long-context reasoning requires agents to acquire and integrate evidence across document collections that exceed their context windows. Existing agent harnesses enable incremental access to these corpora, but acquired evidence and evolving conclusions often remain entangled in a growing interaction history. This implicit state management can lead to two coupled failure modes: unbounded exploration, where retrieval expands the interaction history without resolving decision-relevant information gaps, and evidence-state drift, where previously acquired evidence or subsequent corrections fail to inform the current conclusion. We present LongHarness, a model-agnostic harness that makes the interaction between acquired evidence and evolving conclusions explicit. Its core mechanism, Evidence-Conclusion Coevolution, uses unresolved conclusions to guide exploration toward missing information, while newly acquired evidence strengthens or revises the conclusions that directed the search. LongHarness couples this process with Evidence Lifecycle Management, which keeps accumulated evidence current and traceable throughout the interaction. Together, these mechanisms focus retrieval on remaining information needs and keep conclusions aligned with current evidence. We evaluate LongHarness on OfficeQA Pro V1 and V2, AA-LCR, and LongBench v2 using GLM-5.3-Flash and Qwen3.8-Flash. Compared with direct reasoning using the same backbone, LongHarness improves GLM-5.3-Flash exact match on OfficeQA Pro from 15.8% to 60.2% on V1 and from 4.4% to 61.1% on V2. Against state-of-the-art agent harnesses, it surpasses Claude Code by 12.0 percentage points on V1 and Codex by 18.9 points on V2. With Qwen3.8-Flash, LongHarness reaches 61.7% on V1, outperforming Claude Code by 8.3 points and Codex by 12.0 points.

---

## 91. Evo$^2$: Evolving the Evolver through Weight-Harness Co-Evolution

**Autori:** Chejian Xu, Shujian Zhang, Wenxuan Zhou, John Lambert, Beck Chen, Bo Li, Andrew Hard, Rajiv Mathews  
**Data:** 2026-10-09  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2610.13025v1

> Self-evolving agents are increasingly used to improve language model systems without human intervention through either weight updates or harness improvements. Existing approaches typically pursue these directions separately: some methods update model weights using self-generated experience, while others rewrite the harness that defines how an agent uses prompts, tools, context, and execution feedback. However, these approaches overlook the relationship between model weights and the agent harness. To connect these processes and ensure effective and smooth agent self-evolving, we propose Evo$^2$, a framework for weight-harness co-evolution. For harness updates, we design a unified dual-role pipeline that a single policy serves as both a Proposer, which writes harness edits, and a Reflector, which diagnoses their effects and guides revision. For weight updates, harness modifications and their execution outcomes guide the training of both the Proposer and the Reflector. We further develop EvoTIDE, a training pipeline that recovers usable trajectories through edit extraction and prefix continuation, then combines SFT with interleaved GRPO across the two roles. Extensive experiments across three coding benchmarks demonstrate that Evo$^2$ significantly outperforms existing self-evolution methods. It achieves 82.1% on Polyglot and 48.3% on SWE-bench Verified, compared with 62.6% and 41.0% for the strongest baseline, respectively. We also show that the evolved harnesses transfer to different tasks without further evolution and rank first in cross-benchmark evaluations. Our dual-role harness improvement framework is also able to extend to self-evolution with proprietary models, improving a GPT-5-mini agent's performance from 24.4% to 48.3%. These results demonstrate the applicability of the framework Evo$^2$ across domains and its broad transferability across models and tasks.

---

## 92. Don't Guess, Just Ask: Evaluating Interactive Requirement Clarification for Repository-Level Software Development

**Autori:** Mingyu Chen, Zhiqing Zhong, Manyi Wang, Linxi Liang, Rouyu Chen, Pinjia He  
**Data:** 2026-10-09  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2610.13022v1

> As LLMs become increasingly capable of implementing software, a critical bottleneck emerges: whether they truly understand what users want. Users often begin with vague intent, leaving important requirements to be clarified through interaction. In repository-level development, misunderstandings can propagate and cause costly rework. However, existing benchmarks typically evaluate implementation from complete specifications or underspecified requests, overlooking pre-coding requirement clarification. Prior clarification studies mainly focus on function-level tasks. It therefore remains unclear how well LLMs can transform vague intent into clear requirements through interaction and how this capability affects subsequent code generation. We introduce ReqClarifyBench, an interactive requirement clarification benchmark for repository-level software development. It contains 341 tasks spanning game, miniapp, and web development, each with a vague user intent, a human-validated requirement document, and code evaluation artifacts. We employ LLM-based user simulators with diverse personas derived from real-world conversations. We evaluate six LLMs in terms of clarification effectiveness and generated requirement document quality. Results show that stronger clarification effectiveness does not necessarily translate into higher document quality, and performance varies substantially across user personas. We also find that coding-agent harnesses do not further improve requirement document quality compared with their base LLMs. These findings offer insights for building LLM-based end-to-end software development systems.

---

## 93. EmbodiedCLBench: Evaluating Continual Learning for Self-Evolving Embodied Agents

**Autori:** Jie Huang, Yanan Chen, Ruixun Liu, Kaichen He, Xinyi He, Rui Huang, Zilong Zheng, Zhenliang Zhang, Yiwu Zhong  
**Data:** 2026-10-09  
**Categorie:** cs.AI, cs.CL, cs.CV  
**Link:** https://arxiv.org/abs/2610.13021v1

> Continual learning requires models to accumulate past experience and transfer it to new tasks. Despite substantial research on continual learning, existing work remains largely confined to non-embodied settings, without extending to embodied environments. To address this gap, we introduce EmbodiedCLBench, the first benchmark in embodied simulation for evaluating the continual learning capability of self-evolving agents. With compositional generalization as the core evaluation principle, our benchmark evaluates whether agents can first learn from basic tasks and then recombine the acquired skills to solve complex, unseen advanced tasks. Based on EmbodiedCLBench, we conduct extensive experiments across multiple agent harnesses and learning methods, revealing consistent limitations and distinctive behaviors. Our results show that while advanced tasks can be hardly solved under zero-shot setting, the experience from basic tasks enables consistent improvement. Such benefit from the experience remains stable even if the task complexity increases. However, this improvement does not scale accordingly with the number of learning samples, and current agents cannot extract meaningful information from additional experience. Collectively, our findings highlight continual learning as a fundamental yet underexplored capability, and our benchmark offers valuable resources for designing effective self-evolving agents in embodied environments. Our code and dataset are available at https://pku-value-lab.github.io/EmbodiedCLBench-homepage.

---

## 94. Compaction-Aware Reinforcement Learning For Ascend Triton Kernel Generation

**Autori:** Chuansai Zhou, Yanlin Liu, Bingning Huang, Shidi Xi, Chao Huang, Boxing Chen, Mingming Zhu, Guanghuan Fang, Ben Feng, Zongzuo Wang  
**Data:** 2026-10-09  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2610.23950v1

> Automatically generating high-performance kernels with LLM-based agents promises substantial gains in development efficiency, but two obstacles remain. First, while increasing multi-turn interaction with execution environments is crucial for refining generation quality, continuous context accumulation rapidly exceeds the model's effective context window. Second, training long-horizon tasks via GRPO inherently incurs sparse rewards due to its reliance on terminal outcome evaluation, severely hindering step-level credit assignment; To address these obstacles, we propose ATRL (Ascend Triton Reinforcement Learning), a post-training method that refines GRPO into a compaction-aware, segment-level objective for long-horizon kernel generation. We also design a lightweight agent harness providing cascaded compilation, correctness, and profiling feedback, alongside an Ascend-specific knowledge base injected during agentic RL training and evaluation to compensate for the base model's missing platform expertise. Evaluations on NPUKernelBench and KernelBench, both executed on Ascend hardware, show that ATRL consistently surpasses all baselines, including GRPO, in both correctness and speedup.

---

## 95. Recurrent Harness for Agentic Continual Learning

**Autori:** Yuxin Xiao, Zhiyun Lu, Jianyu Wang, Yangtian Zhang, Yang Song, Qifan Wang, Bailin Wang  
**Data:** 2026-10-08  
**Categorie:** cs.LG, cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2610.12668v1

> Language model agents increasingly operate over long interaction streams, requiring online adaptation to distribution shifts through continual learning. However, existing agent harnesses typically either evolve their states only through forward information flow or rely on additional replay or validation data for harness optimization. To address this, we propose ReHarness, a recurrent harness framework for agentic continual learning that complements forward read and write with backward revision under a strictly online streaming protocol. We ask what information could have been captured differently in the harness state to better inform the current instance in the stream. Specifically, after each instance, we leverage the resulting trajectory as feedback to revise the reflections retrieved for that instance, thereby propagating feedback backward through the textual harness state. Across three continual learning benchmarks and three language model backbones, ReHarness consistently outperforms strong raw-context baselines, memory- and reflection-based methods, and prompt optimization approaches. Further analysis shows that ReHarness produces source-grounded and meaningful revisions, corrects overgeneralized or outdated experience under distribution shifts, and improves both stability and plasticity during continual learning.

---

## 96. Embodied Turing Machines: Stateful Code for Robot Recursive Self-Improvement

**Autori:** Kairui Hu, Siyuan Hu, Fangzhou Hong, Zhaoxi Chen, Ziwei Liu  
**Data:** 2026-10-08  
**Categorie:** cs.RO, cs.CV  
**Link:** https://arxiv.org/abs/2610.12369v1

> Most robot policies keep a model in the control loop: a VLA maps observations to actions, and an Agent Harness, such as Agent-as-Policy or Harness VLA queries a VLM for decision making at run time. We propose a different view: the embodied world is an Embodied Turing Machine, whose tape is the robot and environment state and rules are the policy. If this state can be represented accurately, the decision making can be written entirely in code. We therefore propose Code-Only-as-Policy (COAP): code measures and tracks the robot, environment, and task state from camera images and proprioception, and makes every decision from it. The same code applies across episodes, and different tasks share one library without a VLM or VLA in the loop. Compared with VLAs and Agent Harnesses, we analyze three advantages of COAP: (i) Explicit State: the state can be stored in code; (ii) Execution: code makes decision making controllable, recovers from failures flexibly, and runs fast and cheaply online; (iii) Extensibility: new tasks reuse, inherit, or extend the shared library, so capabilities can accumulate over tasks. These advantages make COAP a suitable medium for recursive self-improvement (RSI): coding agents develop the library in a closed loop, and each change is explicit and controllable. On RoboDojo's 42 bimanual tasks, the resulting library reaches a success rate of 70.24% without a model at test time. The upper bound of COAP lies in how accurately the state is represented for decision making and how robust the code logic is. We thus propose COAP as a new paradigm for embodied tasks; since it applies across episodes, it can also serve as an efficient data engine for VLAs and Agent Harnesses.

---

## 97. Accurate but Not Humble: Evaluating Epistemic Humility in LLM Agents under Knowledge Conflict

**Autori:** Kaiser Sun, Bernal Jimenez Gutierrez, Hongjun Liu, Jingyu Zhang, Jie Gao, Mark Dredze, Daniel Khashabi  
**Data:** 2026-10-08  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2610.12360v1

> When retrieved evidence contradicts an agent's prior beliefs, does it revise its answer, acknowledge uncertainty, or persist with an incorrect conclusion? Existing evaluations of agentic systems focus primarily on task success, offering limited insight into how agents handle such conflicts. We propose to evaluate agents on epistemic humility (EH): the agent's willingness to recognize, act on, and communicate uncertainty during task execution. We operationalize EH through three trajectory-level behavioral dimensions: Identify, Solve, and Escalate (ISE). Through knowledge conflict, situations where the backbone language model's parametric knowledge contradicts the evidence it encounters, or where two contextual sources disagree, we evaluate two conflict settings: (1) controlled conflict and (2) naturally occurring conflict during multi-step agentic execution, each paired with matched no-conflict controls. Evaluating four agents, we find that higher task accuracy does not necessarily correspond to greater epistemic humility: some high-accuracy configurations recognize conflicts during execution but do not communicate unresolved uncertainty in their incorrect final answers. Trajectory-level analysis further reveals that agents frequently detect conflicts in early steps of execution but fail to maintain or resolve them in later steps. Finally, we show that model-level interventions can improve EH, but often at the cost of task accuracy, suggesting that epistemic humility emerges from the interaction among the backbone model, agent harness, and evaluation environment.

---

## 98. A Closer Look at Agentic BBO: Benchmarking LLM Agents for Black-Box Optimization

**Autori:** Ming Chen, Rong-Xi Tan, Ke Xue, Yu-Jie Zhou, Taiye Lu, Zhi-Xuan Gao, Peng Xie, Zijun Shen, Chen Lu, Haopu Shang, Chao Qian  
**Data:** 2026-10-08  
**Categorie:** cs.LG, cs.AI, cs.NE  
**Link:** https://arxiv.org/abs/2610.12183v1

> Black-box optimization (BBO) arises in many scientific and engineering problems where objective evaluations are expensive and limited. Recent large language model (LLM) agents offer a new way to approach BBO by combining task semantics, computation, optimization tools, and feedback-driven decision making, showing great potential due to the integration with mathematically rigorous tools. However, existing agentic BBO studies use different task domains and system configurations, making their results difficult to compare and the effects of individual design choices hard to isolate. We therefore introduce AgenticBBO-Bench, a cross-domain benchmark for agentic BBO spanning synthetic functions, hyperparameter optimization, database tuning, chip design, and molecular design under a unified finite-budget evaluation protocol. In our experiments, agentic BBO achieves higher family-averaged scores than direct LLM-based methods in all five domains and outperforms the best numerical optimizers in four. We further study three factors shaping agent performance: optimization tools, task information and prior knowledge, and the role of the LLM during search. Our results show that additional numerical tools do not consistently improve performance, task semantics are broadly useful while more specific priors are less reliable, and numerical optimizers can effectively absorb gains from search trajectories established by the agent. Finally, we introduce a five-task frontier challenge within AgenticBBO-Bench and evaluate seven LLMs under the Codex agent harness, where GPT-6 Astra and DeepSeek-V4.1-Flash lie on the Pareto frontier of performance and cost among the evaluated models. Our code is available at https://github.com/lamda-bbo/agentic-bbo.

---

## 99. SuperNav: An Agentic Navigation System for Any Task in Any Scene

**Autori:** Jinkai Zhang, Jingyi Xu, Yuanhong Yu, Jiarui Guo, Ruizhen Hu, Hujun Bao, Xiaowei Zhou, Sida Peng  
**Data:** 2026-10-08  
**Categorie:** cs.RO, cs.CV  
**Link:** https://arxiv.org/abs/2610.12126v1

> General-purpose service robots need navigation systems that can handle diverse human requests in unfamiliar environments, combining task generality with scene generality. Some existing methods fine-tune multimodal large language models (MLLMs) to predict navigation actions, making their behavior dependent on the coverage of navigation training data and potentially limiting generalization to new requests and environments. Our key insight is to let the MLLM focus on interpreting requests, understanding scenes, and making decisions while preserving its general-purpose capabilities and delegating motion execution to navigation tools. To realize this idea, we introduce SuperNav, which equips a pretrained MLLM with a specialized agent harness without navigation-specific fine-tuning of the MLLM. Our harness supports these decisions with Navigation Skills, agent-oriented Tools for physical interaction, and task-progress and context management. A unified visual-point interface connects decision-making to motion by allowing the model to specify destinations directly in images and revise its decisions from execution feedback. Together, these components support sustained navigation across different task requirements and environments. SuperNav outperforms four evaluated baselines on instance-level, multi-object, and demand-driven tasks. Category-level evaluation on HM3D and deployment on a real quadruped robot further demonstrate its applicability across environments. Project Page: https://zju3dv.github.io/SuperNav/

---

## 100. EvoAlloc: A Self-Evolving Resource Allocation Agent for Efficient Program Evolution

**Autori:** Yanning Dai, Yuhui Wang, Nanbo Li, Wenyi Wang, Jürgen Schmidhuber  
**Data:** 2026-10-08  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.12086v1

> LLM-based program evolution relies on evaluation feedback to guide the iterative search for high-performing programs. However, evaluation is often computationally expensive, making it essential to allocate limited resources to candidates that can most effectively advance the search. Existing LLM-based methods typically rely on fixed allocation strategies throughout the search, potentially wasting resources on low-value candidates while overlooking promising ones. We propose EvoAlloc, a self-evolving resource-allocation agent that learns from search experience to revise its strategy for allocating computational resources across candidates. EvoAlloc periodically consolidates prior search and allocation outcomes into reusable experience, which informs subsequent strategy revisions. It further uses a counterfactual exploration mechanism to occasionally evaluate candidates denied resources by the allocator, revealing their outcomes to enrich its experience for future strategy updates. Across coding and agent-harness optimization benchmarks, EvoAlloc requires 59-82% fewer full evaluations and 61-89% fewer total LLM tokens to reach baseline-level performance. Moreover, under the same full-evaluation budget, EvoAlloc achieves 8.7-12.0% higher final performance.

---

## 101. MiMo-V2.6: Scaling Reinforcement Learning Towards Self-Improvement

**Autori:** Xiaomi LLM-Core Team, :, Zongming Qiao, Ziyue Hua, Zirui Ou, Zihao Yue, Zihan Jiang, Zhuo Huang, Zhiyang Chen, Zhixian Zheng, Zhipeng Xu, Zhengrui Ma, Yuyang Hu, Yuhang Dong, Yuechen Zhang, Yudong Wang, Yuanxin Liu, Yixin Yang, Yishuo Cai, Yikai Zhao, Yihan Yan, Yifan Zhang, Yifan Song, Xiyu Wei, Xing Zhang, Xin Zhang, Xiaoqian Liu, Xiaodong Ji, Xiangwei Deng, Xueyu Guo, Wenhan Ma, Weimin Xiong, Weikun Wang, Weiji Zhuang, Shuo Liu, Shuhuai Ren, Shuhao Gu, Shimao Chen, Shijie Cao, Shihua Yu, Shicheng Li, Shengjie Zhou, Shaolei Zhang, Rang Li, Qiying Wang, Qingkai Fang, Qianli Chen, Minzheng Wang, Liwen Wang, Linli Yao, Linghao Zhang, Liangyu Cheng, Liang Zhao, Lei Li, Jinhao Dong, Jinyu Xiang, Jianyu Wei, Jiangshan Duo, Huaqiu Liu, Huanjie Fan, Hongyi Guan, Hongshen Xu, Hao Tian, Hanyu Li, Hailin Zhang, Gang Wang, Fuli Luo, Feng Wei, Dong Zhang, Dawei Zhu, Chiheng Lou, Chenhong He, Chenhao He, Chenghua Liu, Bowen Ye, Bowen Shen, Boshen Xu, Bo Yang, Bingquan Xia, Bangjun Xiao, Baixuan Xu, Zhouxiang Mao, Zhiyang Zhang, Zhixiang Xu, Zhenru Lin, Zhengju Tang, Zhaojun Huang, Yuzhe Weng, Yuxing Xiang, Yuxiao Li, Yuheng Yang, Yuhang Wang, Yuchen Liu, Yuanyuan Tian, Yuanliang Dong, Yu Cheng, Yongzhe He, Yongshun Liang, Yong Wang, Yiyan Wang, Yitian Gong, Yijie Zhang, Yanshu Xin, Xun Zhang, Xingjian Zhao, Wenyu Yang, Wenshan Huang, Wenhao Li, Tingwei Huang, Tianyu Yu, Tianyang Lu, Taoyu Yang, Sinan Du, Shutong Tian, Shulin Du, Shengfan Wang, Shanchuan Fang, Qihao Zhang, Qibin Yang, Qian Yu, Qian Tu, Pengrong Xie, Peipei Wang, Peidian Li, Minkun Guo, Mingchen Shao, Luohan Gao, Lijie Wang, Liang Shi, Kaiqi Chen, Kaiming Liu, Kaifei Wang, Kai Yang, Jinlong Xue, Jiechen Zhang, Jiaxuan Liu, Hongxu An, Hao Peng, Hanglong Lü, Guonan Wang, Feiyu Yang, Fanyu Cao, Fangyue Liu, Fan Cui, Cong Wang, Chun Chen, Chenxu Bai, Chengxuan Zhu, Chenghua Wang, Boyi Zeng  
**Data:** 2026-10-08  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2610.11959v1

> Reinforcement learning (RL) is the central training paradigm for advancing large foundation models towards self-improvement. This report introduces the MiMo-V2.6 series, an omni-modal family that pushes the frontier of model intelligence by scaling RL compute. Prior to RL, we conduct mid-training on a broad multimodal corpus to provide ample exploration space, and build a solid infrastructure on the pretrained hybrid-SWA architecture to support subsequent scale-up. We scale RL compute along three dimensions: (1) larger batches and higher throughput, with an asynchronous training that consumes 1,568 samples and 2.7-3.7B tokens per step at context lengths of up to 1M; (2) more diverse and complex environments, spanning code, general, visual, and cyber domains under a mixture of agent harnesses; and (3) more grader compute, via groupwise agentic grading that yields more accurate reward signals for long-horizon tasks and steers the model towards shorter, more token-efficient solutions. To keep training stable at scale, we freeze the MoE router and establish a multi-layer defense against reward hacking. We further build infrastructure for mixed-task agentic RL, including a unified trajectory representation, high-concurrency multi-framework rollout, decoupled control and data planes, and training-inference consistency. We open-source the training dynamics, RL environments, and RL framework to facilitate reproduction and further research on scaled RL and model self-improvement.

---

## 102. Safe, Persistent, and Evolving Agent Harness for Understanding Partially Observable Worlds

**Autori:** Yisen Gao, Yue Guo, Qing Zong, Yiwen Guo, Yangqiu Song  
**Data:** 2026-10-08  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.11552v1

> Large language model agents can invoke tools fluently, but enterprise workflows demand more than selecting the right tools: actions must strictly comply with organizational policies, tool feedback often conceals hidden side effects under partial observability, and long-horizon tasks require persistent state tracking across multiple records. To address these challenges, we introduce E-Ledger, a multi-agent harness for safe and persistent execution. E-Ledger employs a code approval layer that checks every proposed action against policy before execution, and maintains a world ledger of verified hidden rules alongside evidence-backed dynamic state. Because hidden rules are typically unknown a priori, we further propose WorldAbduct, an abductive, world-model-driven harness evolution framework. WorldAbduct diagnoses execution trajectories across four complementary views (state consistency, world-observation gap, policy-gate correctness, and goal judgment) to hypothesize latent rules, and verifies them through targeted abductive interactions before integrating them into the ledger. On the enterprise benchmark World of Workflows, E-Ledger with WorldAbduct improves safe task completion across four LLM backbones, outperforming the strongest evolution baseline by 5--15 percentage points. Experiments in ScienceWorld and DiscoveryWorld further show that abductive harness evolution carries over to scientific environments. Our code is available at https://github.com/HKUST-KnowComp/E-LEDGER-WorldAbduct.

---

## 103. When Interfaces Speak: Data-Aware Generative UI Harness for Active Interaction

**Autori:** Xiaolong Li, Xiaohan Xu, Jinyang Li, Xinnuo Xu, Ge Qu, Nan Huo, Jack Williams, Reynold Cheng  
**Data:** 2026-10-08  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.11123v1

> Most human-agent interaction today remains text-based. Natural language can impose cognitive overload, ambiguity, information chaos, and slow input for complex tasks; ephemeral generative UIs can present structured information and guide users toward task completion. We propose GenUI-Harness, a multi-agent harness pairing a Tool Agent for information retrieval and task execution with a GUI Coder Agent that identifies ambiguities and generates front-end code for structured interfaces. Training the coder with reinforcement learning is challenging: verifiable rewards for interactive UI generation require costly execution, while LLM-as-a-Judge rewards are prone to reward hacking. We address the first challenge with Dynamic UX, a lightweight package for dynamic interaction and reward collection in a single sandbox, and the second with Reward Auditor, a meta-reward mechanism that monitors reward distributions and distills diagnostic patterns into a shared rubric and scoring specification. We introduce UI-TAU Bench, a benchmark for active human-agent interaction through generated UI code, built on 10 real-world domain databases constructed from public data sources and based on Tau-Bench tool-use settings, with Lite (300 tasks) and Full (1,000 tasks) splits. GenUI-Harness achieves an average Pass@3 gain of 4.48 percentage points over smolagents on Lite. Training with GenUI-Harness improves a 4B backbone from 9.33% to 58.00% Pass@3, outperforming larger frontier models such as Claude Opus 5 (46.67%). GenUI-Harness also remains robust on ambiguous and non-ambiguous queries. In a reviewer survey comparing communication channels, generated UIs reduce average dialogue rounds from 3.4 to 1.2. These results show that data-aware generative interfaces can support effective task completion and reduce dialogue rounds in evaluated database-backed workflows.

---

## 104. AgentHorizon: Evaluating Agentic Judges for Long-Horizon Computer-Use Tasks

**Autori:** Xing Han Lù, Dheeraj Vattikonda, Sina Hajimiri, Fatemeh Pesaran Zadeh, Parishad BehnamGhader, Ghazwa Darwiche, Amirhossein Kazemnejad, Christopher Pal, Alexandre Drouin, Siva Reddy  
**Data:** 2026-10-08  
**Categorie:** cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2610.11050v1

> Computer-use agents are capable of completing complex tasks, increasing the use of automatic judges to determine success, either for training or for evaluation without human involvement. Despite their flexibility, their reliability on long tasks spanning multiple applications remains unclear. A trajectory, composed of long sequences of screenshots and actions, may appear complete, but in reality violates constraints from the instruction or introduces an unwanted side effect. To identify these errors, a judge needs to examine the trajectory with respect to the user's instruction. To this end, we introduce AgentHorizon, a benchmark of 1,373 computer-use tasks (instruction-trajectory pairs) drawn from 166 hours of human-recorded trajectories spanning three operating systems. By recording trajectories for closely related instructions, we can construct negative tasks by swapping the instructions. This paired design evaluates judges on their ability to distinguish a successful trajectory from one that completed a similar (but incompatible) request. We release the benchmark under three splits: a frontier split, AgentHorizon (AH), a simplified split, AgentHorizon-Simple (AH-S), and a development split, AgentHorizon-Development (AH-D). We further evaluate eleven judges by (1) directly passing the full trajectory (with up to 300 screenshots and actions), and (2) using them as coding agents across five agent harnesses. We find that our best agentic judge, GPT-5.5, achieves 80.9% balanced accuracy on the AH subset. We find that tool-use improves certain models but results in worse performance for open-weight models, and that judges differ drastically in their ability to accept a valid trajectory and reject failed ones. Our findings highlight the need for judges that are capable of locating and verifying often hidden evidence that a task was properly completed inside long interaction histories.

---

## 105. EmbodiedRSI: Active Continual Robot Learning Through Hypothesis-Guided Co-Evolution

**Autori:** Python Song, Zhixuan Liang, Kelsey Fu, Mengdi Wang, Junfeng Yang, Shilong Liu  
**Data:** 2026-10-07  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.10498v1

> Robot foundation models provide strong visuomotor control, yet their performance can degrade when object positions or task instructions change. Further improvements often require post-training on substantial robot data, which can be costly to collect through methods such as teleoperation. Agentic harnesses can adapt around the model, but current self-evolving harnesses use robot trials inefficiently when deciding which code and skill changes to pursue. We introduce EmbodiedRSI, a self-evolving agentic harness that autonomously decides where to explore next and turns the resulting physical interaction into improved code and skills. EmbodiedRSI realizes this through a Fast-Slow Dual-System Architecture, in which competing code and skill hypotheses are maintained in a Hypothesis Graph. Value-of-Information Experiment Selection chooses physical experiments that can distinguish these hypotheses. Their outcomes guide Code-Skill Co-Evolution. The Slow System builds Hierarchical Memory, and Reward-Grounded Memory Learning selects effective memory according to their value for later Fast-System improvement. On RoboCasa365, EmbodiedRSI reaches 77.0% overall success and 71.3% on Composite-Unseen, compared with 40.1% for the best baseline. EmbodiedRSI also reaches 86.8% overall success on LIBERO-Pro. Beyond benchmark performance, EmbodiedRSI transfers zero-shot to real-world robot, achieving 71.3% overall success across multiple challenging tasks.

---

## 106. AgentTime: Can Agents Estimate and Control Their Own Runtime?

**Autori:** Michael Ofengenden, Maksym Andriushchenko  
**Data:** 2026-10-07  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.09944v2

> An essential control of AI agents is their ability to manage runtime. This ability requires a sense of time-awareness, to predict and estimate wall-clock time and to control their own actions. Prior work has focused on time-awareness, but duration-following and control in native agent harnesses remain unexplored. We present AgentTime, a benchmark for testing whether agents can work for a requested duration, predict their runtime, and estimate elapsed time afterward. It comprises 222 tasks from 18 sources spanning coding, computer use, agentic work, and automated research. Duration-following experiments append a single instruction specifying how long to work, with requests ranging from about a minute to multiple days. Accuracy on these instructions varies substantially: Fable 5.1 in Claude Code deviates from requested runtimes by a typical factor of 2.9$\times$, compared with only 1.2$\times$ for GPT-6 Astra in Codex. However, matching the requested runtime does not, by itself, establish continued work on the task. Among 158 reviewed Astra runs with classifiable transcripts, 14 explicitly slept after appearing to finish. In forecasting experiments, predictions tend to overestimate natural runtimes. In retrospective experiments, removing temporal information more than doubles deviation for Sol and Astra and nearly doubles it for Fable. An agent's ability to complete a task does not guarantee that it can control its own time or work for the whole requested duration. For agents to run reliably, safely, and autonomously over long horizons, we require the evaluation of both.

---

## 107. From Plausible Hierarchies to Useful Taxonomies: Evaluating Agentic Harnesses on Customer Feedback

**Autori:** Prabhath Chellingi, Raviraja G, Viraj Bagal  
**Data:** 2026-10-07  
**Categorie:** cs.AI, cs.LG, cs.SC  
**Link:** https://arxiv.org/abs/2610.09377v1

> Taxonomies are the symbolic representations through which AI systems organize evidence, aggregate patterns, and answer questions over large document collections. Over customer feedback, the category tree decides how every record is counted and routed, which problems get seen, and which team owns them. Agentic harnesses now make it easy to generate a plausible-looking hierarchy, and such trees are checked today with generic, individually scoped checks: each name fits its description, sits under the right parent, and stays distinct from its siblings. We ask a more operational question: when is a generated hierarchy actually useful as a production taxonomy? We build six taxonomies over two proprietary feedback corpora (1,940 and 5,000 records): for each corpus, a production reference and two repeated runs of the same harness under identical inputs. All six pass every generic naming and structure check, and a deeper product-coverage check even prefers the generated trees. Yet in every generated tree at least 97.7% of leaf names merely restate an ancestor's name (13.9% and 2.9% in the references), and in one, three of every four records fall under multiple top-level categories. We introduce two families of whole-tree metrics: structural discriminators test whether a tree's shape was learned from the data or imposed by its generator; team partitionability tests whether branches split feedback into groups teams can own. Trees the generic checks rate as equally correct differ by 27 percentage points in cross-branch leakage, and only one of the two beats a random split. Surface plausibility is an insufficient measure of taxonomy quality: evaluation must measure the whole tree as well as each node.

---

## 108. VeriFine: Scaling Verification for Self-Improvement in Embodied Reasoning

**Autori:** Zewei Zhou, Rachel Luo, Yulong Cao, Chaowei Xiao, Chensheng Peng, Boyi Li, Thomas Tian, Zheng Lian, Yan Wang, Jiaqi Ma, Boris Ivanovic, Marco Pavone, Wenhao Ding  
**Data:** 2026-10-06  
**Categorie:** cs.AI, cs.RO  
**Link:** https://arxiv.org/abs/2610.08761v1

> Self-improving policies continually expose new failure patterns, changing what their judges must be able to verify. However, current fixed judges constrain both optimization feedback and the discovery of useful training examples, limiting further self-improvement. This challenge is even more acute in embodied reasoning, where reliable evaluation must account for spatial grounding, causal reasoning, and safety-aware decision-making. We introduce VeriFine, an agent harness framework that scales verification through the co-evolution of the policy, training curriculum, and judge. The Policy Improvement Loop uses a rubric judge to diagnose recurring failures, construct an adaptive curriculum, and optimize the policy. When progress plateaus and verification becomes a bottleneck, the Judge Improvement Loop selectively queries human guidance on informative failure cases and refines the judge through coactive calibration, in which humans and agents resolve disagreements and converge toward the objective rubric of physical reasoning. The revised judge then guides the next stage of data selection and policy optimization. Experiments on driving and robot navigation tasks demonstrate continuous self-improvement in both policy and judge capability across reinforcement and supervised fine-tuning. These results show how scaling verification supports continuous self-improvement as policy failure patterns evolve.

---

## 109. Towards In-Parameter Memory Augmentation for Large Language Models

**Autori:** Haoyu Huang, Zhongwei Xie, Jiaxin Bai, Yisen Gao, Hong Ting Tsang, Wuganjing Song, Huihao Jing, Yufei Li, Yangqiu Song  
**Data:** 2026-10-06  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2610.08630v1

> Recently Large Language Models (LLMs) and LLM-based agents increasingly need to incorporate knowledge acquired after pretraining, e.g., domain facts, user preferences, documents, and interaction experience. In-context learning (ICL) and ICL-based agent harness remain flexible, but they consume context capacity and incur repeated discretized encoding cost that grows with context length. \textbf{In-parameter memory} offers a complementary substrate: reusable memory information is represented in model parameters, adapters, or other parameter-like objects that are composed into the forward pass at inference time. This survey focuses on methods that augment LLMs with such parametric memory at deployment: a memory-bearing parameter object is plugged into the forward pass during inference, whether it is acquired before or during deployment. We organize the landscape with two orthogonal axes: \textbf{Parameter Placement}, which includes Embedding, Attention, FFN layers, or Hybrid when two or more layers are used; and \textbf{Parameter Acquisition Time}, which distinguishes methods whose memory object is acquired during deployment (online) from those acquired before it (offline). We clarify boundaries, conduct comparisons, and discuss open directions in interference, safety, co-design with ICL, and recursive self-improvement.

---

## 110. EMHO: EMbodied Agent Harness Optimization via Experience Traces

**Autori:** Hyun Jung Lee, Jungtaek Kim, Jongwon Jeong, Tae-Eui Kam, Donghyun Kim, Yong Jae Lee  
**Data:** 2026-10-06  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.08432v1

> Improving embodied agents often focuses on optimizing the underlying model through training, while the surrounding agent harness that controls planning, context, and tool use is typically engineered. We ask whether this harness can instead improve itself directly from experience traces under sparse environmental feedback. We propose EMbodied Agent Harness Optimization (EMHO), a self-evolving framework that keeps the embodied model frozen and iteratively revises its harness by analyzing execution trajectories and prior harness history. EMHO optimizes beyond skills or recovery prompts, modifying how the agent monitors progress, uses vision tools, grounds observations, and responds to failures. To support multiple subtasks with a single harness, we introduce EMHO-Merge, which addresses trade-offs in jointly optimizing a single shared harness across subtasks by using episode-level gains and losses to guide evidence-supported refinement of when and how revised behaviors are applied. We evaluate EMHO on EmbodiedBench across navigation and manipulation tasks, and EMHO consistently improves task success for both Qwen 9B and 27B models. Qualitative analysis shows that EMHO goes beyond recovering from failures and unproductive actions to reshape how the embodied agent interprets and interacts with its environment.

---

## 111. Learn2Play Bench: How Well Do LLM Agents Learn from Experience in Unfamiliar Environments?

**Autori:** Yibo Li, Jinhang Qiu, Zhi Zheng, Qianyun Guo, Jiaying Wu, Shuo Ji, Bryan Hooi  
**Data:** 2026-10-06  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.08215v2

> Learning from experience is essential for LLM agents to adapt to unfamiliar and dynmaic environments. Evaluating this ability is therefore important for understanding how effectively agents acquire and use new knowledge. Existing benchmarks have sought to evaluate this ability, but they primarily evaluate tasks whose rules are provided in the instructions or already familiar to pretrained models, making it difficult to distinguish learning from interactions from reasoning with existing knowledge. To address this, we introduce Learn2Play Bench, a benchmark of newly designed text-based games, whose rules are novel or counterintuitive, requiring agents to acquire knowledge through interaction rather than rely solely on pretrained knowledge. These games provide reproducible feedback and automatic scoring, enabling controlled evaluation of learning across repeated attempts. We also vary game instances to test whether agents can apply what they have learned to new situations. Therefore, we evaluate how backbone models, self-evolving methods, and agent harnesses affect agents' learning ability, revealing three findings: (1) Experience retention: Retaining complete records of actions and feedback can support more effective learning than summarizing these experiences into rules or strategies. (2) Human agent gap: Top-performing human players achieve higher peak scores than the evaluated agents. Human explore more varied strategies, and repeat actions less. (3) Harness matters: With the backbone fixed, changing the harness can improve performance while reducing estimated inference cost. Together, these findings provide insights into how LLM agents learn from experience and suggest directions for future work to improve their learning ability. Project website: https://liushiliushi.github.io/learn2play-bench-website/

---

## 112. Internalizing Agent Experience into Diffusion Model Weights via On-Policy Context Distillation

**Autori:** Wenxuan Wang, Zekai Liu, Weinan Zhang, Yu Cheng, Yang Yang  
**Data:** 2026-10-05  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.07250v1

> Wrapping an image generation model in an agentic harness can effectively boost Text-to-Image task performance: the harness can leverage memory, skills, workflow orchestration, result verification, and iterative refinement to continually construct and revise prompts, thereby eliciting better images. These gains, however, remain external to the diffusion model and are realized only while the full harness runs. We propose Diffusion On-Policy Context Distillation (D-OPCD), which treats the agent-improved prompt as privileged context and distills the knowledge encoded in the agent harness into the weights of the diffusion model, so that the model retains part of the harness's benefit when conditioned on the original query alone. Using a Text-to-Image agent equipped with our proposed Auto Skill Evolver (ASE), we show that D-OPCD can internalize harness capabilities into the generator's weights, raising the average direct-generation score from 60.52 to 65.09 across four benchmarks. With this knowledge absorbed into the weights, the harness can shed its saturated skills and resume evolving: a second ASE round on the updated generator improves on a skill-free harness by additional 1.83 points, pointing toward text-to-image systems in which harness and model keep improving each other through continual co-evolution.

---

## 113. Can Agent Harnesses and Inference Engines Hear Each Other? The HEAR Protocol for Agentic LLM Serving

**Autori:** Jiaqi Zhao, Haodong Chen, Jitai Hao, Wei Zhao, Jinghao Pang, Qiang Huang, Jun Yu  
**Data:** 2026-10-05  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.06597v1

> LLM agents increasingly execute complex workflows involving multi-turn reasoning, tool use, and parallel agents. Efficient serving requires decisions that span two layers with complementary information: the agent harness understands workflow dependencies, context lifecycles, and execution objectives, whereas the inference engine observes request queues, KV-cache state, resource pressure, and execution capabilities. Existing interfaces do not systematically connect these views, limiting workflow-aware execution. HEAR, a bidirectional Harness--Engine Pairing protocol for agentic LLM serving. HEAR standardizes how the harness communicates workflow intent and execution requirements and how the engine returns runtime state, capabilities, and outcomes. By separating protocol semantics from optimization policies, HEAR supports diverse coordination strategies without changing workflow or model semantics. We instantiate HEAR for online cache-aware runtime coordination and workload-aware execution-mode selection for agent roles. Across four conversational and research-agent benchmarks under memory-constrained, concurrent serving, HEAR achieves a $1.61\times$ batch speedup and reduces median time-to-first-token by $2.23\times$ on SCBench. Mooncake shows that workflow intent and live engine state provide complementary benefits across load regimes. On BrowseComp-Plus and DeepResearchBench, workload-specific configurations yield $1.23\times$ and $2.45\times$ end-to-end speedups, respectively, without observed task-quality degradation. These results establish HEAR as a reusable coordination substrate for efficient agentic LLM serving.

---

## 114. HERA: Harness-Environment Co-Evolution for Reliable Agentic Abstention

**Autori:** Han Luo, Bingbing Wen, Guang Yang, Zora Zhiruo Wang, Pan Lu, Lucy Lu Wang  
**Data:** 2026-10-05  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.06563v1

> Large language model (LLM) agents are increasingly capable of acting in complex tool-use environments, yet they often fail to recognize when tasks are infeasible and no valid solution exists. Recent work has formalized this reliability gap as the problem of agentic abstention, and existing approaches typically optimize a model or agent harness against a fixed set of tasks, leading to limited generalization to unseen failure modes. We introduce HERA, a framework for harness-environment co-evolution for agentic abstention. HERA consists of (i) a pipeline to automatically construct verifiable pairs of feasible and infeasible tasks by applying controlled environment mutations that transform solvable tasks into cases requiring abstention, and (ii) a co-evolution procedure in which performance failures on previous tasks are used to drive harness adaptation and generate new execution environments and tasks geared towards previous weaknesses. On held-out evaluation tasks, an evolved harness from HERA improves abstention accuracy from 61.7% to 83.3% while improving feasible-task completion from 68.3% to 76.7%, achieving the highest abstention and feasible-task completion among the compared methods. The resulting best harness transfers across 19 other LLMs, improving abstention accuracy by 15.3 percentage points on average without any model-specific optimization, and enabling smaller models to match the performance of more powerful models at an estimated 85% lower cost.

---

## 115. MedicalHarness: A Controlled Evaluation of LLMs and Agent Harnesses on Medical Tasks

**Autori:** Ziqing Wang, Lili Zhao, Kaize Ding  
**Data:** 2026-10-05  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2610.05778v1

> LLM agents are increasingly built for medical work and scored on clinical benchmarks. Each such score, however, comes from a model running inside an agent harness, the system that controls the loop between the model and its environment. An agent's score is therefore a property of a model--harness pair. For medical agents, how much outcomes change with the harness has rarely been measured. Measuring this change, and explaining it, raises two challenges. First, a harness comparison must change nothing but the harness and be repeated across models and kinds of task. Second, comparing whole harnesses leaves their mechanisms bundled together, so it cannot show when an individual mechanism helps. To address these challenges, we present MedicalHarness, a controlled study of models and agent harnesses on medical tasks. We first build MedicalHarnessBench to evaluate agents on $107$ tasks across four domains that each test a different harness capability. Using this benchmark, we run five open-weight models under five agent harnesses, changing only the harness within a comparison, and analyze both outcomes and execution traces. To study individual mechanisms, we build MH-Lab, a controlled harness that switches off context management, planning or tool exposure one at a time within a shared execution loop. We find that the harness and its interaction with the model account for about a quarter of the outcome variance, and that no single harness is best across models and tasks. Code and data are available at https://github.com/REAL-Lab-NU/MedicalHarness.

---

## 116. LifeLong Digital Twin: A Unified Modeling Paradigm and Agent Harness for Event-Driven Lifelong Health State Trajectories

**Autori:** Jin Jiang, Sean Yates, Jasper Chong, Raymond Brooks, Alex Lawson, Yuqin Qin, Liangcai Gao  
**Data:** 2026-10-04  
**Categorie:** cs.AI, q-bio.QM  
**Link:** https://arxiv.org/abs/2610.05566v1

> Human health is a continuous, dynamic trajectory shaped by the cumulative interplay of biological processes, clinical events, behaviors and environmental exposures across the life course. Unifying the full breadth of lifelong health information, including longitudinal records, genetic variation, molecular profiles and environmental histories, is essential for whole-person modeling and remains a major challenge. We introduce LifeLong Digital Twin, a unified, event-driven modeling paradigm that organizes Life Events into daily Health States and accumulates them into Lifelong Health Context. An accompanying Agent Harness incorporates multimodal evidence beyond the language model's textual context. We evaluate four language models across 25 disease endpoints on three tasks: Disease Trajectory Forecasting, Disease Risk Ranking and Multi-horizon Disease Prediction. The approach yields marked gains over the reference condition: model-averaged F1 increases by 22.0% for disease identification in trajectory forecasting and 18.3% for five-year disease outcomes; thyroid-disease F1 reaches 0.669. The framework provides a foundation for whole-person digital twins and research on personalized lifelong disease prevention.

---

## 117. Harness-Search: Guiding Long-Horizon Search through Multi-Agent Coordination

**Autori:** Shanyong Wang, Zhenwen Ji, Lei Jin, Yining Zhao, Yicheng Qian, Chengqiang Lu, Yi Wu, Yao Hu, Lizhen Cui, Yanyu Xu  
**Data:** 2026-10-04  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2610.05382v1

> Long-horizon search requires agents to gather evidence across multiple steps and synthesize it into well-supported answers. The recent agent harnesses provide a natural and promising framework to support such long-running search processes. As interaction histories grow, one single agent in harnesses might get stuck and cause the policy to lose track of unresolved questions, overlook useful evidence, or terminate before sufficient support has been collected. One of promising way is to decouple three distinct responsibilities of proposing retrieval actions, updating persistent state, and deciding when to stop rather than concentrating them within a single policy. Targeted at it, we introduce Harness-Search, a multi-agent search harness to reduce the local errors propagating across subsequent exploration, evidence curation, and termination decisions. In particular, Harness-Search assigns these responsibilities to three permission-bounded authorities: a Retrieval Policy that proposes search operations, a Memory Operator that validates and commits persistent-state updates, and a Summary Auditor that accepts or rejects termination based on the sufficiency of the curated evidence. Together, these roles form a Propose-Commit-Audit loop in which actions are proposed, persistent evidence is selectively committed, and stopping decisions are subjected to an explicit sufficiency check. Across seven long-horizon search benchmarks, Harness-Search improves both retrieval and answer generation under the same policy backbone, increasing Recall by 4.60-27.92 points and Final-Answer Recall by 12.34-30.13 points over the strongest harness-based baseline on each evidence-retrieval benchmark. Moreover, trajectory-level analyses show that Harness-Search continues to accumulate useful evidence and expand evidence coverage with less redundant retrieval as the search history grows.

---

## 118. MESH-Harness: Self-Improving Agent Harnesses via Bandit-Guided Compositional Evolution

**Autori:** Zhiwei Shang, Yu Huo, Mingrong Gong, An Yan, Zikun Qu, Junhao Dong, Bryan Kian Hsiang Low, Chenglin Wu, Zhongxiang Dai  
**Data:** 2026-10-04  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.05300v1

> An agent harness is the code that organizes context, maintains state, and coordinates tool calls for a language model. We study how to improve the harness under a limited evaluation budget while keeping model weights fixed. Our method, MESH-Harness, organizes each harness into functional modules with explicit role-specific interfaces, allowing alternative implementations of each module to be substituted and recombined. It uses shared module representations and full-covariance LinUCB to score candidate combinations based on predicted performance and exploration value. Mixed-start coordinate ascent selects complete configurations for evaluation without enumerating the combinatorial space. Validation traces then guide local code edits, and the resulting candidates are incorporated into fixed-capacity role-specific pools for subsequent recombination. On text tasks, retrieval-augmented mathematical reasoning, code generation, and interactive scientific tasks, MESH-Harness outperforms Meta-Harness by 5.70, 7.01, 2.00, and 5.00 points, respectively, under matched candidate-evaluation budgets. Iterative harness optimization improves MESH-Harness by 5.63-7.79 points over its first-round configurations. For the reported configurations, aggregate test-time cost is 44.2% lower than that of Meta-Harness, while total cost including search is 14.6% lower. These results show that combining module-level design reuse with feedback-driven compositional search can systematically improve agent harnesses while keeping overall optimization cost under control.

---

## 119. Causal Improvement Graph for Agentic Harness Optimization

**Autori:** Junjie Zhang, Shunyu Liu, Haoyu Wang, Ting-En Lin, Yongbin Li, Dacheng Tao  
**Data:** 2026-10-04  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2610.05039v1

> Agentic Harness is the runtime that constructs task context and controls execution flow, thereby shaping overall agent performance. Given a fixed model and external evaluation, automated Harness optimization seeks to improve this runtime through an iterative proposal--evaluation loop to better solve target tasks. Existing meta-harness methods mainly adopt proposer-centric discovery, in which an LLM-based proposer integrates accumulated experimental findings to determine subsequent Harness revisions. This places the burden of maintaining the evolving improvement state on the proposer as history expands and its underlying experimental logic becomes harder to discern. In this paper, we introduce the Causal Improvement Graph (CIG), a graph-governed meta-harness framework that externalizes the evolving improvement state in a persistent graph, allowing prior findings to directly govern subsequent Harness optimization through local proposer operations. CIG grows and links Evidence, Hypothesis, Intervention, and Outcome nodes to represent what was observed, how it may be explained, how to test that explanation, and what the evaluation reveals. Their structural relations preserve how the improvement state changes across iterations, allowing local proposers to build directly on relations among prior findings rather than recover them from raw history. Across various agent tasks, CIG discovers stronger Harnesses than previous meta-harness baselines and remains robust to the choice of task solver and proposer. Structural ablations further support the design of an explicit improvement state with graph-governed evolution.

---

## 120. Complex Agents, Shallow Tests: Demystifying and Enhancing Test Adequacy of Agent Harness in the Wild

**Autori:** Yifan Xiong, Jingyi Ge, Zhenpeng Chen, Yiling Lou  
**Data:** 2026-10-04  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2610.04921v1

> LLM-based agentic systems are emerging as a new software paradigm. Modern agents are typically composed of backbone LLMs and a surrounding harness that serves as the operational software infrastructure for agent execution. As agent harnesses grow increasingly complex, agents suffer from diverse harness implementation bugs, raising substantial reliability concerns. In this work, we conduct the first empirical study to systematically investigate the test adequacy of harness in real-world agentic systems. Our analysis reveals that agent harness remains substantially undertested. In particular, LLM-dependent harness (LDH) code, despite its critical role in processing LLM outputs and governing agent behavior, receives limited testing attention, with less than half of its lines and branches covered by existing tests. Motivated by these findings, we further propose HarnessTester, the first harness-oriented test generation technique that incorporates explicit agent-harness contract support to construct contract-faithful test setups and extensively exercise LDH code. Our evaluation shows that HarnessTester substantially outperforms state-of-the-art general-purpose test generation techniques in achieving 75.95%/84.76% larger line/branch coverage gains and 69.89% larger mutation-score gains. Furthermore, HarnessTester detects 122 real-world harness bugs in widely-used agentic systems (e.g., OpenClaw), among which, 88 bugs are previously-unknown bugs and 69 bugs have been confirmed by agent developers. These results highlight the practical effectiveness of HarnessTester in improving test adequacy and assuring the reliability of real-world agentic systems.

---

## 121. SHarP: Saliency-based Pruning of Agent Harnesses

**Autori:** Xinyi Gao, Qiucheng Wu, Kaizhi Qian, Handong Zhao, Shiyu Chang, Yang Zhang  
**Data:** 2026-10-03  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.04178v1

> Agent harnesses are systems that coordinate model calls, tool use, and task execution to help large language models complete complex tasks. To meet task requirements and address failures, these systems are often iteratively refined by amending and patching their instructions, tools, and workflows, continuously increasing harness complexity. It is therefore unclear whether some resulting harness modules are redundant, introducing substantial token overhead with little, if any, performance gain. Inspired by neural network pruning, in this paper, we study harness pruning as a means of striking a better balance between task performance and token cost. We propose SHarP (Saliency-based Harness Pruning), a simple yet effective pruning strategy based on the saliency of each harness module with respect to performance and efficiency. Specifically, we first identify tools, instructions, and supporting mechanisms as components that can be individually disabled. We then estimate the saliency of each module by ablating it and assessing its task performance and token cost relative to the full set of single-module ablations. Modules with the smallest contribution to performance or largest computational overhead are subsequently pruned. Our evaluation across various harnesses on held-out validation sets reveals a surprising finding: most harnesses that we studied are highly redundant and can maintain comparable performance and efficiency even after a substantial portion of their modules are pruned. Our pruning approach and empirical findings provide new perspectives on agent harness design and optimization.

---

## 122. Dynamic Harness Search: Building Multi-Agent Systems Per-Query via Prediction

**Autori:** Som Sagar, Shasha Li, Hejie Cui, Ransalu Senanayake, Sercan Ö. Arık  
**Data:** 2026-10-02  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2610.04137v1

> Agent harnesses specify the roles, instructions, tools, and communication structure used to solve a task, and the right harness depends on the query. Because the value of each design choice is observable only through execution, tailoring a harness to each query has required either executing alternatives at inference time or costly manual design. We introduce SHIFT, which moves execution out of the per-query search loop. A local LLM architect learns a policy over harness-building actions from search, and a value function that predicts, from measured executions, a utility balancing accuracy against execution cost. For each query, Monte Carlo tree search uses these predictions to construct a harness. Across 9,193 tasks in six benchmarks, from math to document and general-assistant tasks, with a Gemini 3.5 Flash executor, SHIFT attains the highest mean accuracy, about 80%, outperforming 17 baselines that span prompting, prompt optimization, and workflow search, and exceeding the strongest baseline by 7.2 percentage points. A cheaper mode of SHIFT also attains a higher mean accuracy than every baseline while using 32% fewer execution tokens than the strongest baseline. We further show that choosing structure, instructions, and tools jointly beats choosing only instructions or only tools by up to 9.1 percentage points, and that learned value selection identifies more accurate harnesses with lower execution cost from candidate pools.

---

## 123. MOF-VERIFY: A Failure-Aware Agentic Harness for MOF Hypothesis Verification

**Autori:** Donghyun Lee, Taehoon Lee, Geonhee Ahn, Jieun Kim, Jihyun Park, Suyeon Cho, Yoona Kim, Chaerim Shin, Hoi Ri Moon, Jonggeol Na, Sukho Hong, Jihwan Oh, Soo Kyung Kim  
**Data:** 2026-10-02  
**Categorie:** cs.AI, cs.CE  
**Link:** https://arxiv.org/abs/2610.03056v1

> Large language models are increasingly used as reasoning components in AI-driven materials Co-Scientists, yet the reliability of the resulting verification pipeline remains unclear. Metal-organic frameworks (MOFs) provide a particularly challenging setting because structures may appear under different identifiers, synthesis outcomes depend strongly on experimental conditions, evidence is distributed across heterogeneous sources, and some hypotheses require computation rather than literature alone. We introduce a diagnostic benchmark with four task families covering structural grounding, synthesis-condition verification, evidence-sufficiency verification, and MLIP-based computational verification. T-MOF-1-3 are evaluated under closed-book, retrieval-enabled, and oracle-evidence settings to localize failures in knowledge access, evidence acquisition, and reasoning, while T-MOF-4 separately evaluates computational verification. Guided by these diagnosed failure modes, we develop MOF-Verify, a failure-aware agentic harness that targets structural, literature, evidence-sufficiency, and computational bottlenecks before producing a final verdict. Across multiple backbone LLMs, MOF-Verify substantially improves hypothesis-verification performance over direct inference and retrieval-based baselines. Benchmark datasets are released at https://github.com/IMMS-Ewha/MOF-Verify-Benchmark.

---

## 124. Continual Graph Memory for Mathematical Research Agents

**Autori:** Junyi Zhang, Jinxi Yu, Eric Hanchen Jiang, Jiachen Lu, Zhi Zhang, Xinjie He, Hyunsik Chae, Ethan Ji, Alexander K Taylor, Vigyan Sahai, Yiwen Kou, Kai-Wei Chang, Raghu Meka, Nanyun Peng, Amit Sahai, Terence Tao, Wei Wang  
**Data:** 2026-10-02  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2610.02945v1

> Using frontier agent harnesses to tackle mathematical research problems has emerged as an effective means of advancing mathematics. However, solving frontier problems in mathematics may require a massive number of agents working in parallel for extended periods to construct proofs, thereby generating an enormous volume of intermediate proof results. Organizing these intermediate results throughout a long-horizon proof-search process and reusing knowledge gained from prior explorations remain major challenges. We present Ansatz, a mathematical research agent built around Continual Graph Memory, a graph-based, evolvable, cross-problem mathematical research memory system that explicitly organizes the entire proof search process and reuses information from exploration trajectories of previous problems. Specifically, we develop a unified graph memory that represents all intermediate exploration results, including facts, plans, and counterexamples, together with edges that explicitly represent the relationships among them; dependency-aware retrieval supplies precisely targeted local context; an evidence-sensitive curator updates the research frontier and distills lessons from prior attempts; and scoped recall surfaces earlier statements and negative findings for local re-proving rather than uncritical reuse. Experiments cover runs across all ten First Proof Second Batch problems, together with four component studies. Ansatz reports closure on all ten research tasks, demonstrating its ability to sustain and resume long-horizon mathematical search. Beyond these problems, Ansatz also produces solutions to the Jamison caterpillar conjecture and Erdős Problems 289, 348, and 488 without human intervention, and makes partial progress on several open problems, illustrating its strong ability to solve open mathematical research problems.

---

## 125. HASTE: Evolving Agent Harnesses Against Emerging Attacks Using Sparse Evidence

**Autori:** Xiqiao Xiong, Moxin Li, Zhixin Ma, Ouxiang Li, Wenjie Wang, Fuli Feng, Xiangnan He  
**Data:** 2026-10-02  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.02920v1

> Agent harnesses play a critical role in defenses by enforcing safety constraints to prevent unsafe actions. However, rapidly emerging attacks outpace manual harness adaptation, motivating automated harness evolution. Yet the signals available for harness evolution are often sparse, such as brief descriptions or a few attack examples in threat reports and preprints. To address this limitation, we introduce HASTE, a multi-agent framework that evolves agent harnesses from sparse threat evidence through an adversarial interplay between safety-specification generation and attack-case generation. Safety specifications guide harness updates toward addressing identified safety vulnerabilities, while attack cases probe for remaining safety vulnerabilities after each update. By feeding evaluation outcomes back into both processes, HASTE enables harness evolution against emerging attacks beyond the initially observed evidence. Experimental results across multiple backbone models, attack types, and evidence forms show that HASTE consistently reduces attack success rates while preserving benign-task utility. The code is available at https://github.com/xxiqiao/HASTE.

---

## 126. WebUIProof: Benchmarking WebUI Code Generators with UI-Agent Execution Harness

**Autori:** Yun-Yun Tsai, Yuning Mao, Shiqi Wang, Junfeng Yang, Sinong Wang  
**Data:** 2026-10-02  
**Categorie:** cs.SE, cs.AI, cs.MA  
**Link:** https://arxiv.org/abs/2610.02617v1

> Evaluating WebUI code generation at scale is difficult: outputs may compile and look plausible yet fail under user interaction, and prior benchmarks largely rely on free-form prompts with static checks (build success, screenshots) that miss functional correctness. We introduce WebUIProof, an execution-oriented benchmark that provides structured specifications and dense, executable interaction tests for WebUI generation across two task families: general WebUIs (e.g., dashboards, game, interactive tools) and 3D interactive simulation (e.g., particle/galaxy systems, physics dynamics). WebUIProof includes a UI-agent harness that runs executable interaction tests in a headless browser using an iterative plan--act--observe loop: it locates DOM elements, performs actions, observes resulting UI/DOM changes, and checks the specified assertions. We evaluate across eight commercial LLMs and observe frequent failures on interaction-based requirements even when pages render successfully, especially on 3D simulation interfaces. Finally, we show the UI-agent harness can provide outcome-level training signals. Training compact models (e.g., Qwen2.5 14B and MIMO 7B) with RL rewards derived from executable interaction tests improves functional completion while reducing build failures.

---

## 127. VERSE: Verified Self-Evolving Optimizer for Agent Harnesses

**Autori:** Zekai Wang, Yingqiang Ge, Zekun Wang, Hai Wang, Yuhui Xu, Joshua Frandsen, Shancong Fu, Ashia C. Wilson, Chandan K. Reddy  
**Data:** 2026-10-02  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2610.02616v1

> Harness evolution improves an LLM agent's prompts, tools, and workflow, while the optimizer's own tools and procedures often remain fixed. We study whether an optimizer can improve another agent more effectively by also improving how it diagnoses failures, develops edits, and tests their effects. Two observations guide our design. In a controlled study, optimizer self-evolution fails to improve performance without execution-based verification, but achieves the best result of that study when verification is available. Across five executors, self-evolving optimizers build their own tools for failure analysis, verification, training audits, and workflow control. Motivated by these findings, we introduce VERSE, a Verified Self-Evolving optimizer for agent harnesses. VERSE lets the optimizer test draft edits, replay failures, and perturb suspected steps before submission, while tracking fixes and regressions across rounds. Using this feedback, the optimizer revises both the executor harness and its own prompts, skills, tools, hooks, and notes, while the weights of the optimizer and executor models stay fixed. Under a shared protocol with disjoint training, validation, and test tasks, VERSE improves all four evaluated harness optimizers on held-out SWE-rebench tasks and newer out-of-distribution tasks in five languages. Its best validation-selected harness reaches 42.3% and 37.7% accuracy, respectively, against 39.2% and 29.3% for the strongest baselines. Code is available at https://github.com/wzekai/VERSE.

---

## 128. Harnessing LLMs as Agents: What Does It Cost?

**Autori:** Zelin Zhao, Xinyu Guo, Jingyuan Zhang, Yuxuan Zhang, Yongxin Chen  
**Data:** 2026-10-01  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2610.02488v2

> Language-model agents increasingly rely on harnesses that manage bounded context, persistent memory, tools, verification, and repeated execution, yet existing notions of model capability do not quantify the computational resources these mechanisms consume. We introduce the Language Model Agent Machine (LAM), a resource-bounded abstraction that fixes the underlying semantic model while explicitly charging harness-level resources. We establish four classes of results. Communication: LAM execution is instancewise equivalent to red--blue pebbling under simultaneous call--transfer budgets, transferring classical I/O lower bounds to context--memory traffic. Access: memory interfaces induce asymptotic separations, including a $Θ(n)$ gap between random and non-speculative sequential access on pointer chasing. Recomputation: bit-reversal DAGs require $Θ(n^2/(C+S)+n)$ model calls with context capacity $C$ and persistent-memory capacity $S$, quantifying when stored intermediate state avoids repeated semantic computation. Reliability: we derive tight stage-local sampling bounds, exact imperfect-verification costs, and a Young--Daly-type checkpoint law with a closed-form optimal verification interval. Controlled and held-out experiments on GPT-6 Astra test communication and reliability predictions, including checkpoint optima, policy selection under programmatic checking, and tradeoffs among call granularity, logical input traffic, and reliability on chained MATH tasks. Together, these results provide a resource theory for the computational cost of language-model agent harnesses.

---

## 129. Mingbird: A Local-First Agent Harness Enabling Small Open Models to Complete Real Tasks

**Autori:** Hao Wang, Ting Huang  
**Data:** 2026-10-01  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2610.02001v1

> Small open-weight models (2-9B) run on ordinary laptops, but under cloud-scale agent harnesses they rarely complete real tasks: tool prefill overflows the context, self-correction diverges, tool demonstrations loop, and tasks are silently abandoned. We present evidence, from a controlled single-machine comparison and one third-party benchmark, that a substantial share of these failures is attributable to the harness rather than the model. We introduce Mingbird, a local-first agent harness for Windows and Ollama whose ten mechanisms compensate point-by-point for small-model failure forms, three of them representative: a byte-level net-zero prefill budget, a finish gate that re-reads the task before accepting completion, and signature-level loop detection. On LRAB, a controlled comparison holding machine, models, budgets, and scoring fixed (4 harnesses $\times$ 4 open models (2B-35B) $\times$ 18 real tasks, deterministic artifact scoring), Mingbird reaches 0.886 overall against 0.631 (goose), 0.479 (opencode), and 0.405 (agent-mini), with all 288 cells published; on $τ^2$-bench (278 tasks, three arms, one protocol) it totals 0.856 against 0.791 and 0.737; and a frontier-model probe on the same 18 tasks spans 0.997 to 0.478 across harnesses, with well-formed scaffolds staying within 0.072 of each other. A leave-one-mechanism-out ablation is reported as directional only: same-night replications of the same arm move its mean by up to 0.069, the size of every nominal single-trial delta, and the one batch-matched comparison (full mechanism stack versus text re-read alone) gives the executable completion guards a paired +0.10 across three replications. The evidence carries stated limits: a self-built benchmark, a single machine, and single-trial scoring.

---

## 130. Continuous Process-Level Evaluation for Evolving Enterprise AI Agent Skills

**Autori:** Ngoc Phuoc An Vo, Aarya Doshi, Vadim Sheinin  
**Data:** 2026-10-01  
**Categorie:** cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2610.01833v1

> Enterprise AI agent skills evolve as tool APIs, models, and specifications change, yet final-output evaluation can miss process-level behavioral drift. We present a continuous evaluation framework combining outcome-level and process-level checks, applied to Revenue and Productivity variants of a Business Value Determination skill in an enterprise Value Aware Resiliency system. The framework independently computes per-run ground truth, materializes reusable template tests, and evaluates tool selection, arguments, execution order, and database integrity through programmatic checks and a narrowly scoped LLM judge. We evaluate 240 trials across two skills, two specification variants, two agent harnesses, and three models. Of 175 trials passing all applicable final numerical checks, 162 (92.6 percent; Wilson 95 percent CI: 87.7-95.6 percent) contained another evaluator-detected deviation. Under a broader seven-check final-state definition, 151 of 164 passing runs (92.1 percent; 95 percent CI: 86.9-95.3 percent) still violated a trajectory check. Dependency attribution reduced a mean of 6.34 failed checks per run to 2.65 roots. Specification sensitivity varied by model and harness, with exploratory bootstrap interaction intervals excluding zero for all three Revenue comparisons and one of three Productivity comparisons. Runtime-resolved templates provided reusable regression coverage across the evaluated configurations; longitudinal validation under actual API evolution remains future work.

---

## 131. VideoEvolve: Evolving Agent Harnesses for Video Temporal Grounding

**Autori:** Bingjun Luo, Yuhuan Fan, Jialin Guo, Siqi Li  
**Data:** 2026-10-01  
**Categorie:** cs.AI, cs.CV  
**Link:** https://arxiv.org/abs/2610.01766v1

> Video temporal grounding aims to localize events in videos from natural-language queries. For agents built around frozen video-language models, the harness determines how queries guide temporal predictions and how those predictions are refined. Manually refining these harnesses requires diagnosing grounding failures and coordinating changes to both agent workflows and instructions. We introduce VideoEvolve, a framework that automatically evolves agent harnesses for video temporal grounding. VideoEvolve uses a Cloze-Structured Harness Representation that preserves stage interfaces while leaving agent workflows and instructions open to evolution. Branch-Guided Harness Evolution preserves promising code branches for continued refinement, using execution feedback to guide local edits and validation to determine which improvements are carried forward. Experiments demonstrate improved grounding performance across multiple benchmarks. Component analyses identify instruction refinement as a consistent source of gains, while the benefits of evolved code vary across evaluation settings. Together, these results support automated harness evolution as an effective approach to improving video temporal grounding. Code is available at https://github.com/bingjunluo/VideoEvolve .

---

## 132. Fast Models, Slow Evidence: A Paired and Self-Audited Evaluation of System-1 Decision Models for LLM Agent Harnesses

**Autori:** Jiawei Li  
**Data:** 2026-10-01  
**Categorie:** cs.AI, cs.CL, cs.CR, cs.LG  
**Link:** https://arxiv.org/abs/2610.02267v1

> Agent harnesses make many small, typed decisions per task: which model to call, which tool to use, whether retrieved text is relevant, whether an input carries an injection. System-1 decision models answer such questions in a single forward pass with class probabilities, promising large cost and latency savings over LLM calls. We present a paired evaluation of an open-weight (Laya) and a hosted (Jev) System-1 model on 11 agent decision points built from 18 public sources: 7,283 base cases plus 6,640 robustness variants, with byte-identical inputs, paired tests, and cross-hardware and cross-day reproducibility checks. Jev is significantly more accurate on 9 of 11 decision points (+10.8 to +46.0 pp). Neither model beats chance on zero-shot model routing, and they tie on RAG relevance gating. Laya changes 30% of its answers when the option order is reversed and degrades sharply with many or similar candidates (31% at 50 nearest-neighbour tools, vs. 98% for Jev on items with a unique correct tool). We also audit our own pipeline. Three analysis errors and one design confound distorted headline deployment claims: an omitted pre-screen cost (reported 23.9% saving, actual 4.3%), gate accuracy reported as end-to-end quality (58% vs. 98%), in-sample thresholds (5% target, up to 17% held-out misses), and a "channel effect" on injection false positives that vanishes with channel-native content. Two other suspected confounds did not change the conclusions. All cases, raw outputs and analysis code are available at https://github.com/David-DL-Space/sys1-eval.

---

## 133. WAMJET: A Harness for World Action Model Acceleration

**Autori:** Le Chen, Lixin Liu, Jan Schneider, Zeju Qiu, Simon Guist, Bernhard Schölkopf, Dieter Büchler  
**Data:** 2026-10-01  
**Categorie:** cs.CV, cs.AI, cs.RO  
**Link:** https://arxiv.org/abs/2610.03797v3

> World Action Models (WAMs) leverage pretrained video foundation models for robot manipulation, but their large backbones and video-action co-prediction are expensive. Although existing acceleration techniques offer many ways to reduce this cost, selecting and composing them requires substantial engineering for each model and hardware platform. To tackle this bottleneck, we present WAMJET, an agentic harness that accelerates WAM inference by equipping coding agents with reusable optimization guidance and measurement and validation tools. WAMJET follows a bottleneck-driven workflow where the agent profiles inference, modifies targeted code, validates effects, and iteratively refines the acceleration stack as bottlenecks shift, while preserving action quality. Experiments span six WAMs, three coding agents, and two GPU architectures. WAMJET achieves up to 9.95x lossless speedup over upstream implementations. Approximation and hardware-aware optimization yield additional latency reductions, with comparable success rates. The results show that WAMJET can produce effective acceleration stacks for WAM deployment.

---

## 134. ActiveSaddler: Automated Curriculum Learning for Agent Harness Optimization

**Autori:** Sungho Park, Wonjoong Kim, Jue Zhang, Wook-Shin Han, Pengfei Gao, Chanyoung Park, Yongqiang Yao, Rao Fu, Elsie Nallipogu, Qingwei Lin, Victor Rühle  
**Data:** 2026-10-01  
**Categorie:** cs.AI, cs.CL, cs.LG, cs.MA, cs.SE  
**Link:** https://arxiv.org/abs/2610.00906v1

> Automated harness optimization can substantially improve LLM agents by iteratively updating their prompts, tool interfaces, and control logic from execution feedback. However, existing methods primarily optimize how the harness is updated while largely fixing which training scenarios generate the feedback that drives those updates. As the harness evolves, the scenarios most useful for further optimization can change, suggesting that the training curriculum itself should adapt alongside the harness. We formulate this missing dimension of harness optimization as an automated curriculum learning problem and introduce ActiveSaddler. ActiveSaddler models the evolving curriculum as a non-stationary bandit with dynamically instantiated optimization targets. It abstracts recurring failures into reusable failure-pattern arms, estimates the potential learning progress from further targeting each pattern, and adaptively balances revisiting known weaknesses with exploring unseen scenarios for new ones. Optimization outcomes continually update both the set of discovered failure patterns and their priorities, allowing the curriculum to co-evolve with the harness. Experiments on GAIA2 and Terminal-Bench 2.0 show that ActiveSaddler consistently discovers stronger harnesses, improving test Pass@1 by 4.4 and 7.5 percentage points over the same harness optimizer using a scenario order fixed before optimization, respectively. Ablations further show that these gains depend on dynamically constructing optimization targets, estimating their evolving utility, and balancing continued optimization with new failure discovery. Together, these results establish automated curriculum learning as a new crucial optimization dimension for harness optimization.

---

## 135. Cross-Benchmark Transfer from RL on Agentic Coding Tasks

**Autori:** Sushant Mehta, Logan Ritchie, Edwin Chen  
**Data:** 2026-10-01  
**Categorie:** cs.LG, cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2610.00890v1

> Coding agents often fail in the last mile: they build most of a feature but drop a requirement, test only the cases their implementation already handles, break behavior that was supposed to stay intact, or validate against an unchecked assumption. We ask whether reinforcement learning (RL) on expert-built agentic coding tasks closes this gap, and whether what the agent learns transfers beyond the training distribution. We post-train Kimi K2.7 Code, a 1T-parameter (32B active) open-weight mixture-of-experts model, with RL alone on 1,700 tasks: 1,000 repository tasks graded by hidden fail-to-pass tests and by pass-to-pass tests of existing behavior, and 700 terminal tasks graded by expert-written hidden verifiers. The reward is the fraction of target checks passed and drops to zero if any pass-to-pass test fails. One epoch of GSPO on a rank-32 LoRA adapter improves pass@1 on each of the six external benchmarks we evaluated, across three agent harnesses: SWE-Bench Pro (60.1 to 64.8), DeepSWE (31.0 to 43.4), Terminal-Bench 2.1 (67.4 to 82.0), Terminal-Bench 3 (1.4 to 12.1), Terminal-Bench 4 (0.0 to 7.6), and SWE-Marathon (5.0 to 25.0). Pooled over the five independent task sets (Terminal-Bench 4 revises Terminal-Bench 3), the improvement is significant (p < 0.001), and it remains significant on the three sets released after the training data was collected (p = 0.004); the model also improves under both harnesses never used in training. Median trajectories on DeepSWE and Terminal-Bench 3 are 24-35% shorter in agent steps. The base model's failed DeepSWE runs are mostly near-misses, and on the tasks the trained model newly solves, paired trajectories show it avoiding each of the four failure modes above.

---

## 136. FORALL-LEAN-AGENT for Auditable Reasoning in Formal Mathematics and Software Verification

**Autori:** Naing Oo Lwin  
**Data:** 2026-10-01  
**Categorie:** cs.SE, cs.AI, cs.LO  
**Link:** https://arxiv.org/abs/2610.00885v1

> Coding agents increasingly automate Lean proof development, but successful compilation alone does not establish that a candidate proves the intended statement under acceptable assumptions. We present FORALL-LEAN-AGENT, a frontend-agnostic framework for auditable reasoning in formal mathematics and software verification. The framework combines isolated workspaces, Lean tools, and fresh review with statement comparison, axiom audits, and independent proof checking where supported. Verification evidence and reviewer decisions are bound to the same candidate artifact, making acceptance traceable. We evaluate the framework on VeriSoftBench, PutnamBench, and both problems in the Lean Eval softwareverification track. On the 100-task VeriSoftBench subset, integration with FORALLLEAN-AGENT raises benchmark-rule success from 93 to 100 for GPT-5.6 Sol at low effort while reducing cost from $69 to $62. The PutnamBench evaluation accepts all 672 problems at an average of $4.72 each. These results show that agent harness design can improve correctness and efficiency while providing evidence beyond aggregate solve counts.

---

## 137. Cogentic: Multi-Agent Orchestration for Automated Proof Discovery

**Autori:** Yang Cai, Vineet Gupta, Yanchen Jiang, Christopher Liaw, Aranyak Mehta, Grigoris Velegkas, Di Wang  
**Data:** 2026-09-30  
**Categorie:** cs.AI, cs.GT  
**Link:** https://arxiv.org/abs/2609.40324v2

> We present Cogentic, a multi-agent harness for automated proof discovery on open research problems. While frontier language models can generate strong mathematical ideas in a single shot, single-shot generation is often insufficient for open problems that require exploring multiple competing conjectures, overcoming subtle technical obstructions, and retaining intermediate progress over a long horizon. Cogentic addresses these challenges through an iterative prove-verify loop in which an orchestrator allocates a population of independent provers across distinct proof directions, subjects their output to adversarial verification by several specialized components, and promotes confirmed intermediate results into a persistent verified ledger that later rounds build on. The harness is designed to be able to solve research-level math and theoretical computer science problems. Using either Gemini 3.1 Pro or an early version of Gemini 4 Argon as the base model, Cogentic produced novel results on open problems across online learning, auction theory, and mechanism design. Each result was independently verified by domain experts and is developed in full in companion papers. We list these results, and new ones as they are verified, at https://sites.google.com/view/cogentic .

---

## 138. cua-speedrun: Standardized Benchmarking of the Speed of Computer-Use Agents

**Autori:** Pranjal Aggarwal, Lawrence Keunho Jang, Sean Welleck, Daniel Fried, Ruslan Salakhutdinov, Jing Yu Koh  
**Data:** 2026-09-30  
**Categorie:** cs.LG, cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2609.40284v1

> Computer use agents (CUAs), which use graphical user interfaces (GUIs) to complete tasks on a computer, have recently surpassed human performance on many standard benchmarks, including difficult long-horizon tasks. Their capabilities are undoubtedly impressive, however, a key barrier to the widespread adoption and deployment of CUAs remains their speed and cost. Progress towards faster yet capable CUAs requires reliable evaluation of their speed, but many CUA benchmarks currently face a reproducibility crisis. Benchmarks are based on complex infrastructure with varying machine and container configurations that confound the evaluation of the execution speed of CUAs. Towards addressing this gap, we propose cua-speedrun, which introduces standardized infrastructure and task sets, with a focus on evaluating the speed and efficiency of CUAs. cua-speedrun uses a uniform virtual machine setup and execution pipeline, along with a common agent interface that enables single-agent implementations to operate seamlessly across different benchmarks. Across four different CUA benchmarks, we evaluate how reasoning effort, agent harnesses, and environment latency affect performance, speed, and cost. We find no single model family is optimal for all three; none of the open-weight models are on the frontier, and also, unintuitively, for some models increasing the reasoning effort can speed up task completion, while faster environment input-output can slow down overall task completion time. We also demonstrate that we can effectively reduce the evaluation task set of most CUA benchmarks without degrading overall statistical power, allowing for more efficient benchmarking and comparison. We believe cua-speedrun will enable structured progress towards fast, efficient CUAs, unlocking new real-world use cases and applications. All code, infrastructure, and analysis are available at https://cuaspeedrun.com.

---

## 139. Learning from Research: Toward Lifelong Agent Harness Evolution

**Autori:** Jingbo Yang, Kwei-Herng Lai, Xiaowen Wang, Yaar Harari, Evgeniy Gabrilovich, Shiyu Chang  
**Data:** 2026-09-30  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.40169v1

> Language agents are expected to solve increasingly complex tasks, creating a growing need for continual improvement. One promising approach is to evolve the agent harness, the software that governs tool use, memory management, and task execution, while keeping the underlying language model fixed. Recent methods automate this process by using a meta coding agent to modify the harness based on execution feedback. However, relying on that agent's existing knowledge and observed failures can restrict exploration and make adaptation reactive. Inspired by how human experts learn from the research literature for new solutions, we introduce ScholarEvolve, a framework that automatically draws on state-of-the-art research to guide harness evolution. ScholarEvolve organizes the harness evolution directions into functional modules and uses topic modeling to identify distinct improvement strategies for each module. It implements these strategies and evaluates their combinations to improve task performance. Moreover, the framework is designed to incorporate new publications over time, allowing research advances to drive proactive lifelong evolution. Experiments demonstrate improvements on AppWorld and Tau2-Bench. ScholarEvolve raises Qwen3.5-27B task goal completion from 49.6% to 63.6% on AppWorld Challenge, and raises GPT-5.4-mini pass@1 from 72.7% to 81.9% on Tau2-Bench Telecom.

---

## 140. Better Deck or Different Judge? Evaluating Agentic Harness Gains in Corporate and Investment Banking

**Autori:** Ludovic Gibert, Matis Despujols, Andre-Louis Rochet  
**Data:** 2026-09-30  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.39958v1

> Corporate and investment banking teams use presentations to support credit decisions and advise clients on financing and transactions. Producing these decks requires reconciling financial data, tracing sources and turning analysis into a recommendation. We retrospectively study the development of an agentic harness combining a 27B language model, financial calculations, narrative templates and validation checks. LLM judges guide engineering changes and assess the resulting decks, raising the question of whether higher scores reflect better documents or changes in grading. In shared-session text-only grading with template markers removed, five judges score the complete system 20.4 to 33.6 points out of 95 above the same model generating directly from a short prompt. Every judge scores the system higher on all seventeen development deliverables. Margins against direct Opus generation from a short prompt range from -4.7 to +0.8 points. Judges agree on broad progress across development rounds but agree less on final-deck rankings than on pooled scores. Repeated grading also shifts scores on unchanged decks, making small improvements difficult to distinguish from judge variability.

---

## 141. OSWorld-Science: A Benchmark of Computer Use Agents for Learning and Using Scientific Software

**Autori:** Dingyuan Dai, Heli Qi, Lei Liu, Yinxi Li, Baiding Chen, Zijun Dou, Qingcheng Zeng, Qi Kang, Oliver Sun, Eric Wang, Bo Zhou, Haixin Wang, Yufan Du, Shi Bo, Ruihan Lin, Mengqi Yuan, Dunjie Lu, Steven Dillmann, Yiming Shi, Tina Su, Amy Xin, Minghao Liu, Xi Wang, Xu Huang, Ge Zhang, Pengyu Nie, Zhen Yang, Jie Tang, Juanzi Li, Weihao Xuan, Tianyu Liu  
**Data:** 2026-09-30  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.39903v1

> Scientific software presents a demanding test for computer-using agents based on visual language models (VLMs): completing a research workflow requires interpreting specialized interfaces, manipulating scientific objects, and producing verifiable results. We thus introduce OSWorld-Science, a benchmark and evaluation environment that combines scientifically meaningful tasks, artifact-based evaluation, and an efficient agent harness for studying computer use in the scientific domain. The benchmark contains 12 VLMs and 146 high-quality tasks across several scientific domains and software configurations, covering workflows such as molecular drawing and retrosynthesis, pathology image analysis, statistical computing, and physical simulation. Tasks are developed through expert proposals and iterative human--AI co-design, with selection guided by scientific value and difficulty. Task-specific execution-based evaluators inspect application states and generated artifacts, including molecular structures, segmentation masks, plots, and numerical results, and award partial credit for incomplete outcomes. Our special harness integrates model adapters, interaction-loop control, and trajectory logging to support comparisons of models and interaction strategies. Our results show that current state-of-the-art VLMs with a strong harness still face challenges in addressing key questions in the scientific domains. We also analyze the benchmarking results across multi-linguistics, reasoning efforts, context length and other factors and derive several important conclusions and directions to assist future development. Overall, we provide an integrated framework connecting expert-defined scientific goals to verifiable software outcomes, enabling systematic evaluation of both agent capabilities and harness design in scientific workflows.

---

## 142. Thinking Outside the Box: Can Language Models Rely on External Guidance Selectively?

**Autori:** Minghan Wang, Boyuan Wang, Jinhang Zuo, Yuxin Tao, Fang Kong  
**Data:** 2026-09-30  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2609.39578v2

> Agent harnesses often improve language models with human-designed workflows, but as models grow more capable, unreliable guidance can increasingly constrain their execution. We call the ability to benefit from useful guidance while overriding unreliable guidance thinking outside the box. We introduce Box$^2$-Bench, which holds the model and task fixed while varying workflow reliability to isolate how models regulate their reliance on guidance. On Box$^2$-Bench, frontier models often benefit from reliable guidance but remain vulnerable when it is misleading or becomes unreliable. To test whether this capability can be learned, we train two open-weight models using bad workflows, reserving good workflows for evaluation. We explore two complementary training strategies: counterfactual supervised fine-tuning improves robustness, while outcome-based reinforcement learning can shift the balance toward greater use of helpful workflows. We further find that this behavior extends beyond workflows to other forms of external information, improving peer correction and robustness to corrupted memory. Together, our results identify selective reliance on fallible external information as a dimension of agent reliability not captured by task performance alone.

---

## 143. Scale and Selection: What Makes Automatic Harness Evolution Work for Visual-Interface Robot Agents

**Autori:** Zhijie Wei, Ferris Tan, Jinghui Wang, Hao Zhou  
**Data:** 2026-09-30  
**Categorie:** cs.RO, cs.AI  
**Link:** https://arxiv.org/abs/2609.39304v4

> When an off-the-shelf coding agent is used directly as a robot policy, observing a browser-based 3D interface through screenshots and acting by posing a virtual target gripper through a few tools, the agent's harness, its prompts, tools, and control rules, largely determines success, and until now it has been written by hand. We show that this harness can be improved automatically by another coding agent, the optimizer agent, and report two findings about what makes it work. First, the number of rollouts the optimizer agent sees per round governs whether the evolved harness generalizes: with rounds fixed, held-out success rises as the training batch grows from 5 to 100 rollouts, while small batches overfit the training tasks. Second, the optimizer agent must not be given free rein. Accepting every revision it proposes degrades the harness within a few rounds; a simple Champion-Challenger rule that promotes a revision only if it beats the incumbent on the same fixed cases turns the same loop into one that raises held-out success on LIBERO tasks from 51% to 67% over 30 rounds. The evolved harness is also a natural place to attach a pretrained policy, through one tool that hands it control. Distilling the rollouts of that combination back into the policy with multi-teacher on-policy distillation yields a standalone policy at 62.2% on RoboCasa365 under the official protocol, 4.8 points above its starting point with no harness at inference; the evolved harness on top of the distilled policy reaches 71.2% on the RoboCasa365 leaderboard benchmark, 13.1 points above the best published entry, and the loop closes when harness evolution resumes on the stronger policy. Automatic harness evolution for visual-interface robot agents is thus feasible, but its gains hinge on the rollout scale behind each decision and on how the optimizer agent's revisions are selected.

---

## 144. Fyan: A Human--AI Harness with Semantic Auditing for Document-Level Formalization

**Autori:** Wei Zhao, Yangshuo Zou, Chengxiang Ding, Yifan Wu, Xuchuan Wang, Zimu Mao, Lei Zhang, Tao Luo  
**Data:** 2026-09-30  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.39228v1

> We present FYAN, a human--AI harness for document-level mathematical formalization. Rather than treating theorems in isolation, FYAN coordinates an end-to-end workflow spanning specification, proof planning, logical review, Lean proof construction, knowledge curation, and validation, with support for independent supervision and human guidance. A central component is evidence-grounded semantic auditing, which assesses whether formal statements faithfully preserve their informal specifications. A language model constructs structured evidence over local correspondences, omissions, scope, and logical relations, while a deterministic validator checks this evidence and produces reproducible judgments. When a substantive but admissible deviation is accepted, FYAN requires an explicit proof-transfer obligation connecting the formal statement back to a source-facing interpretation. With the same model (DeepSeek-V4.1-Flash) in every stage, FYAN proves 86 of 143 FormalTCS theorems under a strict Lean check, against 69 for a general agent harness, and raises the natural-language proof score from 0.501 to 0.851. On ConsistencyCheck, its semantic audit catches more inconsistent statements than a direct LLM judge, both on labels verified against the source (recall 0.777 vs. 0.636) and on the original labels (0.873 vs. 0.820), and localizes each mismatch it reports to a specific hypothesis, conclusion, or scope. FYAN also built ODENumLib, a 9,355-line Lean library for the numerical analysis of ordinary differential equation.

---

## 145. Schema: Discovering Unknown Environments via Agentic Program Induction

**Autori:** Guanning Zeng, Jiani Wang, Wenjie Ma, Shaofeng Yin, Chenyang Wang, Shichen Liu, Angjoo Kanazawa, Wode Ni, Xiuyu Li, Andrea Zanette, Haiwen Feng  
**Data:** 2026-09-30  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.39140v1

> Learning to complete tasks in unfamiliar environments with unknown rules remains a key challenge for LLM agents. Current LLM agents often record their discoveries in prose, which may not provide a compact, explicit account of how the environment works. Inspired by how scientists organize observations into testable, predictive theories, we introduce Schema, an agent harness that organizes learning and action through interactive program induction. The LLM agent decides what to investigate and how to act, expressing its evolving understanding of the environment as executable programs. The harness consists of a persistent program workspace and a small set of interfaces for checking these programs against the interaction history, planning within them, and executing plans under step-by-step verification. Schema raises ARC-AGI-3 RHAE from 58.7% to 99.2% with the same base model, solves 100% of the public DiG-bench games, and reaches the median performance of the top-50 human players on MazeBench. Extensive analysis shows the effectiveness of Schema in unknown mechanism discovery, and ablations confirm the contribution of each component.

---

## 146. Approval Laundering: Systematizing Approval--Execution Binding Failures in AI Coding-Agent Harnesses

**Autori:** Yang Wang  
**Data:** 2026-09-30  
**Categorie:** cs.CR, cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2609.38983v1

> Modern AI coding-agent harnesses (Claude Code, Codex CLI, Cursor) rest their security boundary on a largely unexamined assumption: that the action A a human approves is the same action A' the harness executes, where A is fixed by a stated policy for what a scope grant or session-scoped approval authorizes. We show this assumption fails systematically and reproducibly. We introduce Approval Laundering, a taxonomy of six failure modes by which a harness's enforcement mechanism silently substitutes A' for A after approval: Scope, Argument, Temporal, Tool, Delegation, and Semantic laundering. Unlike prior work that evaluates risk classifiers against static corpora or infers implicit authorization boundaries, we study credential-binding integrity: given an already-approved action, does the harness dispatch exactly that action? Instrumenting Claude Code's pre-execution mediation point (PreToolUse), we conduct a controlled, headless, repeated-measures study of all six classes (N=19-20 runs each), reporting a Bound-Gap Rate (BGR) with Wilson confidence intervals and inter-rater agreement (kappa=1.0). We prototype Approval Token, a keyed capability Hk(principal, agent_id, session_id, tool, arguments, scope, expiry) issued by a mediator that never returns the key to the agent, evaluated via paired before/after replay of 118 runs (McNemar's exact test). The token fully eliminates Delegation laundering and, for our seeded session-identity-mismatch construction, Temporal laundering (p<10^-5), but by design leaves Scope laundering unaffected and shows no significant reduction in Argument laundering (p=1): an honest negative result, since these two classes leave every recorded dispatch field unchanged, diverging one process level below what a field-only verifier can observe. We discuss implications for defenses that bind only at the tool-invocation boundary.

---

## 147. Composing Task-specific Agent Harnesses at Test Time with Reusable Primitives

**Autori:** Peng Kuang, Haibo Jin, Dehao Wu, Feiyang Deng, Xiaopeng Yuan, Jerry Wang, Haohan Wang  
**Data:** 2026-09-30  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.38912v1

> Agent harnesses govern how large language models (LLMs) gather context, invoke tools, verify results, preserve state, and terminate, largely affecting agent performance. However, the value of each harness mechanism can differ across heterogeneous tasks: a mechanism that improves one task may impose overhead or context distraction on another, leading to the suboptimality of a global harness. We characterize this suboptimality as a mismatch induced by fixed mechanism choices, motivating task-specific harness construction. Nonetheless, generating harness code for each task introduces generation and debugging costs, with execution risks that can compound as more mechanisms are generated. To address those challenges, we introduce Harness Primitives, reusable harness mechanisms with clear application scope and composition contract mined from failed task trajectories. Based on Harness Primitives, we propose STITCH, a framework that Selects suitable primitives given Task Information and compiles them into Task-speCific Harnesses at test time. This separation enables task-specific harnesses without generating or repairing mechanism code at test time. Extensive experiments demonstrate that STITCH not only improves harness adaptability and robustness, but also scales with the primitive library size, boosting task success rates by up to 12 points over fixed harness baselines, surpassing human-designed harnesses like Codex CLI while maintaining a minimal test-time harness composition overhead of only 2.7%, 638 times more efficient than generating task-specific harnesses from scratch. Ultimately, our work demonstrates that building task-adaptive harnesses can be beneficial for completing diverse tasks and that building reusable primitives can be a promising path towards this goal.

---

## 148. VidHarness: Evolving Agent Harnesses for Cost-Efficient Long Video Understanding

**Autori:** Susan Liang, Jianmin Wu, Daxiang Dong  
**Data:** 2026-09-29  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2609.38413v1

> Vision-language models (VLMs) can answer questions about hour-long videos, but processing every frame is prohibitively expensive, even though the evidence for a question usually spans only a few seconds. Video agents, i.e., harness programs wrapped around a frozen VLM, address this by observing the video selectively, yet existing harnesses are hand-crafted by experts through slow build-and-test cycles. We propose VidHarness, a framework that automates harness design for cost-efficient long video understanding, in which a harness proposer iteratively evolves harnesses based on execution feedback from an evolution environment. To escape the local optima of greedy refinement, we organize the evolution as Monte Carlo tree search (MCTS), and to reduce the evaluation cost, we integrate uncertainty-aware multi-fidelity validation, which screens new harnesses on a few questions and promotes only the promising ones. Since the best harness varies with the frame budget, we further introduce a mixture-of-harness that routes each question to a harness specialized for its budget. VidHarness sets new state-of-the-art results on LongVideoBench, Video-MME, and Video-Holmes, outperforms the strongest hand-crafted video agent by up to $11.2$ points, and generalizes to the knowledge-intensive benchmarks Video-MMMU and MMVU with fewer than half of the frames of uniform sampling.

---

## 149. MILO: Automated Harness Discovery via Orchestrated Multi-Agent Evolution

**Autori:** Prithwish Jana, Mononito Goswami, Hao Liu, Xinyu Li, Langlin Huang, Zhehui Huang, Zhishen Huang, Patrick Blöbaum, Anoop Deoras, Purak Jain, Nikos Kanakaris, Sahika Genc  
**Data:** 2026-09-29  
**Categorie:** cs.LG, cs.AI  
**Link:** https://arxiv.org/abs/2609.38349v1

> Modern agentic systems combine an AI model with a harness that controls execution and environmental interactions. Harness design strongly affects long-horizon performance, yet its combinatorial search space demands substantial human effort that must be repeated as models change. Existing automated methods explore this space narrowly, optimizing only components such as prompts or skills or becoming trapped by fixed, exploitative search strategies. We introduce MILO (Meta-evolutionary Island Orchestration), a framework that co-evolves agent harnesses and the strategy used to discover them. MILO combines: (i) hierarchical lineage memory over island-based trees, using rejected mutations as negative evidence; (ii) per-island mutator agents that rewrite complete harnesses using global search history and parent-specific feedback; and (iii) an orchestrator that adapts search through lineage grafting and speciation, mutator reassignment and curriculum revision. Across Terminal-Bench 2.1, PaperBench, and DeepSWE, MILO-discovered harnesses outperform eight state-of-the-art harnesses and six search methods using frontier (Opus 4.8) and open-weight (gpt-oss-120b) models. With Opus 4.8, MILO improves resolution over its initial harness by $+12.0\%$, $+28.3\%$, and $+10.3\%$, respectively, compared with best prior-search gains of $+4.5\%$, $+18.3\%$, and $0\%$. On Terminal-Bench 2.1, it achieves $86.1 \pm 2.0\%$, exceeding the official leaderboard's top entry ($83.8 \pm 2.3\%$) while using 26\% fewer tokens than its initial harness. On EinsteinArena open problems, MILO improves best-known upper bounds for Erdős minimum-overlap ($0.3808586 \to 0.3808568$) and the first and third autocorrelation inequalities ($1.50274365 \to 1.50274360$; $1.45081 \to 1.44889$).

---

## 150. Learning Meta-Skills for Agent Harness Design in Test-Time AI4AI

**Autori:** Cheng Qian, Kunlun Zhu, Beibin Li, Zhenhailong Wang, Heng Ji  
**Data:** 2026-09-29  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2609.38143v2

> Agent performance depends on both reasoning ability and the environment in which it acts. We study test-time AI-for-AI, asking how a Builder can learn to construct better execution environments for a Target while both models' weights remain fixed. To make the Builder's experience reusable, we introduce Meta-Skill: principles specifying when support is needed and what resources to provide. The Builder learns these principles from Target's execution feedback on the development set, then uses the frozen skill bank to construct harnesses for unseen tasks. Across Harness-Bench and NewtonBench, full-bank meta-skills improve macro-average performance by 8.95 percentage points over no-skill construction, and 12.02 points over direct delivery of the same bank to the Target. These results highlight the value of translating experience into executable support. Gains when the same model serves both roles further suggest a path to system level self-improvement through learning to build better environments.

---

## 151. HARDE: Optimizing Agent Harnesses for Runtime Risk Detection and Execution Control

**Autori:** Zhuo Liu, Moxin Li, Zhixin Ma, Wentao Shi, Wenjie Wang, Fuli Feng  
**Data:** 2026-09-29  
**Categorie:** cs.CR, cs.CL  
**Link:** https://arxiv.org/abs/2609.38291v1

> Large language model (LLM) agents are vulnerable to safety risks such as injected malicious instructions or misleading information, motivating runtime defenses that prevent unsafe action in execution across diverse risks while preserving benign-task utility. Existing system-level defenses either focus on risk detection rather than timely prevention or rely on predefined rules with limited flexibility across diverse risks. We propose a risk-aware harness that integrates LLM-based monitoring for flexible risk detection and structures monitor-guided execution around three core modules: trigger, monitor, and feedback, enabling targeted safety interventions while limiting disruption to benign task execution. To adapt the harness to different risks and deployment settings, we introduce HARDE, a two-stage harness optimization framework that first performs isolated probing of each module to derive an optimization guide, then uses this guide to iteratively optimize the harness based on safety and utility feedback. Experiments across three attack benchmarks show that HARDE improves runtime safety while preserving utility, outperforming manually designed harnesses and naive optimization baselines. Our analysis shows that effective runtime defense benefits from complementary safety mechanisms, attack-aware harness optimization, and harness designs matched to monitor capabilities. Our code is available at https://github.com/Liuz233/HARDE.

---

## 152. AgentBug-Smith: Automatically Reproducing Real-World Harness Bugs in Agentic Systems

**Autori:** Yiming Cheng, Alfin Wijaya Rahardja, Mengshi Zhang, Zihao Chen, Zhenpeng Chen, Yiling Lou  
**Data:** 2026-09-29  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2609.37864v1

> Agent harness bugs exhibit unique characteristics and remain challenging for state-of-the-art software agents to repair. Progress in this area is further hindered by existing benchmarks, which contain only a small and fixed number of executable harness bugs while requiring hundreds of human hours to construct. This work presents AgentBug-Smith, an automated harness bug reproduction approach that continuously discovers and reproduces real-world harness bugs from open-source agentic systems. Across different backbone LLMs, AgentBug-Smith consistently outperforms existing bug reproduction techniques designed for general software, achieving 10.67% - 27.56% higher success rates of reproducing harness bugs. By applying AgentBug-Smith to open-source agentic systems in the wild, we construct Live-Harness-Bench, a live and extensible benchmark that currently contains 200 reproducible harness bugs. We further demonstrate the utility of Live-Harness-Bench through two downstream applications. First, we use Live-Harness-Bench as the evaluation benchmark to systematically evaluate state-of-the-art software agents, revealing their limited capabilities in repairing real-world harness bugs. Second, we use Live-Harness-Bench as a knowledge base of real-world harness bug fixes, from which reusable repair skills can be distilled to improve existing software agents, increasing their harness-bug repair rates by 6.32%. Together, AgentBug-Smith and Live-Harness-Bench establish a scalable foundation for continuously evaluating and improving software agents on harness bug repair, turning real-world agent failures into executable evaluation instances and reusable knowledge for harness improvement, thus contributing to the ultimate goal of recursively self-improving agents.

---

## 153. Mixture of Self-Improving Branches For Agent Harness Optimization

**Autori:** Haoyu Dong, Yuhang Zhou, Zihao Lin, Yifan Wu, Bo Peng, Mingyi Wang, Xiangjun Fan, Lizhu Zhang, Zhuokai Zhao  
**Data:** 2026-09-29  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.37834v1

> Harness optimization provides a practical setting for recursive self-improvement (RSI), where agent-generated modifications inform subsequent changes through execution feedback. Recent work such as Meta-Harness implements this process through iterative code generation and evaluation, but retains a fixed development set and proposal policy. These constraints channel evolution along a single search trajectory, increasing the risk of converging to a local optimum. We make the improvement process itself adaptive by organizing search into branches with evolving development subsets and proposal policies. Each branch retains development cases solved by more of its leading harnesses than by those of other branches, drops cases solved by every leading harness across all branches, and revises its proposal policy using its own search history. To deploy the resulting complementary harnesses, we propose a router to select one development-selected branch head for each new input before execution. Across mathematical reasoning and agentic coding benchmarks, our system achieves relative improvements over Meta-Harness of 34.8% on Olympiad-level mathematical reasoning, 11.6% on Terminal-Bench 2.0, and 3.8% on SWE-bench Lite, with harness selection and router configuration based solely on development data. These results show that evolving branch objectives and proposal policies can yield complementary harnesses whose strengths a router combines without access to test outcomes.

---

## 154. Foundations of Proactive Agents: Principles, Technical Layers, and Proactivity-Gym

**Autori:** Jio Oh, Seunghyun Do, Young-Jun Lee, Steven Euijong Whang, Dongyeop Kang  
**Data:** 2026-09-29  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.37267v1

> Proactive LLM agents can turn idle compute into useful support before users ask. Yet even correct work can misread user context, impose review costs, or undermine trust. This work proposes foundations for designing, realizing, and evaluating proactive LLM agents around three joint principles (3T): Task Capability, anticipating relevant needs and correctly performing useful work; Temporal Allocation, allocating compute according to resource availability and when results are needed; and Trust, sustaining users' confidence and appropriate reliance on the agent. We connect these objectives to a design space organized around five dimensions: task scope, anticipation horizon, activation trigger, processing timing, and intervention depth, and specify the situation and system modeling needed to support its choices, including user and environment representations, backbone LLMs, and agent harnesses. Lastly, we propose PROACTIVITY-GYM, a simulation-based evaluation testbed including multi-day scenarios, stateful environments, and persona-conditioned simulated users that can evaluate the consequences of proactive assistance across interactions. Evaluations across 23 model-harness configurations uncover substantial performance gaps across 3T and reveal that LLM judges often conflate task capability and trust. A human study with 30 participants demonstrates the importance of the joint 3T optimization: participants show sharp trust declines after intervention misalignment despite correct outcomes, and prefer sleep-time assistance, even when imperfect, to preserve ongoing focus. Together, these findings support designing and evaluating proactive agents through the joint consideration of useful work, compute allocation, and evolving user trust.

---

## 155. WEFT: Scaling Tool-Use Post-Training for General-Purpose Agents

**Autori:** Bo Mao, Hang He, Linting Wang, Lizhi Lin, Maosen Zhou, Guanming Liu, Jinxiu Liu, Tianyu Huai, Chaoyun Zhang, Bingxuan Li, Kepeng Lei, Guanting Dong, Zhou Shao, Rui Zheng, Hang Yan, Jie Zhou, Chengcheng Wan, Tao Gui, Liang He, Xipeng Qiu  
**Data:** 2026-09-29  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.36887v1

> Recent efforts to scale tool-use post-training have largely centered on the synthesis of executable environments, which constitute only one component of a broader agentic interaction system comprising the environment, task, agent harness, and evaluator. Scaling environments in isolation, however, does not guarantee commensurate gains in model performance, because reliable learning signals depend on coherent interactions among all components of the agentic interaction system. To address this problem, we introduce WEFT (Whole-system Evolution For Tool-use Post-training), which couples scalable agentic interaction system construction, execution-driven self-evolution, and stable post-training. WEFT scales agentic interaction system construction across environment breadth, task complexity, and interaction diversity. Execution-driven self-evolution iteratively uses execution traces and state evidence to attribute failures and revise the responsible components, with fresh rollouts evaluating the changes and providing evidence for subsequent evolution rounds. For stable post-training at scale, WEFT addresses both optimization and execution reliability: prefix-preserving sampling retains verified progress and atomic-turn credit assignment localizes learning signals, while MegaMCP maintains isolated, recoverable state across concurrent rollouts over shared tool services. Extensive experiments across various models and benchmarks demonstrate the effectiveness of WEFT for tool-use post-training. WEFT-8B and WEFT-14B outperform all evaluated matched-size environment-scaling baselines on BFCL V4, $τ^2$-Bench, and Claw-Eval. In particular, WEFT-14B improves over Agent-World-14B by 6.41, 2.23, and 12.27 percentage points. WEFT-35B-A3B further extends these gains to more challenging long-horizon workflow benchmarks, including Toolathlon-Verified and AutomationBench.

---

## 156. S4VY: Segment Anything in Feed-Forward 4D Visual Geometry

**Autori:** Jingdong Zhang, Xin Li, Jan Kautz, Wenping Wang, Chris Choy  
**Data:** 2026-09-29  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2609.36875v2

> Accurate instance segmentation in dynamic scenes is important for downstream applications such as robotics and autonomous driving. Existing Segment Anything models operate primarily on 2D image or video masks and preserve identity through sequential memory, while promptable 4D instance segmentation built upon feed-forward visual geometry remains underexplored. We introduce S4VY, a Segment Anything model built on feed-forward 4D visual geometry. From a set of RGB observations, S4VY transforms shared visual-geometric features into an exhaustive set of class-agnostic 4D instance masks through a space-time query decoder, with each persistent object query binding one entity across all observations. This representation supports prompt-independent segmentation as well as point- and box- conditioned selection, without requiring a seed mask or temporal ordering. We further develop an agentic harness for natural-language grounding in the large observation space of a 4D scene. Active tree search identifies relevant frames without scanning every fixed window; a dual-stream grounder combines fine-grained VLM visual priors with geometry-consistent instance features through complementary bounding-box prediction and object-query matching; and an independent critic selects the final 4D instance mask from their predictions. Extensive experiments demonstrate state-of-the-art 4D instance segmentation and strong language-guided grounding performance under a unified evaluation spanning static and dynamic scenes.

---

## 157. AI as a Compiler: Compiling Triton kernels without the Triton compiler

**Autori:** François Costa, Charly Castes, Thomas Bourgeat, Azalia Mirhoseini  
**Data:** 2026-09-29  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.36800v1

> Compiler backends are expensive to build and maintain as programming models, workloads, and accelerators evolve. We investigate whether large language models can replace the conventional optimizing and lowering pipeline, a process that we call AI lowering. We study AI lowering from Triton to NVIDIA PTX: an LLM agent translates Triton kernels directly into PTX. We build an environment that evaluates candidate PTX, and an agentic harness in which an LLM translates Triton kernels into PTX. Across twelve common kernels on Ada, Hopper, and Blackwell GPUs and ten kernels from recent ML papers, AI lowering achieves 0.83x-3.34x the performance of autotuned Triton. The largest gains come from transformations that Triton's lowering pipeline does not perform, such as decoding packed binary weights directly into Tensor Core operands (3.34x on BitDelta), assigning each thread a complete softmax row in tensor memory (1.37x on FlashAttention), and reusing overlapping convolution windows (up to 2.23x). These results rely on a robust evaluation harness with comprehensive verification support. We build on Volta, an existing PTX verifier, and substantially extend it to support modern GPU architectures by introducing support for Blackwell's tcgen05 Tensor Core interface. This requires modeling three architectural features: managed tensor memory, descriptor-based operand layouts, and asynchronous execution coordinated through commits, waits, memory barriers, and proxy fences. We discuss the challenges involved in formalizing them, as well as the current limitations. Our results suggest an emerging future in which AI compilers replace custom-written intermediate representations and checkers, reducing the time and engineering effort required to bring up software for new general-purpose and custom chips.

---

## 158. Gödel Forest: Balancing Search Depth and Breadth for Data-Centric Recursive Self-Improvement

**Autori:** Ziqi Zhao, Fanqing Meng, Haocheng Lu, Lingxiao Du, Qiguang Chen, Mengkang Hu, Xiao-Ming Wu  
**Data:** 2026-09-29  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2609.36675v2

> Recursive self-improvement (RSI) aims to achieve compounding gains by having models improve themselves. While most existing RSI systems optimize external agent harnesses or prompts around a frozen base model, data-centric RSI directly updates the model's own parameters by training on agent-generated data. However, because validating data strategies requires expensive model training, existing methods face a fundamental dilemma: a single agent gets trapped in narrow directions and lacks exploration breadth, while naive parallel search or heavy trace sharing sacrifices long-horizon search depth. To address this challenge, we introduce G"odel Forest, a multi-agent framework that organizes recursive self-improvement as an ensemble of co-evolving search trees. In G"odel Forest, each agent autonomously grows a persistent tree, deepening, branching, or pruning data strategies based on model feedback to secure depth, while parallel trees explore distinct regions of the data space to expand breadth. Crucially, rather than leaving trees isolated or flooding them with heavy execution logs, a dynamically co-evolving memory connects the forest: agents continuously distill their successes and failures into compact procedural lessons anchored to a global leaderboard. Through this forest ecosystem, a dead-end in one tree instantly warns the whole forest against unpromising paths, while an empirical breakthrough quickly seeds new exploration branches in neighboring trees. Evaluated on RSIBench-Data across six diverse domains, G"odel Forest outperforms the single-agent baseline by an average of 10.70% while reducing wall-clock time on five tasks. Ablations confirm that co-evolving shared memory yields a +7.00% gain over independent parallel search, demonstrating that collective distillation is key to scalable self-improvement. The code is available at https://github.com/evolvent-ai/Godel-Forest.

---

## 159. Planarian: Managing Agent State with Statepoints

**Autori:** Jinnan Guo, Hao Mark Chen, Kapil Vaswani, Andrew Paverd, Peter Pietzuch  
**Data:** 2026-09-28  
**Categorie:** cs.OS, cs.AI, cs.CR  
**Link:** https://arxiv.org/abs/2609.35366v1

> LLM agents solve complex tasks by iteratively changing files, invoking local tools, and interacting with remote services, which modifies state across their local environment and remote services. Today, agents and users must manage these changes explicitly, whether reverting exploratory actions or recovering from erroneous ones. Doing so safely requires coordinated actions, yet current agent harnesses lack unified abstractions and mechanisms for managing local and remote state consistently and efficiently. We describe Planarian, an agent runtime with state management that enables agents and users to recover from erroneous actions and explore alternative executions over consistent local and remote environment state. Planarian introduces the abstraction of agent statepoints, which are consistent, restorable point-in-time versions of the environment state. Planarian exposes three state-management primitives to agents and users: (i) snapshot creates a new statepoint spanning local and remote state without requiring external services to support checkpoints: it relies on efficient incremental process and file system snapshotting to capture local sandboxed state, and transparently records compensating actions to undo remote state changes; (ii) rollback restores the environment to a previous statepoint by reverting to a prior local checkpoint and replaying compensating actions for remote state changes; and (iii) fork creates multiple isolated branches from a statepoint, enabling the agent to explore alternatives in parallel. We show that Planarian enables agents to undo mistakes and explore alternatives in parallel, improving task quality by up to 15x, and allows users to recover from erroneous actions with only 3% overhead.

---

## 160. Timeline-Bench: Evaluating Agents on Realistic Video-Editing Tasks, from Raw Footage to Final Cut

**Autori:** Gunin Gupta, Nirmit Arora, Pavan Kalyan Tankala  
**Data:** 2026-09-28  
**Categorie:** cs.CV, cs.AI, cs.MM  
**Link:** https://arxiv.org/abs/2609.35143v1

> AI agents increasingly carry out long-horizon professional work, but their evaluations rarely require a finished creative deliverable. To this end, we introduce Timeline-Bench, a benchmark of 56 real video-editing tasks, each asking an agent to turn raw production material into a finished video. Tasks range from selecting dialog takes and shaping interview footage into a story to cutting commercials from product shots, voiceovers and graphics. Every task provides a brief, source assets, a container and a set of tests. A task is resolved when the output passes every test. The tests check the delivery format, the content and the brief's explicit requirements, and include a quality test calibrated on 2,582 blind judgments by 43 video editors. We evaluate 16 agents that pair frontier models with coding-agent harnesses such as Codex, Claude Code and OpenCode. The best, GPT-6 Astra in Codex with curated editorial guidance, resolves only 15 of the 56 tasks (26.8%), and the average agent resolves 14.0%. Human editors prefer the reference edit in 83.5% of judgments. Most unresolved runs (562 of 771) fail only the quality test: agents perceive footage through stills and transcripts and check their renders for defects, not craft. We release the tasks, verifier and per-run results at https://timelinebench.tensortest.com.

---

## 161. Beyond Skill Evolution: Self-Evolving Context Management Policies for Long-Horizon Agent Harnesses

**Autori:** Weiyuan Li, Jinghan Xu, Aili Chen, Xintao Wang, Shuang Liang, Jiaqing Liang, Deqing Yang  
**Data:** 2026-09-28  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.34649v1

> Harness evolution improves LLM agents by learning from execution trajectories, but existing experience- and skill-based methods are less effective on long-horizon tasks. As interactions grow, useful evidence can be buried by redundant or outdated context, making context management itself a key bottleneck. We introduce ContextEvo, a framework that learns a context policy from long-horizon trajectories. ContextEvo reconstructs the model-visible context at key decision points, identifies context-related failures, and applies targeted policy updates. Starting from the open-source Pi-agent harness, ContextEvo improves performance across three long-horizon task benchmarks, achieving results comparable to or better than several prominent agent harnesses, including Codex, OpenCode, and OpenClaw. Additional analyses show that fixed or locally evolved context strategies can fall short under long-horizon information pressure, while our methods adapt to the information demands of each environment.

---

## 162. GenMem: Generative Symbolic Memory for Self-Evolving Harness

**Autori:** Xinke Jiang, Tao Feng, Weixuan Xu, Zhixin Zhang, Zhibang Yang, Wentao Zhang, Runchuan Zhu, Xu Chu, Junfeng Zhao, Yasha Wang  
**Data:** 2026-09-28  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2609.34633v1

> Long-term memory supports the self-evolution of LLM agents by retaining experience and skills across tasks and enabling their retrieval, reuse, and revision in subsequent long-horizon decision-making. Yet existing memory management approaches remain limited to discriminative retrieval and to address the sparse, hierarchical, and highly redundant structure of reusable experience: only a small, task-dependent subset of trajectories and memories warrants retention, retrieval, or revision. Learning these operations is further complicated by sparse, delayed, and indirect task-level feedback, with weak supervision across the memory lifecycle. Moreover, continual memory evolution introduces an architectural tension as addressing invariance: stored experience is perpetually revised, yet the addressing interface consumed by learned retrieval policies must remain stable. To address, we present GenMem, which reformulates memory management as generative symbolic addressing. Its core mechanism is the Symbolic Identifier (SID), a multi-level discrete token tuple drawn from a Cartesian-product address space that factorizes a million-scale sparse memory space using fewer than one hundred discrete symbols. Instead of generating ever-changing raw content, the memory agent learns to generate SIDs, while memory evolution rewrites the payload at a fixed address without shifting the address itself. Architecturally, GenMem couples a MemRetriever and a MemEvolver within a multi-agent harness, trained via GRPO with dense process and outcome rewards with two-channels optimization. Under offline memory evolution, experiments spanning ALFWorld, WebShop, multi-hop QA, medical reasoning, and deep research evaluate GenMem against strong memory-augmented baselines...

---

## 163. GlyphBench: A Playground for Language-Model Reinforcement Learning

**Autori:** Roger Creus Castanyer, Marc-Alexandre Côté, Matthew James Sargent, Augustine N. Mavor-Parker, Glen Berseth, Pablo Samuel Castro  
**Data:** 2026-09-28  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.34214v1

> We introduce GlyphBench, an environment suite for reinforcement learning (RL) post-training of language-model agents, with over 360 tasks spanning diverse games. GlyphBench renders spatial observations as two-dimensional Unicode grids and connects training, evaluation, and trajectory replay through a unified interface designed to support efficient and reproducible research. We use GlyphBench to study how observation interfaces, reasoning effort, and agent harnesses affect performance, and how RL configurations shape learning dynamics. Our results show that glyph observations outperform native text and pixels in our Craftax experiments, with further gains on several BALROG environments. RL on 100 GlyphBench tasks improves Qwen3.5-4B on held-out Reasoning Gym problems, reaching 63.48% accuracy and outperforming the base model, a math-trained baseline, and a code-trained baseline. These experiments provide empirical evidence that reasoning gains from gameplay can yield stronger transfer than math or code. Together, these results highlight GlyphBench's value as a testbed for systematic research on how language-model agents learn, interact, and generalize.

---

## 164. Towards Certificate-Driven Software Porting: A Self-Improving Agentic Harness for Scientific Program Optimization

**Autori:** Piyush Jha, Aishik Ghosh, Vijay Ganesh  
**Data:** 2026-09-28  
**Categorie:** cs.AI, cs.PL, cs.SE  
**Link:** https://arxiv.org/abs/2609.34069v1

> The upgrade and rewriting of large scientific codebases has traditionally been a major challenge. While evolutionary search with large language models (LLMs) can port and accelerate legacy code, repair feedback in prompts alone does not prevent subsequent candidates from repeating the same errors. We introduce Certificate-Driven Evolutionary Search (CDES), which extends evolutionary search with enforceable restrictions derived from failed candidates, recorded as certificates of assumptions, checker evidence, and justified restrictions. Its control logic enforces these restrictions through rejection, backtracking, and targeted repair while preserving compatible edits. We apply CDES to CPU-to-GPU translation of two particle-simulation functions from the Geant4 toolkit, evaluated with a harness that goes beyond unit tests to combine formal checks, numerical comparisons, physics checks, and GPU safety tests. Generated implementations achieve 13.78x and 23.54x function-level speedups over CPU code, including data conversion and transfers; for one function, GPU throughput exceeds an expert implementation by 14.9%, reaching 16.1% when complementary components are combined. In an ablation over execution settings, certificate feedback increases the fraction of candidates passing required correctness checks from 55% to 90%.

---

## 165. Vestrum: Improving Agent Harnesses by Adapting Their Verification, Structure and Memory

**Autori:** Jayant Parashar, Eugene F. Douglass, William C. Bastian, Suchendra M. Bhandarkar  
**Data:** 2026-09-27  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.33822v1

> An agent harness controls how a language model accesses information, uses tools, preserves memory, and checks its work. Improving this software is costly when each evaluation requires a long interaction with an environment. We introduce Vestrum, a framework that turns failures in execution traces into scoped harness changes without training the task model. Its organizing overhypothesis is that tasks of a shared kind may exhibit recurring failures whose remedies transfer within that kind. Vestrum expresses failures as recognizable classes, proposes changes across verification, retrieval, decomposition, and knowledge synthesis, and screens their scope before evaluating them as a bundle. A persistent lessons file informs subsequent proposals. Across five settings and two baseline harnesses, the frozen harnesses improve held-out performance: UltraHorizon rises from 47.6 to 59.8 over GAM, Terminal-Bench 4 Hard from 63.7% to 70.3% of checks passed over Claude Code on eight held-out tasks at 1.03x test cost, and cell-type annotation agreement from 67.5% to 77.8% on held-out sections of one slide, alongside gains on LoCoMo and AMA-Bench. Across our searches, verification grounded in evidence helped both intermediate steps and final answers, at lower cost at intermediate steps, while critics asked to rebuild finished answers broke more than they repaired. On the three memory benchmarks, Vestrum also scores above the evaluated GEPA configurations in every paired evaluation.

---

## 166. SecProbe: Adaptive Evaluation of Coding Agents on Cybersecurity Vulnerabilities

**Autori:** Xiaonan Luo, Yue Huang, Kehan Guo, Ping He, Chuan Zou, Chujie Gao, Lichi Li, Yuchen Ma, Zhangchen Xu, Zichen Chen, Yufei Han, Xiangliang Zhang  
**Data:** 2026-09-27  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2609.33763v1

> Assessing cybersecurity vulnerability awareness in coding agents requires evaluations that reveal capability gaps and remain informative as models evolve. Static benchmarks offer fixed coverage and difficulty, while scarce vulnerable repositories and costly expert authoring limit their renewal at scale. We introduce SecProbe, a framework for adaptive evaluation that combines Item Response Theory (IRT) with on-demand synthesis of repository-scale vulnerability-repair tasks. From observed performance, \textsc{SecProbe} estimates agent ability and identifies where additional evidence is most informative, selecting existing tasks or synthesizing new ones accordingly. As one use case, we construct 353 tasks spanning six programming languages and 151 CWE types and evaluate nine frontier models with two agent harnesses. Success rates peak at 28.33\%, highlighting substantial gaps in vulnerability recognition and repair. Compared with random and one-shot baselines, \textsc{SecProbe} achieves comparable agent ability estimates while requiring agents to solve up to 29.5\% fewer tasks. These results support adaptive evaluation as an efficient and discriminative approach to assessing cybersecurity vulnerability awareness.

---

## 167. Long-Horizon Analog Design Bench: Benchmarking Agents on Hours-Long Analog and Mixed-Signal Circuit Design Tasks

**Autori:** Analog Design Bench Team  
**Data:** 2026-09-27  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.33356v1

> Coding agents now sustain hours-long, tool-driven loops, yet their ability to carry long-horizon analog and mixed-signal circuits to electrical specification remains unmeasured. We introduce Analog Design Bench, a long-horizon agentic benchmark of 50 transistor-level design tasks contributed by 17 chip designers. Agents work with an open-source simulator, while an isolated verifier evaluates the submitted circuit using specification-based electrical tests. We evaluate 15 agent configurations across 2,250 two-hour attempts and observe full-specification pass rates from 8.0% to 78.0%. Coding-benchmark performance correlates with analog results but leaves much of the performance spread unexplained. Our failure analysis shows that most unsuccessful submissions have no recorded legality rejection but fail electrical acceptance, identifying electrical closure as the dominant endpoint challenge. We test time, reasoning effort, agent harness, and supplied design knowledge as interventions. Longer budgets and higher reasoning effort improve performance, while general skill documents provide little benefit and sometimes reduce performance. Supplying a task-matched reference topology, an idealized form of circuit-IP retrieval, raises DeepSeek V4 Pro by 18.7 percentage points and mainly accelerates GPT-5.6 Sol.

---

## 168. Compositional Safety Failures in Harness Evolution: Identification and Runtime Monitoring

**Autori:** Zhixiang Zhang, Zesen Liu, Wai Ip Lai, Hongxu chen, Dongdong She  
**Data:** 2026-09-27  
**Categorie:** cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2609.33123v3

> Self-evolving agent harnesses continually update persistent components such as memory, prompts, skills, and tools. We call this process harness evolution. However, such evolution could introduce unexpected safety risks. Existing work studies harness misevolution and validates candidate harnesses or attributed individual component updates, leaving safety analysis of cross-component update interactions largely unexamined. To address this gap, we study compositional safety failures in harness evolution, where interactions among individually safe and utility-preserving component updates can produce undesirable or unsafe agent behavior, revealing a safety risk intrinsic to harness evolution. Across three safety-related benchmarks, we identify 43 pairwise and 18 irreducible 3-way compositional safety failures. Conventional solution incurs combinatorial complexity in validating cross-component interactions, leaving the safety checking impractical as the harness evolves. To solve this, we introduced a typed hypergraph that represents component states as nodes and safety-relevant higher-order interactions as hyperedges. When the harness changes, the hypergraph updates only the interaction neighborhood of the changed states rather than reconstructing the global composition space. Building on that, we develop a hypergraph-guided runtime monitoring mechanism. Experiments show that our method effectively mitigates compositional safety risks while preserving task utility and reducing interaction-checking costs, and further reveal an empirical safety-utility-cost trade-off across different safety mechanisms.

---

## 169. Beyond Token Savings: A Systematic Study of Context Compression in LLM Agents

**Autori:** Ritul Satish, Prasoon Sinha, Akiho Kawada, Neeraja J. Yadwadkar  
**Data:** 2026-09-26  
**Categorie:** cs.LG, cs.AI  
**Link:** https://arxiv.org/abs/2609.32961v1

> As LLM agents tackle longer tasks, they increasingly compress growing histories of reasoning, actions, and tool outputs. Compression can reduce token use, but it also changes the information available for later decisions. Existing agentic harnesses bundle decisions about what to compress, when to compress, and how much to remove into fixed policies. A systematic characterization is needed to disentangle these decisions and reveal how each affects task success and execution cost. We systematically vary these decisions across three open-weight models on SWE-bench Verified and Terminal-Bench 1.0. Across nearly 35,000 agent runs, we measure task success, token use, end-to-end latency, and estimated cost. We find that fewer tokens need not mean faster or cheaper execution: on Terminal-Bench with Qwen, policies using roughly one-third as many tokens can take 20-80% longer than the uncompressed agent. Policies with similar overall success can solve different tasks, while the same policy can perform quite differently across models. Our results motivate evaluating compression by its effects on agent execution and tailoring policies to the task, model, and workload.

---

## 170. Hearsay: Can an Auditor Trust the Record a Deployed Agent Harness Writes?

**Autori:** Jiahong Dai, Zhuochen Yang, Pengyang Shao, Kelvin Ng, Zhongyi Liu, Chengquan Ju, Yuting He, Bo Hu  
**Data:** 2026-09-26  
**Categorie:** cs.CR, cs.AI, cs.CE, cs.SE  
**Link:** https://arxiv.org/abs/2609.32495v1

> An agent harness, the code that turns a model into an agent, writes its own record of each run, and that record is all a later reader gets when a run is disputed, investigated or audited. We call a record evidentiary when a reader who was not there can check it without trusting the writer. Across sixteen deployed frameworks, none writes one in full. Hearsay examines the record, not the task: five harnesses run fourteen tasks, three blinded LLM examiners and a human panel read the records, and every excerpt an examiner quotes is checked mechanically for who wrote it. First, the record lets a reader name the fault but not prove how the run went. Examiners name the right fault in 74 to 91% of 140 runs, but the fault can be proved only from two files the benchmark adds; for what happened in between, fewer than one citation in ten lands on anything the harness did not write, and the examiner with the fewest false alarms catches half of the entries we delete, rewrite or fabricate. Second, the remedy is a second author, not a stronger seal on the first. An append-only log of what passes between harness and model, kept outside the harness and read against the record in both directions, reports all 28 omissions and fabrications we made a harness commit as it ran, where a hash chain over the harness's own record passes all 28. Handed the log, examiners keep their fault verdicts but rest more of their citations on what the harness did not write. What makes a record evidence is who writes it, not what is captured.

---

## 171. PluginRSI: Recursive Improvement of Agent Harnesses with Reusable Plugins

**Autori:** Yaorui Shi, Yuchun Miao, Yuxin Chen, Jiayuan Zhang, Yueqing Sun, Xierui Song, Xiang Wang, An Zhang  
**Data:** 2026-09-26  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.32423v2

> The harness surrounding a language model is a central determinant of agent performance. Recent methods optimize harnesses by searching over complete programs, where individual mechanisms are difficult to isolate and reuse. We introduce PluginRSI, which represents a harness as a composition of atomized plugins and organizes harness evolution around these plugins. Individual plugins are improved independently and accumulated in a shared library, then recombined into new harnesses at each iteration. PluginRSI improves over existing harness optimization methods across software engineering, command-line interaction, and question-answering tasks. The resulting harnesses retain their advantage when transferred to other solver models without further optimization. The evolved plugin library accelerates subsequent optimization from the initial harness, which helps faster and higher convergence on unseen tasks. These results show that accumulating reusable mechanisms provides an effective basis for continued harness improvement.

---

## 172. SCLATE: a Substrate for Continual-Learning Agent Training and Evaluation

**Autori:** Youngmok Jung, Sirajul Salekin, Henry Tran, Javier Movellan, Zhao Huang, Manjot Bilkhu  
**Data:** 2026-09-26  
**Categorie:** cs.AI, cs.DC, cs.LG  
**Link:** https://arxiv.org/abs/2609.32391v2

> Continual-learning agents are systems of models, harnesses, and memory operating over long multi-session horizons. Evaluating and training them requires interleaving tasks with agent-side events such as session stop and start, crons, and memory consolidation. Yet existing benchmarks and training frameworks schedule only the benchmark's own events, leaving each benchmark and agent pair to build a custom scheduling loop. We present SCLATE, an execution substrate where benchmarks and unmodified agents each add their events to one open event scheduler through an adapter. A hybrid simulated clock runs these events on a shared timeline, flowing in real time while the agent works and skipping idle gaps, which compresses a month-long scenario into hours. SCLATE also serves as a rollout engine that runs any agent's harness and memory unmodified, recording the tokens and log probabilities of every model call through an in-container proxy. We port seven benchmarks to SCLATE and compare ten unmodified harness and memory configurations head to head on ten models. The comparison shows that an added memory system does not reliably beat the harness's native memory and that models differ widely in how they use the same harness and memory. We then post-train Qwen3.5-4B through unmodified harnesses and memory systems. The model learns to use both, reading 6.8x fewer file lines with a 16.7-point higher SWE-bench Verified pass rate, and writing richer memory records, while its held-out MetaClaw accuracy rises by up to 11.8 points.

---

## 173. Measurement Boundaries in LLM Financial Agent Evaluation: Fixed-Tape Execution and Multi-Defect Auditing

**Autori:** Weicheng Xue  
**Data:** 2026-09-26  
**Categorie:** cs.LG, cs.AI, cs.CE, cs.SE  
**Link:** https://arxiv.org/abs/2609.32379v1

> What controls are needed to interpret execution performance and audit scores in LLM agent evaluations? We study two limits on these interpretations in a financial agent harness. In Study~A, comparing independent runs under idealized and stressed execution on three synthetic settings that share one 24-day upward phase mixes the execution rule with fresh model responses and portfolio feedback: the parsed decision paths agree in only $19.8\%$ of $450$ pairs. Replaying each stored response tape through both execution destinations gives a narrower result. Conditional on those responses, stressed execution changes total return by $-0.0170$ (95\% interval $[-0.0230,-0.0117]$), or $10.4\%$ of the idealized baseline, and ten seed clusters do not resolve the model ranking. Study~B corrects an incomplete answer key and replaces legacy tasks with matched zero-, one-, and two-defect tasks under an explicit multi-label prompt. The drop in target violation recall from one to two defects is positive in five of six combinations of auditor and source (median $0.267$), with three surviving Holm correction. Yet the auditor that includes both target labels most often has micro-precision $0.149$, emits findings on $98/100$ zero-defect tasks, and returns the exact dual-defect set in only $21/100$ cases. Target recall by itself therefore gives a poor account of audit quality on this construction. The studies address different limits: what an execution comparison estimates, and what target recall captures. Together, they show how fixed conditions and diagnostic controls bound the claims a score can support.

---

## 174. Omni-IO Skills: Harnessing Your Agent Omni-Native

**Autori:** Yanlin Li, Mingyang Hao, Shengqiong Wu, Hao Fei, Mong-Li Lee, Wynne Hsu  
**Data:** 2026-09-25  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2609.31847v1

> General-purpose agents can plan, reason, and act over long horizons, yet their production capabilities remain fragmented across text, images, audio, video, documents, 3D assets, and code. Extending a foundation model to additional modalities ties capability growth to costly model updates, while assembling specialist models and tools leaves unresolved how procedures, dependencies, intermediate assets, and cross-turn revisions should be coordinated. We present Omni-IO Skills, a plug-and-play Agent Harness that makes existing agents omni-native through hierarchical Skills, a standardized multimodal execution interface, dependency-aware orchestration, and a persistent Asset Registry. Multi-asset workflows are represented as Declare Execution Graphs, which schedule independent operations concurrently and register successful outputs for downstream and cross-turn reuse across replaceable execution backends. Its 27 Skills cover 38 representative tasks spanning seven artifact modalities and four capability families: understanding, generation, reasoning, and retrieval. On UniM-90, the harness raises the input-support rates of GPT-5.6 Sol and Claude Sonnet 5 from 40.00% and 38.89% to 100%, while increasing relative Semantic--Quality Coupled Score from 26.99 to 74.94 and from 27.82 to 77.78, respectively; Strict Structure Score reaches 100.00 and 99.78. These results establish harness-level capability composition as a practical route to broad, evolvable Omni systems without changing the host agent's reasoning core.

---

## 175. DynBranch: Speculative Subgraph Reuse for Dynamic Agentic LLM Serving

**Autori:** Junyi Shen, Noppanat Wadlom, Zhengyuan Su, Yao Lu  
**Data:** 2026-09-25  
**Categorie:** cs.DC, cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2609.31047v1

> Agentic LLM workflows decide their execution paths at runtime. Downstream computation may be predictable, or may have run before, yet it cannot begin until the model or the user resolves the branch. We call this serialization the branch-resolution barrier. Caching alone does not hide it: the key that identifies a reusable result is not known until then. In this paper, we propose DynBranch, which makes an unresolved branch addressable before it resolves. Its stable coordinate lets candidate subgraphs run during resolution and completed subgraph results be reused across later requests. A two-level controller admits this work when its expected benefit exceeds the load price. DynBranch sits at the model-API boundary and requires no changes to agent harnesses or model execution engines. Across four agentic workloads with Qwen3-32B on 4x H200 GPUs, DynBranch reduces mean latency by up to 32% over each workload's strongest prior system and by 46-66% against a no-reuse floor, while preserving workflow results. The benefit persists across backbone families and on a commodity Qwen3-8B/RTX 4090 deployment.

---

## 176. MammoClaw: Towards Skill-Evolving Agent Harness for Breast Cancer Mammography Analysis

**Autori:** Krishna Kanth Nakka  
**Data:** 2026-09-25  
**Categorie:** eess.IV, cs.CV  
**Link:** https://arxiv.org/abs/2609.31789v1

> In this work, we explore MammoClaw, a training-free agent framework that leverages frozen MLLMs for mammography analysis. To support agentic investigation, we equip the agent with lightweight mammography-specific tools for targeted image analysis, including ROI, paired-view, and contralateral-breast examination. MammoClaw iteratively gathers evidence through these tools, while skill evolution enables non-parametric adaptation by transforming failed trajectories into reusable guidance for later runs. We evaluate the framework on BI-RADS assessment and breast density estimation tasks. In our experiments, we find that tools alone do not reliably improve performance, whereas evolved skills can improve tool-use behavior and performance in some settings. Beyond these results, MammoClaw enables transparent inspection of evidence acquisition, tool interactions, and failure modes, facilitating the analysis and auditing of agent behavior. We view this work as an exploratory study of training-free, self-evolving agentic approaches for mammography and hope it provides a concrete starting point for future work on mammography-specific tools and self-evolution mechanisms. We release our code at https://krishnakanthnakka.github.io/mammoclaw.

---

## 177. World Action Agent: Harnessing VLMs for Robot Manipulation via World Action Rehearsal

**Autori:** Yehang Zhang, Haojian Huang, Yifan Chang, Jianchong Su, Bohan Zhou, Yingjie Xu, Wosong Chen, Tianhao Zhou, Chenxu Wang, Tianyi Zhang, Yangkai Wei, Wenqian Li, Shiyuan Deng, Yinchuan Li, Ying-Cong Chen, Zexi Li  
**Data:** 2026-09-24  
**Categorie:** cs.RO, cs.AI  
**Link:** https://arxiv.org/abs/2609.29964v1

> General-purpose vision-language models (VLMs) bring broad knowledge and spatial reasoning to robot manipulation, yet existing systems either use them indirectly, to predict constraints or write programs, or give them a view of the scene rather than a world in which to act. We present World Action Agent (WAA), a multi-agent harness through which VLMs pilot robots with basic tools, making every decision within a visual action workspace. The workspace has three properties. Contact views, selected automatically from the scene geometry, present the scene around the current interaction. Action rehearsal turns each action into an editable proposal that the agent, alone or through an Imagination Agent, previews and revises against planning feedback before execution. In-view correction closes the loop between observation, rehearsal, and low-level execution, letting the agent remove residual offsets in the view where it observes them. Through the same workspace, WAA acquires embodied procedural knowledge in two ways: it evolves multimodal skills from expert videos and human teaching under evidence-based review and consults them through a Skill Agent, and its interaction traces train smaller VLMs to pilot the same harness. On LIBERO-Pro, WAA with skills evolved only from LIBERO-90 reaches a state-of-the-art 75.6% average success, outperforming end-to-end VLAs, code-as-policy agents, and a visual-harness baseline with the same backbone; the same skills remain effective on robosuite without further learning. Fine-tuning Qwen3.5-9B on harness traces raises its out-of-domain success from 1.7% to 43.3%.

---

## 178. Where Does Exactly-Once Live? Model, Harness, and Tool-Contract Effects on Duplicate Side Effects in LLM Agents

**Autori:** Jiapeng Li  
**Data:** 2026-09-24  
**Categorie:** cs.LG, cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2609.29095v1

> When a tool-using agent's write times out or returns a server error, the action may already have taken effect. Retrying blindly duplicates it -- a second charge, a second announcement, a second deployment -- while giving up skips required work. We ask where exactly-once behaviour should be enforced: in the model, in the agent harness, or in the tool contract. We introduce LIMBO, a deterministic sandbox of six services with realistic contracts (optional idempotency keys, eventually consistent and missing read paths) and twelve fault modes injected at the service boundary, including late commits, redelivery and partial batches; every episode is graded against a ledger of committed effects. Across 25,930 episodes spanning nine recent models, three production agent harnesses, two contract variants and fifteen recovery conditions, the answer depends on the fault. When an immediate read-back can reveal what happened, the model decides: frontier models instructed to act exactly once almost never duplicate a write whose acknowledgement was lost (0.5%), weaker models often do, and the model explains 53% of the explained variance. When it cannot -- the request is still in flight, or the transport delivered it twice -- the same frontier models duplicate in 56% and 74% of episodes, and the contract explains 81%. We prove that no verification-only policy is exactly-once under late commits without a bound on in-flight time. Waiting works when such a bound is short and known, but with heavy-tailed in-flight delays even an hour of waiting per episode falls short of offering an idempotency key on every write, which lowers the duplicate rate from 28% to 4% because agents use keys when they exist. The harness barely matters, a guard that attaches keys transfers across harnesses unchanged, and agents reported success in 90% of the episodes in which they had duplicated an effect.

---

## 179. Who Is Behind the Harness? Fingerprinting LLMs through Agentic Behavior

**Autori:** Chuyi Wang, Xiaohui Xie, Tongze Wang, Fangchen Luo, Yong Cui  
**Data:** 2026-09-23  
**Categorie:** cs.CR, cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2609.28559v1

> LLMs increasingly operate through coding-agent harnesses that inspect repositories, invoke tools, and modify files. Substituting the model behind such an agent can therefore change security-relevant decisions, including whether it verifies changes or recovers safely from failures. Existing LLM fingerprints largely infer identity from direct text or token distributions. In coding agents, these signals are mediated by system instructions, controller logic, tools, and execution feedback, limiting their transfer. We present LIDAR (LLM Identification from Decisions and Actions at Runtime), an active black-box fingerprinting method for coding-agent execution. Three coding probe pairs expose post-edit verification, transient-failure recovery, and specification--test conflict resolution under controlled changes. LIDAR represents the resulting trajectories with complementary instance-level and distribution-level features and compares them with clean references using a lightweight probabilistic identifier. It requires no access to model weights, logits, or provider internals. Across 36 models from seven families and two agent harnesses, LIDAR achieves high Top-1 accuracy and MRR and outperforms four existing fingerprinting and API-auditing baselines. Ablations confirm that the two feature levels, all probe pairs, and their controlled variants contribute. These results show that agent execution behavior provides model-identity evidence beyond final outputs.

---

## 180. The Capability Manifold and ML Scaling Laws

**Autori:** Syed Ali Raza Zaidi, Maryam Hafeez  
**Data:** 2026-09-23  
**Categorie:** cs.LG, cs.AI  
**Link:** https://arxiv.org/abs/2609.27588v1

> Existing machine learning (ML) scaling laws relate predictive loss to compute, model parameters, and data. However, as models are increasingly deployed through agentic harnesses, loss alone is insufficient to characterize downstream performance: models with similar loss can exhibit different capabilities in reasoning, retrieval, planning, and adaptation. Yet, no unified framework connects such capabilities to the coupled resources available across the ML lifecycle. We bridge this gap by introducing a capability manifold, a multidimensional framework mapping downstream capabilities to pre-training, post-training, and test-time resources through bounded scaling functions. Analytical Jacobians quantify capability sensitivity to resource changes and interactions. As an initial application, we embed Kaplan- and Chinchilla-type scaling laws and test-time compute within the framework, demonstrating how existing scaling relationships can be unified as trajectories on a common capability manifold.

---

## 181. Agensh: Scaling Organizational Intelligence to 1,024 Agents

**Autori:** Zhihao Zhan, Ting Song, Li Dong, Shaohan Huang, Jianxun Lian, Yan Xia, Furu Wei  
**Data:** 2026-09-22  
**Categorie:** cs.CL, cs.MA  
**Link:** https://arxiv.org/abs/2609.26781v1

> A multi-agent system can reduce latency on complex tasks by executing work concurrently. Several pioneering harness frameworks support multi-agent systems. However, the scalability of current multi-agent harnesses is often constrained by a central orchestrator's capacity to allocate tasks and coordinate workers. To address this limitation, we introduce Agensh, a scalable self-organized multi-agent harness without a central orchestrator: concurrent workers execute a multi-agent cooperation loop, continuously gathering context, claiming and self-assigning sub-tasks, taking action and sharing findings, verifying results, and merging progress in an asynchronous manner. The loop is supported by the agentic organization infrastructure comprising three components: a shared workspace holds proposed, ongoing, and completed work; a message interface lets workers communicate; and shared context retains reusable findings and work intentions. To test the scalability of Agensh, we evaluate it on the five hardest ProgramBench tasks with GPT-5.6-sol (high). Scaling from 1 to 128 agents raises the mean final test-pass rate from 19.31% to 28.78%, an approximately 49% relative improvement. Larger organizations reach comparable test-pass rates earlier. On pandoc, scaling from 1 to 1,024 agents raises the final test-pass rate from 33.89% to 55.06%. Worker trajectories further show that different forms of self-organized cooperation gradually emerges and standardizes as the organization grows. These results reveal the number of agents as a new scaling dimension for multi-agent organizations to expand the frontier of general intelligence, offering a practical solution for complex tasks under hard latency constraints or time budgets.

---

## 182. Grow the Harness, Not the Context: From Strategy-Free Scaffolds to Reusable Specialist Agents

**Autori:** Laizhen Li, Jiarui Li, Juanjuan Zhao, Kejiang Ye, Ye Li, Cheng-zhong Xu, Xitong Gao  
**Data:** 2026-09-22  
**Categorie:** cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2609.26760v2

> Large language model (LLM) agents often handle streams of related tasks, yet standard harnesses repeatedly ask the model to reconstruct the same control decisions inside each task's context. We study whether task feedback can instead turn recurring control into reusable executable code, while reserving LLM calls for task-specific semantic reasoning. We introduce Growing Harness, a failure-guided training paradigm that learns the agent harness itself from a strategy-free scaffold that exposes fixed model and tool interfaces but encodes no task-solving controller. Function-level execution traces localize each failure to a bounded code surface, an optimizer repairs a window of failures jointly, and a success-first held-out gate rolls back repair sequences that harm prior capability. Accepted edits accumulate in one shared harness, allowing its control structure to emerge from task feedback. Across BrowseComp-Plus and WebArena-Verified with three deployment models from 4B to 120B parameters, Growing Harness achieves the highest mean success in five of six benchmark-model settings and trails the best mean by 0.7 pp. in the sixth. Relative to a Tool-Calling agent, it reduces LLM calls by 76.0-91.8% and deployed-agent inference cost by 74.4-98.6%. On WebArena-Verified, its success remains 44.7-45.3% across model scales, whereas Tool-Calling falls to 6.7% with the 4B model. Ablations show that trace-local edits, joint repair, and gate-based rollback each improve final success. These results show that persistent program growth can move recurring control out of model context and into low-cost code, yielding reusable specialist agents that remain effective with smaller deployment models.

---

## 183. FIRE: Failure-Informed Runtime Engineering for Reliable Language-Model Agents

**Autori:** Nikita Agarwal, Nivedit Jain  
**Data:** 2026-09-22  
**Categorie:** cs.AI, cs.CL, cs.SE  
**Link:** https://arxiv.org/abs/2609.26048v1

> Language-model agents often reach a working solution and then fail to consistently deliver it. We study runtime policies: targeted natural-language instructions and action denials applied by the agent harness at states that preceded observed failures, without changing model weights or the user prompt. With this, keeping capability constant, we observe a meaningful unlock in delivered reliability. Across the complete 87-task Terminal-Bench 2.1 suite, with two attempts per task, policies increase repeated success (pass^2) in all three GPT-5.6 tiers: 50.6% to 54.0% for Luna, 55.2% to 60.9% for Terra, and 64.4% to 73.6% for Sol. Sol's best-of-two success changes by 1.2 points while repeated success rises by 9.2, showing that policies chiefly convert reachable solutions into dependable delivery. We further cover 14 tasks under Terra's frozen portfolio. Policy-guided Terra reaches 71.4%, compared with 64.3% for unassisted Sol, at about half the cost, demonstrating how engineering around models could unlock dependability for a use case. To isolate the mechanism we run a randomized five-arm experiment: real policies reach 61% on eligible tasks, versus 39% without a policy, 36% with a timing-matched sham, and 39 to 43% with generic verification or reconsideration. The intended corrective behavior appears in 22 of 24 coded policy attempts, against at most 14 in any other arm. Runtime policies are therefore a practical reliability layer: they make capabilities an agent already possesses substantially more repeatable.

---

## 184. Qwen3.8-Omni: Towards Native Omni-Modal Agents

**Autori:** Qwen Team  
**Data:** 2026-09-22  
**Categorie:** cs.CL, cs.CV, cs.MM  
**Link:** https://arxiv.org/abs/2609.25611v1

> We introduce Qwen3.8-Omni-Flash, a natively multimodal agentic model for real-world multimodal productivity. Compared with previous omni models, which primarily emphasized perception and interaction, Qwen3.8-Omni-Flash substantially improves multimodal understanding and reasoning, as well as performance on long-horizon agentic tasks. These capabilities are supported by a native multimodal co-training strategy that preserves strong text-domain capabilities while facilitating the transfer of agentic capabilities from text to audio and video tasks. The model inherits the sparse mixture-of-experts (MoE) architecture of Qwen3.8-Next and extends the context window to one million tokens, supporting long-context multimodal reasoning and long-horizon planning. These advances enable integration into production workflows as a primary agent or a specialized sub-agent, supporting video editing, long-form audio and video translation, music-conditioned music video or movie generation, and video-based note or omni-skill creation. To address the lack of native audio and video support in existing agent harnesses, we release Qwen-MM-Plugins, a lightweight open-source plugin framework for multimodal productivity. We further frame real-time multimodal interaction as a system-level challenge requiring orchestration of context and memory management, tool use, and sub-agent delegation. Accordingly, we release Qwen-Live-Harness, an open-source framework for building responsive, real-time multimodal agents based on Qwen3.8-Omni-Flash. Extensive evaluations demonstrate that Qwen3.8-Omni-Flash achieves strong performance across multimodal understanding, reasoning, long-horizon agentic execution, and video productivity tasks. These results and the accompanying open-source tools support Qwen3.8-Omni-Flash as a practical foundation for deploying natively multimodal agents in research and production.

---

## 185. Harness-Zero: Harness Distillation via Agent-as-Harness

**Autori:** Haoran Ye, Yuxing Lu, Haonan Dong, Zhaochen Su, Guojie Song  
**Data:** 2026-09-21  
**Categorie:** cs.AI, cs.CL, cs.NE  
**Link:** https://arxiv.org/abs/2609.24974v1

> Agent harnesses, the external systems that mediate model-environment interaction, can substantially improve agent performance, but their gains remain tied to the harness at deployment. Because the best harness varies across domains, instances, and models, a general-purpose agent must either settle for a suboptimal shared harness or route among an ever-growing set of specialized ones. We therefore study agent harness distillation: using a domain- or instance-optimized harness as training-time guidance and transferring the behaviors it induces into model weights, so that its gains survive under a single fixed target harness. The challenge is that the two harnesses differ in action space and available information, so guidance from the optimized harness cannot serve directly as supervision for the target one. We introduce Harness-Zero, which enables harness distillation through agent-as-harness. Guided by the optimized harness, a harnessing agent corrects student responses before execution in the target harness's action space, turning harness guidance into training demonstrations. Fine-tuning on the resulting trajectories internalizes harness-induced behavior into the model, so the specialized harness can be removed at deployment. Our experiments spanning knowledge work, tool use, and science domains show that: (1) For frontier LLMs using the same evolved harness, agent-as-harness outperforms code-as-harness. (2) With the specialized harness removed at deployment, Harness-Zero improves the base model's macro-average task success from 23.3% to 44.3%, even exceeding the 41.7% it reaches with that harness still attached. (3) Harness-Zero recovers harness-induced behaviors absent from the base model, with 82.3% average recovery across 28 patterns in the three domains.

---

## 186. RRSI: Regularized Recursive Self-Improvement of Agent Harnesses

**Autori:** Peng Xia, Rujun Han, Zifeng Wang, Yanfei Chen, Yufan Zhuang, Yoonho Lee, Chengsong Huang, Han Yu, Zhongying CuiZhu, Yifei Ming, Huaxiu Yao, Burak Gokturk, Tomas Pfister, Chen-Yu Lee  
**Data:** 2026-09-21  
**Categorie:** cs.LG, cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2609.24972v3

> An LLM agent's capability is largely magnified by its harness, namely the prompts, control flow, tooling, memory, and context management surrounding the frozen backbone model. Recent methods increasingly automate this process by iteratively proposing and selecting component-wise edits of an agent harness, practically establishing a form of recursive self-improvement (RSI) at the agent-system level. However, such recursive evolution may overfit by memorizing the training tasks, showing large in-distribution gains that shrink or even vanish on out-of-distribution benchmarks. We introduce Regularized Recursive Self-Improvement of Agent Harnesses (RRSI), which incorporates the principles of regularizations into harness self-improvement by constraining the evolution candidate proposal and selection. The proposer operates with a temporally annealed budget, limiting how many edits a candidate can bundle, and it encourages unexplored trajectories based on evolution history. The selector is equipped with a critic and a pruner: the critic screens benchmark-specific proposals, while the pruner, removes changes that are too small, too expensive, or no longer useful. Together these constraints favor reusable agent mechanisms over benchmark-specific ones or even noises. Across eight benchmarks spanning coding, agentic workspace and engineering design tasks, RRSI gains up to 6.0 points on the split it evolves against and up to 4.3 points on the five out-of-distribution benchmarks, while producing a harness that runs on 30% fewer policy tokens than the unregularized evolution. Code is available at https://github.com/google-research/rrsi and project page is https://regularized-rsi.com/.

---

## 187. DIP-CAD: A Design-Intent-Preserving Agent Harness for Parametric CAD Modeling

**Autori:** Xi Cheng, Chenxi Zhai, Hang Cheng, Mingyu Fan, Pingfa Feng, Long Zeng  
**Data:** 2026-09-19  
**Categorie:** cs.CV, cs.AI  
**Link:** https://arxiv.org/abs/2609.22688v2

> Parametric CAD modeling requires not only matching the target shape, but also preserving design intent after parameter editing. However, most existing methods focus on improving static shape generation accuracy, while the dependencies that govern later edits are often overlooked. To tackle this issue, we present DIP-CAD, a design-intent-preserving agent harness for generating parametric CAD model from image. DIP-CAD combines vision-language model reasoning with CAD kernel operations to construct dependencies that encode the design intent. In parametric CAD, these dependencies are mainly established through geometry references in modeling commands and constraints in parametric sketches. At command level, ID-based explicit geometry reference binds modeling commands to selected faces, edges, or vertices. At sketch level, local-coordinate bridge ensures accurate sketch placement, providing the basis for correctly establishing sketch constraints. Constraints among sketch primitives and constraints to external projected geometry further preserve both internal sketch relationships and dependencies on existing geometry. To providing a more comprehensive data foundation for parametric CAD modeling tasks, we introduce the Geometry Explicit Reference Dataset (GERD), whose structured data format links stepwise modeling commands to intermediate CAD models through explicit geometry references. On GERD-EVL and a DeepCAD test subset, DIP-CAD improves mIoU for static model generation by 11.1% and 5.6%, respectively. In parameter-editing evaluations, the corresponding mIoU improvements are 7.0% and 4.2%. Case studies further demonstrate how parameter edits drive shape update while preserving design intent.

---

## 188. Inference-Engine Fingerprinting Attacks are Practical: Exploring Model-Driven Environmental Discovery, Exploitation, and Escape

**Autori:** Sarah Radway, Andrew Cheng, Vijay Janapa Reddi, James Mickens  
**Data:** 2026-09-17  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2609.20614v1

> Frontier AI models are rapidly gaining the ability to exploit vulnerabilities in complex pieces of software. The risk is not theoretical, as evidenced by recent sandbox escapes performed by frontier models at OpenAI and Anthropic. Discussions of how to sandbox inference stack components often focus on components other than the inference engine itself (e.g., network proxies or code execution environments). However, the inference engine is an attractive target for a misaligned model. For example, if a model can trigger exploits in that engine merely by generating specially-crafted output tokens, the model can initiate a multi-step, to-the-bare-metal exploit chain in the engine, without relying on vulnerabilities in other components of the inference stack, and without assistance from externally-provided, maliciously-crafted input tokens. In this paper, we show that a misaligned model can perform inference engine fingerprinting to determine the specific engine (e.g., vLLM, SGLang) which executes the model. Once the engine has been fingerprinted, the model can leverage engine-specific exploits to take control of the engine using only carefully-selected output tokens. We provide concrete examples of model fingerprints in five popular engines, and demonstrate how realistic agentic harnesses allow a model to leverage those fingerprints to identify the local engine. We also describe a proof-of-concept, to-the-bare-metal exploit chain that originates from a fingerprinted (and subsequently compromised) inference engine. We conclude by discussing several ways that inference engines could be changed to make fingerprinting attacks more difficult.

---

## 189. SoL-Pi: Recursively Scaling Auto-Research Loops for Efficient Agent Harness

**Autori:** Haozhe Liu, Tian Ye, Sensen Gao, Qihang Cao, Yitong Li, Mingchen Zhuge, Duomin Wang, Ruihua Zhang, Ping Luo, Jiawang Bian, Lei Zhu, Ligeng Zhu, Enze Xie, Song Han  
**Data:** 2026-09-17  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.20519v1

> As coding agents move from supervised code completion to unattended, around-the-clock exploration, their work expands from isolated predictions into long trajectories of reasoning, tool use, and feedback. Token efficiency therefore becomes important for scaling recursive self-improvement. We take an RSI-inspired approach at the harness layer, scaling auto-research loops across increasingly numerous and diverse environments for harness rollouts. At this scale, the process yields reusable improvements that transfer beyond their development setting, moving automated harness discovery toward production-level outcomes. Four mechanisms survive selection and form SoL-Pi, spanning action execution, context compaction, observation handling, and delegated reading. On the 51-task EdgeBench evaluation, SoL-Pi achieves performance comparable to Pi across GPT-5.6 Sol and Opus 5 while reducing recorded token traffic by 44.7-49.0% and API cost by about one third. In other words, estimated hourly savings are \$8.75-\$13.50 relative to native Codex and Claude Code harnesses, and \$4.36-\$5.71 relative to Pi.

---

## 190. How Do Agent Harnesses Create Value? Planning Information and Release Control in Stateful LLM Agents

**Autori:** Yukun Zhang, Kemu Xu, Yishen Chen  
**Data:** 2026-09-17  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.20474v1

> Agent harnesses supply planning guidance, organize execution, and check completion. We study how these components affect success, erroneous acceptance, and cost in two Retail experiments and an Airline pilot in $τ^2$-bench. The primary comparison pairs prewritten task-specific plans (Fixed) with shuffled policy text matched in word count (Sham), isolating the contribution of guidance content. Across 265 matched cells, Fixed improves oracle-verified success by 7.17 percentage points (90\% task-clustered bootstrap interval, 1.15--13.36 points), with gains concentrated in higher-complexity tasks. A read-only terminal verifier rejects 61\% of Retail oracle-invalid episodes while withholding 17\% of correct ones, at less than one cent of additional cost per episode. Which component matters more depends on the loss assigned to erroneous acceptance: at low liability the planning gain dominates; at high liability the verifier's avoided false passes dominate---and a standalone verifier captures nearly all the false-pass benefit of the full planning-plus-verification stack at a fraction of its cost.

---

## 191. Rethinking Multi-Agent Collaboration: When More Is Less

**Autori:** Yishuo Yuan, Yibo Wu, Yihan Zhang, Minyuan Sun, Shenliang Li, Xinkai Ma, Yifan Li, Jiaheng Liu  
**Data:** 2026-09-17  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.19759v2

> The rapid advancement of large language models and single-agent harnesses has reshaped the landscape of autonomous systems, raising a critical question of when multi-agent collaboration offers genuine value. As individual agent capabilities continue to scale, multi-agent collaboration faces diminishing returns while incurring growing context overhead. Through systematic analysis, we delineate the capability boundaries of multi-agent collaboration relative to single-agent alternatives, showing that it confers systematic benefits specifically in long-horizon tasks with sparse dependencies, while single-agent harnesses remain superior in tightly coupled, sequential workflows. Building on these insights, we propose SAIGE, a lightweight multi-agent collaboration mechanism based on Semantic-Aware Incremental Graph Evolution. SAIGE models collaboration as a dynamically evolving graph, where nodes are agent instances spawned on demand and edges encode semantic dependencies established through content-based information retrieval. Experiments on long-horizon, complex task benchmarks show that SAIGE achieves a favorable trade-off between context efficiency and task performance, and that scaling the agent pool or deepening the recursion level does not consistently improve outcomes. Our findings suggest that multi-agent superiority is bounded by task structure rather than universal, and that more agents do not necessarily make a system more intelligent.

---

## 192. AeroWeaver: An Embodied-Agent Harness for Weaving Aerial Skills into Distributed, Adaptive Swarm Execution

**Autori:** Jiabin Lou, Yirong Yang, Haopeng Wang, Xuxin Lv, Xinyu Liu, Diyuan Hou, Xuehong Liu, Rongye Shi, Wenjun Wu  
**Data:** 2026-09-16  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.18520v1

> Collective intelligence is a collaborative autonomy paradigm in which multiple agents pursue shared objectives through local perception, information exchange, and coordinated action. UAV swarms embody this paradigm by coordinating multiple vehicles in tasks such as search, inspection, and tracking. Recent advances in large language model (LLM) agents have strengthened natural-language task understanding and high-level planning, providing a flexible semantic interface between mission descriptions and collective behavior. While these advances expand semantic reasoning, applying LLM agents to UAV swarms raises challenges in grounding model decisions in executable capabilities, reconciling global task reasoning with distributed execution, and using mission-specific experience for continual adaptation. To address these challenges, we introduce AeroWeaver, an embodied-agent harness that weaves individual UAV skills into coordinated mission-level behavior. AeroWeaver connects semantic decisions to governed skills, organizes role-conditioned local agents for distributed coordination, and uses role-indexed state-action-reward experience to refine skill selection online. Experiments and runtime validation show that AeroWeaver maintains valid skill execution under tested conditions and supports body-local multi-UAV operation without a central agent generating joint actions from global context, while reward-guided online updates provide a training-free path for adaptive learning swarm agents from accumulated execution experience. Code: https://github.com/Admire-ljb/AeroWeaver.

---

## 193. Stellar Colosseum: A Many-Agent Harness for Long-Horizon Research in Mathematics and Theoretical Computer Science

**Autori:** Honghao Lin, David P. Woodruff, Yuan Deng, Jieming Mao, Song Zuo, Vahab Mirrokni  
**Data:** 2026-09-14  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2609.15983v2

> Language models can produce plausible short proofs, but may still be unreliable on long-horizon research problems, where progress depends on a sequence of uncertain and interdependent decisions. We introduce Stellar Colosseum, a model-agnostic harness for allocating inference across research in mathematics and theoretical computer science. Colosseum explores alternative strategies before proof construction, uses a readiness gate to decide when a route is mature enough to decompose, represents the proof plan as interdependent section-level subproblems, and routes verifier findings back to the affected part of the argument. Across these stages, it generates candidates in parallel, attacks them with targeted falsification, and combines candidates and their critiques into a single research artifact through overlapping random-sample tree aggregation. The Colosseum workflow has been integrated into Google Antigravity's Teamwork framework as the Long Proof pattern. We demonstrate the capabilities of Colosseum through open-ended research and evaluations on theorem-proving and competitive programming benchmarks. Using Colosseum with Gemini 3.1 Pro, we obtain several new results that address open problems arising from papers published at top venues such as FOCS and JMLR. On TCS-Bench, a benchmark of research-level theorem-proving tasks drawn from papers published at FOCS, STOC, and SODA, Colosseum achieves 71.0% accuracy using Gemini 3.1 Pro and Gemini 3.7 Flash. In a separate Codeforces evaluation using Gemini 3.1 Pro, the proof-oriented pipeline with execution feedback solves 218 of 222 problems.

---

## 194. The Router Within: Eliciting Native Skill Routing from a Frozen LLM

**Autori:** Ruishuo Chen, Xun Wang, Yu Chen, Zhuoran Li, Longbo Huang  
**Data:** 2026-09-14  
**Categorie:** cs.LG, cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2609.15982v2

> Skills extend an LLM agent beyond its parametric knowledge, and the gain they promise rests on picking the right one. Deployed harnesses route by preloading every skill's metadata into the context, which disperses the agent's attention and caps the library size. Retrieval pipelines move the selection out of the context, but also out of the agent's capability. We show that the frozen agent LLM already carries the routing signal in its own forward passes, and that two linear maps suffice to read it out with no skill text in the context. Our Gavel (Glance And Verdict from a frozen LLM) reads it in two steps. A glance scores the full library by matching the task's mid-layer states against a compact bank that one forward pass builds for each skill at installation, with the two maps as the only trained parameters. A verdict then resumes each shortlisted skill's forward pass, reads the model's own likelihood and yes/no judgment, and fuses both with the glance as a product of experts. Trained once, Gavel transfers zero-shot to three public benchmarks and SkillTraj, our new benchmark of 372 simulated agent trajectories. On Qwen3-32B it outperforms progressive disclosure and retrieve-and-rerank pipelines that add 1.2B to 16B external parameters, by up to 13.4 points on written tasks and up to 21.9 when the need for a skill arises mid-rollout. Routing accuracy improves as the backbone does, and in a bash-agent harness Gavel lets the 32B trigger the right skill on Skill-Use more often than models of up to 1.6T parameters in Codex.

---

## 195. MUSE: A Theory-Harnessed Story Engine for Vibe Narrativizing

**Autori:** Jianxiang Ma, Xiaocui Yang, Daling Wang, Mingfu Zhang, Zijing Wang, Yuesong Hou, Yichen Gao, Junzhao Huang  
**Data:** 2026-09-14  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2609.15188v4

> LLMs have been able to generate fluent prose, but high-quality stories also require coordinated decisions about plot, character, and language across planning, drafting, and revision. We formulate Vibe Narrativizing as turning natural-language writing requirements into a finished story. MUSE, a Theory-Harnessed Story Engine, addresses two bottlenecks: rule quality and sustained rule realization. Story theory supplies the rules, and a practical agent harness puts them to work. Knowledge engineering organizes Robert McKee's theory through rule atomization, semantic consolidation, mechanism abstraction, a single source of truth, and layered disclosure; typical examples clarify judgments that depend on context and aesthetic purpose. The harness preserves story decisions in intermediate deliverables across design, character performance, scene composition, and revision. Context engineering supplies each role with relevant guidance and decisions; a masterwork corpus provides inspiration and prose references. A worked example follows a requested object from its thematic role to climactic actions. Across four base models, MUSE improves WritingBench by 1.1 to 6.2 points over zero-shot generation; it is the only multi-stage system in our comparison to do so. It also raises LongStoryEval by more than ten points on three of the four models. ConStory-Bench consistency error density remains in the low single digits for all four models, below every reproduced story-system baseline on three of the four models. Ablations locate the largest quality contribution in structural design, voice-specific effects in the character path, and further gains in revision.

---

## 196. ModularRSI: Modular and Generalizable Recursive Harness Self-Improvement

**Autori:** Siwei Wu, Jincheng Ren, Yizhi Li, Haau-Sing Li, Chengran Yang, Xudong Ma, Yuxuan Zhang, Weicheng Gu, Jian Yang, Riza Batista-Navarro, Chuanyi Zhang, Xianglong Liu, Ming Zhou, Bryan Dai, Chenghua Lin  
**Data:** 2026-09-14  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2609.14857v2

> Recent work extends recursive self-improvement (RSI) to agent harnesses for long-horizon coding and terminal tasks, enabling agents to improve execution mechanisms from experience. However, generalizable harness RSI remains challenging. First, evolving harnesses on evaluation benchmarks or their subsets makes it difficult to distinguish reusable improvements from benchmark-specific adaptation. Second, single-trajectory updates can conflate systematic harness deficiencies with instance-specific reasoning and solution details, producing modifications that transfer poorly to unseen tasks. Third, localizing recurring behavioral deficiencies within monolithic harnesses is difficult, while whole-harness optimization can entangle unrelated mechanisms and complicate attribution and validation. We propose ModularRSI, a benchmark-disjoint, contrastive, and modular framework for generalizable harness evolution. ModularRSI contrasts successful and failed trajectories for the same task and aggregates evidence across tasks to identify recurring behavioral deficiencies. It decomposes the evolvable harness into five functional modules: Agent Loop, Tool Use, Observation Management, Context Management, and Task Completion Detection. Each module evolves independently within a restricted modification scope, followed by an integration stage that combines the evolved modules into a unified harness and resolves potential conflicts. To support benchmark-disjoint evolution, we curate 2,000 executable evolution tasks from external sources that are disjoint from downstream evaluation benchmarks. Experiments on TB2.0 and SWE-Bench Verified show consistent improvements on unseen in-domain and cross-domain tasks, with the evolved harness also transferring across different foundation models.

---

## 197. Safety Signals to Verify NetOps Agents with Action-Level Granularity

**Autori:** Tobias Labarta, Frederik Pahde, Novak Boškov, Maximilian Dreyer, David Birkenberger, Manzoor Ahmed Khan, Sebastian Lapuschkin, Wojciech Samek  
**Data:** 2026-09-13  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.14422v2

> Agentic Network Operations (NetOps) are an emerging paradigm promising to enable workload-aware, self-adjustable, and reliable autonomous networks. While agents have proven their value in incident summarization and telemetry signal extraction, their effectiveness as autonomous control-loop engines heavily relies on their long-horizon reliability. One such setting is the datacenter fabric, where an agent must respond to alarms and operator intents while abstaining from high-risk actions that may cause or extend downtime. Abstention, however, presupposes that an action's impact is known pre-execution, which necessitates a per-action ground truth that NetOps agent benchmarks do not provide. We construct such a ground truth for the network repair task of NetArena. A symbolic replay of the emulated network, validated against the environment at every turn, yields the exact value of every action. From the action-level value, we derive two pre-execution targets, namely whether an action reduces the repair distance (progress) and whether it increases it (harm). We show across 10 agent models, that agent verifiers leveraging internal signals predict both harm and progress more reliably than a baseline using observable signals only. Perspectively, we aim to use these signals as safety feedback to an agent harness to abstain from risky actions and protect the target system.

---

## 198. Tasks over Application Manuals: Revealing Gaps in Long-Horizon Procedural Reasoning for Language Models

**Autori:** Utkarsh Soni, Syed Shariyar Murtaza, Yifan Nie, Sachin Chandrasekhar, Eugene Wen  
**Data:** 2026-09-11  
**Categorie:** cs.CL, cs.AI  
**Link:** https://arxiv.org/abs/2609.13005v1

> Large language models (LLMs) have achieved strong performance on a wide range of natural language tasks, and recent benchmarks suggest that they are increasingly adept at multi-hop reasoning. However, these benchmarks are typically short-horizon, requiring only a small number of retrieval or inference steps, and provide limited evidence of reliability on real-world tasks that involve following manuals spanning hundreds of pages with complex, interdependent guidelines. In this paper, we introduce Tasks over Application Manuals (TAM), a benchmark for evaluating long-horizon procedural reasoning. We construct TAM by curating real-world tasks from two domains: ICD-10-CM clinical coding (mapping medical conditions to diagnostic codes) and U.S. federal sentencing (computing crime sentencing guideline outcomes, specifically offense levels), with human-validated labels. Each task requires following an authoritative manual with tens of thousands of rules and executing a sequence of interdependent steps across different sections to produce an exact answer. We evaluate general-purpose prompting approaches, including retrieval-augmented generation, ReAct-style prompting, and an agent-harness baseline on GPT-5, and find that the best exact-match performance remains extremely low: 1% on ICD-10-CM coding and 15.5% on sentencing tasks. These results show that current benchmarks may overestimate LLM reasoning ability and miss a key challenge: reliably following long, rule-based procedures. The complete TAM data and code are publicly available.

---

## 199. Online Video Agent Harness for Long Video Understanding

**Autori:** Sen Yang, Boqiang Duan, Jing Yang, Weihao Bo, Jie Liu, Boyuan Tong, Ze Feng, Wenkang Zhang, Jingdong Wang, Hua Wu  
**Data:** 2026-09-11  
**Categorie:** cs.CV, cs.AI  
**Link:** https://arxiv.org/abs/2609.12818v1

> Long video understanding often behaves like a visual needle-in-a-haystack problem: query-relevant evidence is sparsely distributed across long temporal spans, while packing dense frames into a single VLM context incurs \textit{context rot} and high cost. Existing video agents often rely on query-agnostic offline preprocessing or ad hoc tool sets, which can miss query-specific details and waste computation. In this work, we present VideoXAgent, a purely online video-agent harness for long video understanding that starts from the given video file and user query, plans and decomposes the task, invokes specialized expert tools on demand, and aggregates multimodal evidence to produce a final answer while resolving conflicts among observations. To support this on-demand invocation, we design a suite of heterogeneous expert tools guided by a data-driven taxonomy of atomic capabilities, spanning scripts, VLMs, and domain models (e.g., detection, OCR, ASR, face recognition). The harness further enforces objective evidence prompting and budget-aware control to curb hallucination and non-termination. Across Video-MME-Long, LongVideoBench-Long, LVBench, and MINERVA, VideoXAgent is competitive with frontier LMMs and video agents under a smaller context footprint---about 50k tokens of agent context per sample, even on hour-long videos. In particular, on complex video-reasoning benchmarks such as MINERVA, it matches this level while using only about 15\% of the context of a 1,024-frame dense-packing baseline. Notably, the harness remains effective with a visually weak or even text-only orchestrator, suggesting that strong long-video understanding can emerge from progressive agentic evidence seeking rather than from packing the full video into a single context. Project page: https://go-agent-x.github.io/video_agent_harness/

---

## 200. COBRA-Skills: Contextual Bandit-Guided Evolution for Agent Skill Optimization

**Autori:** Pingchen Lu, Xiangyi Wang, Xiang Li, Jie Mao, Zikun Qu, Junfeng Luo, Yao Shu, Bryan Kian Hsiang Low, Zhongxiang Dai  
**Data:** 2026-09-10  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.11682v1

> Large language model (LLM) agents can benefit from reusable skills distilled from prior task experience, yet existing skill optimization methods often rely on costly execution-based evaluation and substantial task data. We introduce \textbf{COBRA-Skills}, an efficient framework that formulates skill optimization as budgeted sequential optimization over a dynamically evolving candidate space. COBRA-Skills couples contextual-bandit-guided prioritization with evidence-grounded skill evolution, selectively allocating evaluations to promising or informative candidates while continually refining the skill population from execution feedback. Across six heterogeneous agent benchmarks and three target models, COBRA-Skills consistently achieves the strongest average performance among compared methods, while reducing optimization cost by 55--58\% relative to SkillOpt and using only 50 unique optimization examples per benchmark. Further analyses show that COBRA-Skills remains robust to changes in the agent harness and performs effectively when the target model itself is used for skill generation and refinement.

---

## 201. RobustSGPO: Search-Space Control for Agent Harness Evolution

**Autori:** Zibo Zhao, Jijun Shi, Mo Zhou, Zhongyuan Wang, Shifu Bie, Yunfei Zhang, Xuanting Zhou, Xiangyu Wu, Bin Liu, Ruiming Tang, Wenwu Ou, Kun Gai  
**Data:** 2026-09-09  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.09646v2

> Semantic-gradient-based prompt optimization (SGPO) improves agent harnesses using execution feedback, but its local update rule leaves the choice of edit scope and operation unresolved. We introduce RobustSGPO, which specifies the requested edit, constructs and checks the patch, and continues search from either the incumbent or retained snapshots. We evaluate permission scheduling, cumulative controls, and task-family transfer in the AgentX brainstorming workflow using 120 tasks, 95 runs, and 7,350 candidate attempts. Periodic $1\to2\to3$ scheduling exceeds fixed maximum permission by 0.28 test-score points. RobustSGPO increases completion on 30 held-out tasks from 60.0% to 80.0% and improves test quality from 3.77 to 4.14 under a 20-million-token budget. Category retention reduces source-task degradation after a shift, whereas random retention reaches a higher destination endpoint. Search-space control benefits quality through executable edits and alternative starting points, with measurable retention overhead.

---

## 202. Co-Evolving Harnesses and Models: On-Policy Correction Helps Weaker Models Catch Up Where Imitation Fails

**Autori:** Zhou Yu, Bin Bi, Shiva Kumar Pentyala, Shubham Mehrotra, Sougata Chaudhuri, Shilpa Bhagavath, Zeyuan Chen, Ran Xu, Phil Mui, James Zhu, Sitaram Asur  
**Data:** 2026-09-08  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.09134v1

> Agent harnesses (the system prompt, tool set, execution hooks, and context-management scaffolding around a model) are a critical determinant of agentic task success. Automated harness evolution can enable smaller models to perform well on domain-specific tasks at a fraction of frontier-model cost. Since both the harness and model weights shape behavior, we ask how harness evolution and lightweight fine-tuning should be combined. Across seven enterprise agent tasks, we first evolve a harness with the weaker model, then find that a stronger expert often uses it more effectively, suggesting expert supervision could close the remaining gap. However, training the weaker model on the expert's complete trajectories under the evolved harness backfires: performance regresses on all seven tasks by 4 to 30 points across Qwen3-Coder and Gemma 4, even though the same procedure helps under the unevolved harness. Our analysis shows that imitation transfers knowledge and increases scaffold usage, but disrupts model-harness fit: the weaker model adopts the expert's planning strategy without the competence to execute it and no longer matches the harness evolved around its native planning style. We therefore develop an on-policy expert-correction pipeline, automated by a meta-level MLE agent, that localizes the failing turn in the weaker model's own rollout and asks the expert to rewrite only that turn. This preserves the model's planning style and combines the gains of harness evolution and model adaptation. Our results identify and resolve a source of contention between harness and weight updates, yielding a compatibility-preserving recipe for economical co-evolution on domain-specific enterprise tasks.

---

## 203. Experience Funnel: A State-Policy Alternating Loop for Self-Evolving Agents

**Autori:** Wenbo Gao, Zhaomou Song, Zhiyuan Ji, Renxi Liu, Xing Li, Xianzhi Yu, Xiaoguang Li, James Chung-wai Cheung, Weizhe Lin, Yaoyuan Wang  
**Data:** 2026-09-08  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2609.08919v1

> Autonomous agents powered by large language models (LLMs) continuously accumulate experience through interaction, creating an opportunity to improve future behavior through self-evolution. A fundamental challenge is how to transform abundant, task-specific interaction experience into reusable model competence without sacrificing the ability to adapt rapidly to newly observed evidence. Explicit textual states, such as skills and agent harnesses, provide fast, human-readable and editable adaptation, but incur persistent dependence on external context; parametric policies provide compact and reusable competence, but are substantially slower to update. We present \textit{Experience Funnel}, a self-evolving framework that couples fast state adaptation with slow policy consolidation in an alternating loop. Interaction trajectories are first distilled into an explicit textual state, where newly acquired experience can be rapidly incorporated and validated. The framework then selectively identifies state-enabled behavior that remains useful across state revisions and consolidates it into the policy through transition-aware distillation. The updated state--policy pair subsequently generates new rollouts, providing fresh evidence for the next round of state adaptation and policy consolidation. Experiments across diverse agent benchmarks show that \textit{Experience Funnel} consistently improves agent capability over state-only evolution and policy-internalization approaches, while progressively converting useful explicit experience into autonomous policy competence.

---

## 204. A Theory of Reliable Self-Evolution for Agent Harnesses

**Autori:** Qianshu Cai, Yonggang Zhang, Jun Nie, Maohao Ran, Huajiang Zheng, Jun Song, Xinmei Tian, Yike Guo, Wei Xue  
**Data:** 2026-09-08  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.08175v2

> In harness self-evolution, agents modify their own prompts, code, tools, and orchestration while keeping the underlying language model fixed. Recent work has shown that agents can improve themselves in response to task failures and achieve substantial performance gains. However, gains on failed tasks do not automatically ensure that performance on previously successful tasks is preserved, raising concerns about reliable adoption. In this work, we provide a theoretically grounded condition under which a self-evolved harness can be reliably adopted. We then propose a validation rule to make the evolved system satisfy the reliable adoption condition with theoretical guarantees. Consequently, the system can achieve progressive improvement through evolution. This leads to a natural question: Does reliable self-evolution have a performance ceiling, and which factors govern this ceiling? Our theoretical results show that the performance ceiling is determined by the costs of verification and evaluation. On the other hand, self-evolution may stall in practice. In this regard, we show that experimental evidence on agent performance shifts can be used to identify the sources of stagnation. Our work thus establishes a theoretical framework for understanding and advancing reliable harness self-evolution.

---

## 205. VEX-Bench: Benchmarking LLM Agents for Assessing Exploitability of Software Supply Chain Vulnerabilities

**Autori:** Jiahao Shi, Edward Tsien, Yifeng Di, Hongjiao Zhang, Yuan Tang, Ronit Dey, Ilona Shishov, Gal Netanel, Zvi Grinberg, Vladimir Belousov, Bat-Zion Rotman, Ilan Pinto, Tianyi Zhang  
**Data:** 2026-09-07  
**Categorie:** cs.CR, cs.LG, cs.SE  
**Link:** https://arxiv.org/abs/2609.08040v1

> The software supply chain has become an increasingly exposed attack surface because of its reliance on intricate yet fragile dependencies. Existing defenses such as GitHub Dependabot often raise many false alerts because their coarse-grained matching cannot determine whether a vulnerable dependency is actually exploitable. Security analysts typically spend substantial time assessing vulnerability exploitability case by case. Recent LLM agents have emerged as promising candidates for this task given their advanced capabilities in coding and cybersecurity, yet no existing benchmark evaluates them on it. Prior benchmarks target zero-day settings, where agents detect and exploit previously unknown vulnerabilities. In contrast, software supply chain security focuses on how known vulnerabilities in upstream dependencies affect downstream projects. This requires agents to reason across repositories and determine whether an upstream vulnerability is exploitable in the downstream project. To address this gap, we introduce VEX-Bench, the first benchmark for evaluating LLM agents' ability to assess the exploitability of software supply chain vulnerabilities. It contains 75 real-world cases mined from GitHub and labeled by security experts, covering Python, Java, and Go. We evaluate nine models across three agent harnesses. While GPT-5.5 and Claude Opus 4.6 reach approximately 80% F1 on binary vulnerability-status classification, only GPT-5.5 surpasses 70% macro-F1 on fine-grained justification classification. This gap highlights the challenge of moving beyond binary exploitability assessment to identifying fine-grained exploitability reasons. Code and data: https://github.com/steven1518/vex-bench

---

## 206. Scientific Agents: Evaluating Profession-Specific System Prompts on Scientific Tasks

**Autori:** Timothy Kassis  
**Data:** 2026-09-07  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2610.00084v1

> Detailed profession-specific system prompts raise token use and estimated cost per response without a consistent accuracy gain. We evaluate Scientific Agents, an open-source corpus of 503 profession-specific AGENTS.md profiles, with Gemini 3.8 Flash via OpenRouter in the Pi agent harness. We compare matched profiles with four controls: a minimal baseline ("You are a helpful assistant"), the profile's opening role sentence, a generic scientific rigor guide, and a profile from an unrelated domain. Across nine text-based science benchmarks (4,531 sampled questions, 100 matched profiles), 4,488 items completed all five conditions after API-error retries, scored with automated, rule-based grading. The average profile-baseline accuracy difference is -0.6 percentage points (95% bootstrap interval [-1.5, +0.2] across fixed tasks), and no benchmark shows a statistically clear improvement. Matched profiles produced 1.5-2.3 times as many output tokens and cost 2.2-4.5 times more per successful call. On 60 tool-using BioMysteryBench bioinformatics problems (three runs each for baseline and profile), mean solve rates were 46.7% with the profile and 56.7% at baseline, a difference of -10.0 percentage points (95% interval [-16.7, -3.3]) driven by more frequent token- and time-limit stops under the profile. Longer prompts had one unexpected operational advantage: on SuperGPQA, frequent provider API drops left the short baseline with a correct first-pass answer on only 54.0% of items, against 71.6% with the profile. Generic and mismatched prompts were about as reliable, so this gain comes from prompt length or formatting rather than domain expertise. For the tested model and tasks, loading full profession profiles by default does not improve accuracy and costs considerably more; whether selective retrieval of profile sections or open-ended scientific tasks would change this remains to be tested.

---

## 207. OpenDiscoveryTrace: Process Traces for Evaluating AI Scientist Workflows

**Autori:** Aayam Bansal, Keertan Balaji  
**Data:** 2026-09-05  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.09203v1

> Existing benchmarks for autonomous AI scientists evaluate only final outputs---generated code, hypotheses, or papers---yet discard the reasoning process by which those outputs were obtained. This makes it impossible to audit scientific methodology, diagnose failure modes, or distinguish systematic reasoning from fortunate guessing. We present \textbf{OpenDiscoveryTrace}, a public dataset of 558 complete AI scientific agent trajectories that captures how models reason, not just what they produce. Each trajectory records a structured 9-field-per-step trace---including thoughts, tool calls, observations, errors, revision triggers, and self-reported confidence---as models execute 124 scientific tasks spanning drug discovery, materials science, genomics, and scientific literature analysis. The dataset covers seven models: three frontier models (GPT-5.4, Claude Opus 4.6, and Gemini 3.1 Pro; 124 trajectories each, fully balanced across domains and difficulty levels) and four open-weight models (Qwen2.5-7B, Mistral-7B-v0.3, Phi-3.5-mini, and Qwen2.5-1.5B; 30 each), plus 60 live-retrieval variant trajectories. Pilot analysis on 363 LLM-judged trajectories reveals that process traces expose behavioral differences invisible to output-only evaluation: all three frontier models achieve comparable success rates (84--89%), yet Claude Opus 4.6 produces 30$\times$ more errors than GPT-5.4 (2.5 vs. 0.08 per trajectory, $p < 0.0001$, Cliff's $δ= 0.613$), with qualitatively different error profiles---66.7% tool misuse for Claude versus 83.6% reasoning errors for GPT-5.4. We define five benchmark tasks with baselines from logistic regression, random forests, LSTMs, and Transformer models. The dataset, trace schema, agent harness, and benchmark definitions are publicly available under CC BY 4.0 to support research on process-level evaluation, scientific agent auditing, and AI governance.

---

## 208. Beyond Prompts: Measuring and Optimizing LLM Tool-Agent Harnesses

**Autori:** Cen Mia Zhao, Haibo Ruan, Wenjie Chen, Pei-fen Tu, Usman Abbasi, Joel Hesch  
**Data:** 2026-09-04  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.05736v2

> LLM tool agents can be improved without retraining by modifying the runtime harness around a fixed model: prompts, tool interfaces, middleware, state handling, and recovery logic. We study this setting as resource-bounded harness selection for fixed-model multi-turn tool agents, with the search surface scoped to prompts and tool-boundary middleware: edits are guarded intercepts at the tool boundary, not arbitrary rewriting of agent execution logic. Our optimizer-agnostic protocol reports mean held-out lift, worst-condition lift, repeatability, logged cost diagnostics, and RelLift95(B), a conservative estimate of the held-out gain of the harness selected under budget B. We instantiate the protocol with prompt-only and prompt-plus-middleware optimizers, including PRISM, which clusters failures and routes repairs to prompt, tool-boundary middleware, or joint edit surfaces within a Pareto search. On BFCL multi-round, tau2-Retail, and tau2-Telecom, PRISM obtains mean held-out lifts of 14.2, 14.9, and 10.1 percentage points and positive empirical RelLift95 on all three benchmarks, and a component ablation attributes the margin chiefly to failure-surface routing and the edit-pattern constraint. Across optimizers, the results show that some search procedures can occasionally find large gains but still choose brittle updates, so the reliability of the chosen harness should be reported alongside average held-out lift.

---

## 209. Environment Evolution for Terminal Agents

**Autori:** Zhiyuan Fan, Tinghao Yu, Yuanjun Cai, Jiang Zhou, Jiangtao Guan, Jincheng Liu, Yun Yang, Dingxin Hu, Zhuo Han, Xing Wu, Feng Zhang, Lilin Wang  
**Data:** 2026-09-03  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.04128v1

> Scaling interactive and verifiable environments is critical for training terminal agents. As frontier models become more capable, environments synthesized from scratch become less challenging and thus provide limited learning signals. Recent co-evolution methods iteratively synthesize environments near the model's learnable frontier based on weaknesses exposed during rollouts. However, their dependence on on-policy rollouts limits generalization and the continuous provision of learning signals as the model becomes stronger. In this paper, we propose environment evolution, which incrementally increases environment difficulty off-policy and schedules the evolved environments generation by generation during training to provide continuous learning signals. We derive three evolution directions that influence environment difficulty from the multi-turn learning objective and then implement evolution along these directions through a loop-engineered multi-agent harness. Quantitative rollout experiments with Hy4 preview, Claude Opus 5, and GPT-5.6 Sol show that environment evolution consistently produces more difficult environments. We validate its effectiveness on Qwen3.6-27B and Qwen3.6-35B-A3B through simple long-horizon RL training, improving their performance by 14.4 and 18.0 percentage points on Terminal-Bench 2.1, respectively.

---

## 210. A Blind Trust, the Bloody Thrust: When Attacker-Controlled Hook Updates Steer AI Agent Harnesses towards Malicious Behaviors

**Autori:** Pengxun Li, Litian Zhang, Jianwei Hou, Shujiang Wu, Song Li, Zifeng Kang, Xi Zhang  
**Data:** 2026-09-03  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2609.03884v2

> Modern AI agent harnesses expose lifecycle hooks that bind shell commands to runtime events such as session start, tool calls, and file edits. These commands run with host privileges yet ship as lifecycle-hook configuration and may fire at times the LLM never observes. We identify the lifecycle-hook update path, which harnesses trust blindly, as a new attack surface. Under a supply-chain threat model in which an attacker controls only plugin metadata and lifecycle-hook configuration, a benign versioned plugin can be trojanized by an update that silently binds attacker-chosen commands to benign events, yielding malicious host-side behavior such as privilege escalation. We propose HookPry, an open-source and fully automated attack framework that systematically exploits this vulnerability across heterogeneous AI agent harnesses. HookPry realizes ten attack objectives; across 25 combinations of harnesses and backends in 1,000 end-to-end runs, it compromises all seven evaluated harnesses, with per-harness success rates reaching 92.5%. Representative defenses remain insufficient: Microsoft Defender has 0% recall, and the union of three static defenses misses 47.5% of malicious artifacts.

---

## 211. Bioinfoysis Technical Report

**Autori:** Qingyang Shao, Xin Zhang, Zhouyang Yuan, Xianying Chen, Yujia Xiang, Zihao Yang, Tong Ye, Yangqi Zhang, Jiakang Xu, Xiaoqing Yan, Xuan Luo, Keyi Li, Enci Fan, Kai Kang, Zhuohan Liu, Xingyu Jin, Chunran Teng, Tao Li, Xinyu Lyu, Minghui Wang, Wenfeng Li, Yidan Gao, Siyu Liu, Mingrui Luo, Zhu Liang, Guanren Qiao, Zhiping Xu  
**Data:** 2026-09-03  
**Categorie:** cs.AI, cs.MA  
**Link:** https://arxiv.org/abs/2609.03871v2

> Large language model agents have shown promise in bioinformatics, but most existing systems focus primarily on producing final answers, treating planning, tool use, and code execution as transient interactions. This design is poorly suited to long-horizon bioinformatics tasks, where conclusions must remain connected to the data, computations, and intermediate evidence that support them. We introduce \textbf{Bioinfoysis}, a multi-agent harness that represents each request as a persistent, artifact-grounded analysis run. Bioinfoysis combines global planning with step-wise, evidence-driven replanning: the planner maintains an executable checklist and revises pending steps using structured handoffs returned after each worker execution. These handoffs bind intermediate results to their responsible agent, checklist step, and plan generation, preventing stale evidence from being silently reused after replanning. A controlled runtime validates generated scripts, tables, and figures before they are used in downstream analysis or reporting, while role-specific context, persistent memory, and governed bioinformatics skills support reliable execution over long analysis trajectories. We evaluate Bioinfoysis on BixBench and two question-answering tracks of LAB-Bench 2. On BixBench, Bioinfoysis achieves state-of-the-art accuracy of 82.4\%. Across four underlying language models, Bioinfoysis increases average accuracy from 27.81\% to 64.13\% on SeqQA2 and from 3.13\% to 31.25\% on DbQA2. These results demonstrate that reliable bioinformatics automation depends not only on model capability, but also on the harness that governs planning, execution, memory, and evidence flow. We hope that the emergence of Bioinfoysis will play a driving and leading role in the development of the bioinformatics community. Our demo website can be seen in https://report.bioinfoysis.com/.

---

## 212. What Do CAE Simulation Agents Really Need Beyond a Generic Harness?

**Autori:** Jiasheng Shi, Tianhan Zhang  
**Data:** 2026-09-03  
**Categorie:** cs.CE, cs.CL, physics.comp-ph  
**Link:** https://arxiv.org/abs/2609.03718v1

> Computer-aided engineering (CAE) simulation is among the largest and most demanding areas of engineering, where setting up a solver such as OpenFOAM, FEniCS, or COMSOL takes real expertise. Large language model (LLM) agents promise to turn a natural-language request into a working simulation, and recent CAE agents add simulation-specific machinery: multi-agent decomposition, domain retrieval, and scripted reflection. That machinery suited weak base models; modern harnesses already supply multi-turn reasoning, tool use, and execution feedback. We ask what a CAE simulation agent still needs beyond a generic harness. With information access and repair budget held fixed, a single-agent harness matches or beats multi-agent specialized systems (FoamBench 96.4\% vs.\ 88.2\%). Ablations trace this to capabilities the harness already provides: execution-feedback repair lifts FoamBench from 71.8\% with no repair round to 96.4\%, while scripted reflection adds nothing. The one input that still helps is domain knowledge supplied as solver tutorials, our largest measured gain (80.9\% to 96.4\%).

---

## 213. Improving Evaluation Realism with Inference-Time Compute and Deployment Scaffolds

**Autori:** Axel Ahlqvist, Richard Guan, Juan-Pablo Rivera, Adeline Kassler, Dmitrii Troitskii, Alexandra Souly, Kai Fronsdal, Robert Kirk, John Hughes  
**Data:** 2026-09-02  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2609.02302v1

> A core obstacle to alignment evaluation is evaluation awareness: capable models can tell when they are being tested rather than deployed, weakening the conclusions a safety evaluation can support. We present two techniques that make simulated alignment evaluations harder to distinguish from real deployments. Our first technique, critique refinement, spends additional inference-time compute on each simulator action: the simulator generates multiple candidate actions, refines them using feedback from an instance of the target model on how to make them more realistic, and continues the evaluation with the most deployment-like candidate. Our second technique, DISH (Deployment-Imitating SWE-Agent Harness), wraps the target in an agent harness, reducing the gap between simulated and real deployment environments in coding settings. We test the techniques on multiple target models and find that they compose: applying both yields larger realism gains than either alone. Our results show that automated approaches can improve the realism of alignment evaluations, and that these improvements use additional compute more effectively than making the audits longer.

---

## 214. Measuring the Microtask Eligibility Gap: When Is an Off-the-Shelf SLM Enough for an Agent Harness?

**Autori:** Jundong Hu, Shekar Ramachandran  
**Data:** 2026-09-01  
**Categorie:** cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2610.00025v1

> Agent harnesses increasingly want to run small language models (SLMs) on the microtasks around a frontier large language model (LLM) planner: auto-approving shell commands, writing memory, selecting tools, ranking past turns. We ask whether off-the-shelf SLMs meet practitioner-defined thresholds and, when they fail, why, and whether quantization changes the answer. We build a benchmark of 4 such microtasks with fixed prompts and automatic metrics, each with a pre-specified threshold $τ$ anchored to a cheap non-LLM baseline and a CI-aware eligibility rule (a configuration passes only if its confidence bound clears $τ$). Sweeping Qwen3 0.6/1.7/4/8B at their best (FP16, greedy, one frozen prompt, no tuning), we find an eligibility gap: 0 of 16 (4 tasks $\times$ 4 models) configurations pass (verified by checking the raw outputs and parser behavior). A logprob decision-threshold diagnostic (T1/T3/T4; T2 via a context-length/cascade probe) separates the failures into capability deficits and failures that can be addressed by changing the decoding threshold (4 regimes). Quantization to 4-bit (RTN/GPTQ/AWQ) does damage that depends on model size and moves no configuration into eligibility (certified on the reconstructable hard-label tasks T1/T3, diagnostic/windowed robustness on T2/T4), so the gap tracks model size more than precision; it replicates on Llama-3.x (12/12 ineligible) and is robust to the anchor choice (a $τ$-sweep) and to prompt wording (0/112 eligible across the original plus 3 neutral paraphrases per cell). The practical implication: place SLMs behind a baseline that meets the CI-backed threshold, and use the SLM only where the baseline fails to meet the threshold; e.g. a 4B re-ranker over a BM25 shortlist beats BM25 ($+0.047$ [0.020, 0.073], without itself certifying eligibility).

---

## 215. CordisBench: Can Language Models Reason About Component Lifecycles in Dynamic Agent Harnesses?

**Autori:** Damien Sileo, Dimitri Kachler  
**Data:** 2026-09-01  
**Categorie:** cs.CL, cs.AI  
**Link:** https://arxiv.org/abs/2609.01600v1

> Dynamic agent harnesses let language models change the software that shapes their own execution. This flexibility brings a new reasoning burden: a local plugin change can propagate through dependencies and cleanup. We introduce CordisBench, a 1,200-question benchmark of this lifecycle reasoning. It combines a controlled formal setting with programs executed against Cordis, a runtime that manages component dependencies and cleanup, and asks models to identify affected components, predict state after a specified teardown order, determine which conditions hold under all or some orders, and choose reconfigurations that succeed when executed. Across these tasks, we evaluate three efficiency-oriented models at low reasoning effort with 2, 4, 8, 16, 24, or 32 relevant interactions, using deterministic task-specific scoring. Models usually handle small systems well but grow less reliable as more interactions become relevant, especially when predicting final state and when reasoning across teardown orders. Additional inference effort recovers marked gains for some models. The cost is nontrivial: on our 16-interaction subset, GPT-5.6 Luna uses nearly 3,000 reasoning tokens per question at medium effort. For these controlled instances, that cost is avoidable: an independent finite reference semantics agrees with Cordis execution on every observation and action outcome used for scoring across all 528 executable questions.

---

## 216. Harness-of-Harness: Multi-Day Autonomous Software Development with Continual Improvement

**Autori:** Haoyang Yan, Min-le Su, Hangfan Zhang, Zhanhao Li, Chen Zhang, Shao Zhang, Yang Chen, Lei Bai, Shuyue Hu  
**Data:** 2026-09-01  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.01481v1

> This paper studies autonomous software development, in which LLM-based coding agents transform high-level requirements into complete, functional, and usable software systems without human intervention. We introduce Harness-of-Harness (HoH), a framework that enables coding agents to continually improve software during autonomous development. HoH operates on existing coding-agent harnesses, and organizes their executions into iterative planning-coding-testing loops. To sustain improvement across loops, HoH balances repair with capability growth, scopes development into small and verifiable increments, separates implementation-time testing from independent evaluation, and constrains verifiable outputs rather than prescribing agent workflows. It progressively exposes deliverables, role-specific tools, and skills, encourages reuse rather than recreation, and maintains versioned project histories. On GameCraft-Bench, FrontierSWE, and ProgramBench, three harness-model pairs (Codex with GPT-5.5, OpenCode with DeepSeek-V4-Pro, and Pi with MiniMax-M3), HoH consistently outperforms the corresponding standalone harnesses, achieving an average relative gain of 52.25 percent and a maximum gain of 82.86 percent after three iterations. In a multi-day deployment with more than 70 iterations, HoH autonomously develops a first-person-shooter game, featuring a coherent storyline, fully implemented core mechanics, human-playable experience, polished visuals and integrated audio. Github: https://github.com/Flesymeb/HarnessOfHarness Project Page: https://flesymeb.github.io/HarnessOfHarness/

---

## 217. HarnessDev: Can LLMs Create and Evolve Their Own Agent Harness?

**Autori:** Yuhao Wu, Jingyuan Zhang, Jiajun Shi, Xinping Lei, Qingshui Gu, Yuxuan Zhang, Zexuan Wang, Chen He, Chen Huang, Maojia Song, Zhiyuan Zeng, Shaowen Wang, Jinkai Liu, Yunfeng Shi, Jiaheng Liu, Shen Yan, Wenhao Huang, Ge Zhang, Wenxuan Zhang  
**Data:** 2026-09-01  
**Categorie:** cs.SE, cs.CL  
**Link:** https://arxiv.org/abs/2609.01437v1

> As agents move from research prototypes to deployed tools, their capability increasingly depends on model-external execution infrastructure, commonly termed the agent harness. Changing this harness while holding model weights fixed can substantially alter task performance. Current agent evaluations typically report downstream performance under a chosen harness, leaving a model's ability to develop the harness itself comparatively underexplored. We introduce HarnessDev, a benchmark that shifts the unit of evaluation from task outputs to runnable infrastructure. HarnessDev covers two stages. In Creation, the agent starts from a minimal seed and a small number of cases, then builds a complete execution system. In Evolution, it starts from its own created harness and iteratively revises it using downstream execution feedback, with the goal of improving benchmark performance. We then evaluate each constructed harness on capability (task success on held-out benchmarks) and efficiency (execution-token cost). The reported Creation results cover six creator LLMs, four domains, and five downstream benchmarks totaling 2,207 unique downstream instances, with hidden evaluation tasks withheld from development. We find that generated harnesses remain substantially behind mature human-engineered references on code and on search and research, while matching or exceeding the selected references on writing and machine-learning experimentation, with large variation in execution cost. Evolution produces some performance gains, but they are unstable and transfer only partially to held-out tasks. Experiments with a fixed runtime model further show that the gains depend strongly on the model executing the harness, indicating limited transfer across models.

---

## 218. MemoryWalker: Stop Training Agents on Contexts They Never Saw

**Autori:** Zinco J, Xunjie Zhu, Shen Huang, Zhenyi Wang, Pengjun Xie, Jieping Ye  
**Data:** 2026-09-01  
**Categorie:** cs.LG, cs.CL  
**Link:** https://arxiv.org/abs/2609.00865v1

> Production agent harnesses such as Claude Code and Qwen-Agent compress context during rollout, but training under compression creates a conditioning problem: every eviction branches the effective history, so the learning object is a tree rather than a sequence. Existing linearizations either retain the rightmost path, causing time-travel leakage, or replay a depth-first traversal, causing train-inference mismatch. We introduce two exact, gradient-equivalent corrections: LogitTree, a segmented K-forward traversal, and a packed 4D attention mask. LogitTree requires K+1 backward passes; the 4D mask requires a custom kernel and white-box eviction records. We also propose SDCC (Self-Distillation for Conditioning Consistency), a single-backward-pass variational relaxation. At each eviction, it minimizes forward KL between the compressed student and a stop-gradient teacher on the reconstructed pre-eviction prefix. A residual per-junction KL of epsilon_KL gives an O(sqrt(epsilon_KL)) bound on the train-deployment total-variation gap. SDCC also applies to black-box harnesses. On seven web-search benchmarks with TC-RAG, AgentFold, MemexRL, Claude Code, and OpenCode, naive training inflates the train-rollout log-probability gap, especially on eviction-heavy batches. The exact methods stay at the no-compression floor, and SDCC substantially closes the gap, with lower logit drift and higher rollout rewards.

---

## 219. Agentic programs: an emerging form of scientific software in computational materials science

**Autori:** Yunsung Lim, Haekwan Jeon, Jaesun Kim, Jisu Kim, Seungwu Han  
**Data:** 2026-09-01  
**Categorie:** cond-mat.mtrl-sci, cs.AI  
**Link:** https://arxiv.org/abs/2609.00795v1

> Computational materials science has traditionally delegated algorithmic tasks to computers while leaving scientific judgments to humans. We argue that recent LLM-based agent harnesses enable an emerging form of scientific software, agentic programs, that combine deterministic algorithms with bounded LLM-based judgment, task-specific verification, episodic maturation, and complete delegation in production. We illustrate this concept with DeMARS, an agentic program for constructing atomistic models from experimentally measured disordered crystal structures.

---

## 220. mimeo: Compiling Public Expert Corpora into Agent Skills and Testing What Transfers

**Autori:** Timothy Kassis  
**Data:** 2026-08-31  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.00453v1

> Giving an agent a file about a named expert can supply hard-to-find material, produce a recognizable persona, or change what the agent decides. These are different claims. We test each one. mimeo is an open-source tool that finds a person's public work, checks each extracted quotation against the cached source text, and writes a file an agent can load. Eight logged builds averaged 38 model calls; the check rejects 13.2% of extracted quotations. We tested four expert files with one coding-agent harness. Knowledge access was clearest: mimeo answered all 20 obscure, quotation-heavy questions; no closed-book condition answered more than 10. Keyword search (BM25) over the same pages answered 15-17, a gap this sample cannot resolve. Grounding showed one clear benefit: personas written from model memory misstated a documented position on 1-4 of 20 answers under every grader; the plain agent and mimeo never did. Every persona was easy to spot on short open prompts, and adding task material lowered identification by 18-23 points. mimeo was no more identifiable than a from-memory profile. Judgment transfer remained unresolved because both tests hit their ceiling: every condition found 94-97% of the problems planted in engineering tasks and scored 94-100% on 16 new application scenarios. An AI-judged "sounds like the expert" score changed with the judge: two of four preferred answers based on a model's stereotype, while two found no difference on the same text. That is a caution against relying on a single AI judge. The evidence supports mimeo as a compact, inspectable reference on a person, not as a demonstrated transfer of their judgment. Toolkit and expert profiles: https://github.com/K-Dense-AI/mimeo

---

## 221. Aspire: Can Models Self-Evolve from Vague Goals?

**Autori:** Yuhao Wu, Jingyuan Zhang, Jiajun Shi, Yuxuan Zhang, Xinping Lei, Junting Zhou, Zexuan Wang, Yuchen Wu, Huan Zhou, Duo Wang, Yinzhu Piao, Yongchang Peng, Yunfeng Shi, Jin Chen, Zuo Wang, Jinkai Liu, Jiaheng Liu, Wenxuan Zhang, Shen Yan, Wenhao Huang, Ge Zhang  
**Data:** 2026-08-31  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2608.31111v1

> Many important forms of human learning begin with a vague goal, such as "become a better physicist" or "improve at research." Learners must interpret the goal, identify capability gaps, decide how to learn, and determine whether they have actually improved. In contrast, existing work on LLM self-evolution typically begins with tasks and evaluation metrics specified by humans, reducing self-evolution to optimizing an explicit objective rather than deciding what and how to learn. We introduce ASPIRE, a benchmark for vague-goal-driven self-evolution. ASPIRE provides only a natural-language capability goal while downstream evaluation tasks remain hidden. The agent must operationalize the goal by choosing data and update methods, constructing training and validation signals, and deciding when to evaluate. ASPIRE supports both model-weight and agent-harness evolution in a unified interactive environment and evaluates the resulting systems on a hidden, expert-authored set of 520 items spanning six goals. Our experiments show that vague goals redirect search effort toward goal interpretation. Current agents routinely complete training and harness-editing loops, but weight-level gains remain sparse and unstable, and the strongest evolved harness remains below the engineered Qwen-Agent reference. Agents often train on mismatched data and trust narrow self-evaluations, so local gains fail to transfer to hidden evaluation and continued search and training can erase earlier improvements.

---

## 222. Learning to Evaluate Before Improving: Automatic Rubric Induction for Automatic Research Agents

**Autori:** Xuehai Wang, Haowei Qin, Tongxin Liu, Junkai Li, Buqiang Xu, Jintian Zhang, Yijun Chen, Zirui Xue, Shumin Deng  
**Data:** 2026-08-31  
**Categorie:** cs.CL, cs.AI, cs.IR, cs.LG, cs.MA, cs.SE  
**Link:** https://arxiv.org/abs/2608.31076v1

> Autonomous scientific research agents are increasingly applied to end-to-end scientific workflows, including literature review, data analysis, experimentation, and report generation. However, open-ended research tasks often do not clearly specify the analyses, methods, and success criteria required to complete the task. As a result, agents may miss important analyses, use inappropriate methods, or draw conclusions that are insufficiently supported by evidence. To address the problem, we present AutoSciRub, an evaluation-first framework that induces a task-specific executable rubric before research execution, and uses it to guide execution, criterion-level verification as well as iterative revision. AutoSciRub decomposes an underspecified instruction into atomic scientific goals, grounds them in relevant literature and task-visible data, and synthesizes specific, actionable, and verifiable criteria. The resulting rubric makes implicit experimental and evidential requirements explicit, providing guidance for experiments and analyses. During revision, rubric-guided verification identifies unmet criteria and enables targeted refinement of the research report and its supporting artifacts. On ResearchClawBench, AutoSciRub consistently improves all tested configurations, with an average gain of 2.08 points across three backbone LLMs under the fixed Codex harness and 2.95 points across three agent harnesses using a fixed DeepSeek-V4-Flash backbone. On a randomly sampled 20-task subset of AstaBench E2E Discovery, AutoSciRub further achieves an average improvement of 16.8 points across three agent harnesses, while maintaining or increasing the number of successfully completed tasks. These results demonstrate that evaluation-first guidance provides an effective and generalizable control mechanism for autonomous scientific research (Code: https://github.com/zjunlp/AutoSciRub).

---

## 223. SkillZip Pro: Execution-Aware Dynamic Compression of Progressively Loaded Skills for Self-Evolving Agents

**Autori:** Xiaofan Bai, Chao Liu, Hongqiang Lin, Di Wu, Mingli Song, Xuan Jin, Xipeng Cao, Yuhong Li  
**Data:** 2026-08-31  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.30785v1

> Production agent skills are directory bundles, not isolated prompts. The root is loaded at activation; references, schemas, scripts, assets, and nested subskills are loaded only when an execution path needs them. Compressing only the root misses most deployment cost and may move branch-specific details into the always-loaded context. Flattening instead destroys progressive-loading boundaries. We introduce \method, an evaluation-free compressor for complete, progressively loaded skill bundles. It leaves the agent harness unchanged and emits an ordinary directory. The method combines two safeguards. First, it compresses \emph{across files}, removing content from a reference or subskill when the root or a declared environment contract already provides it. Second, it preserves routing, so every required file and directly callable entry remains reachable after rewriting. Users can configure \method along two independent axes. \emph{One-Shot} mode rebuilds the full bundle; \emph{Continual} mode reuses state and applies Zip-on-Write after each evolution patch. \emph{Persistent} compression rewrites the shipped bundle to reduce storage and runtime context. \emph{Transient} compression keeps that bundle byte-identical and builds a task-specific view, reducing only per-run context after build cost. Entry contracts mark private, public, and conditional resources; a multi-entry audit preserves standalone public subskills. On a production content-moderation skill evaluated by our industrial multi-round harness, \method removes \hl{38\%} of skill bundle tokens and \hl{10.4\%} of end-to-end per-run tokens with no quality loss, while an unprotected 71\% configuration loses up to 26 accuracy points to one-sided false positives. On a multi-entry bundle, \method effeciently reduces token cost while near-perfectly preserving every route and public entry.

---

## 224. Lies We Can See: Joint Verbal and Non-Verbal Deception by VLM Agents in Embodied Social Interactions

**Autori:** Jaewoo Ahn, Junseo Kim, Hyunseo Kim, Heeseung Yun, Jaehyeon Son, Zsolt Kira, Gunhee Kim  
**Data:** 2026-08-31  
**Categorie:** cs.CL, cs.AI, cs.CV, cs.LG  
**Link:** https://arxiv.org/abs/2608.30428v1

> Strategic deception by LLM and VLM agents has emerged as a central AI alignment and safety concern. Social-deduction games (where each player holds a hidden role and communicates with others to deduce identities) serve as the canonical testbed, particularly in multi-agent settings. Existing testbeds, however, are text-only and run on a single fixed agent configuration, missing the non-verbal sensorimotor channels treated as core by deception taxonomies and leaving it ambiguous whether an observed behavior reflects the underlying model or the surrounding harness. We introduce MineAmongUs, a 3D multimodal Among Us sandbox where imposter agents must deceive crewmates through joint verbal and non-verbal action. We also propose ARIA, a configurable VLM-agent harness that exposes five cognitive-component ablation axes; and an atom- and arc-level annotation scheme grounded in deception taxonomies and operationalized at scale by an LLM-as-a-Judge reaching near-human atom-labeling agreement. Empirical results show that VLM agents pursue imposter wins through joint verbal and non-verbal deception, with non-verbal channels emerging as the more decisive winning contributors across both harness ablation and cross-VLM evaluation. Taken together, our work opens a new path for embodied VLM-agent alignment research.

---

## 225. Last Step Matters: Early Uncertainty Cannot Predict Failure in Long-Horizon Agents

**Autori:** Zongyue Li, Chengyue Yu, Lei Zang, Chenyi Zhuang, Linjian Mo, Leilei Gan  
**Data:** 2026-08-30  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2608.29685v1

> Early failure prediction is important for long-horizon agents, as it enables timely intervention and can reduce inference and tool-use costs. Uncertainty quantification, such as verbal confidence and perplexity, offers a promising approach to detecting agent failures; however, it has not been explored whether these signals retain their discriminative power during the intermediate stages of long-horizon execution. We evaluate mainstream uncertainty signals on deep-research tasks and find that verbal confidence reliably distinguishes failures at trajectory completion, achieving a mean AUROC of 0.85, whereas all evaluated signals offer limited predictive value earlier in execution, with none exceeding a mean AUROC of 0.60 at 50% trajectory progress. We identify an underlying mechanism explaining this gap: path switching, where agents frequently abandon their current search direction in-trajectory, breaking the link between early signal and final outcome. These findings challenge the assumption that intermediate uncertainty can reliably guide early intervention. They also motivate a practical recommendation for agent harnesses in deep-research settings: use final-step confidence to decide whether to restart, an approach that our experiments find more effective than in-trajectory intervention.

---

## 226. Harness-RL: Black-Box Reinforcement Learning with Action-Args Decoupling for Central-Agent Multi-Agent Harnesses

**Autori:** Xinke Jiang, Zhixin Zhang, Zhibang Yang, Jiaran Gao, Rihong Qiu, Shijin Chen, Xu Chu, Junfeng Zhao, Yasha Wang  
**Data:** 2026-08-30  
**Categorie:** cs.MA  
**Link:** https://arxiv.org/abs/2608.29641v1

> Large language model agents increasingly solve long-horizon tasks through multi-agent harnesses in which a central agent coordinates specialized sub-agents, tools, and environments. Training the central policy in such a harness raises two challenges. First, an action label is a low-cardinality decision, whereas its args form a high-dimensional conditional sequence; optimizing both with a shared sequence-level signal can produce conflicting gradients. Second, dynamic scheduling creates interdependent sessions with branches, parallel calls, and rewritten contexts, which cannot be faithfully reduced to one flat token sequence. We introduce Harness-RL, a structured reinforcement learning framework that combines Conflict-Aware Policy Optimization (CAPO) with interface-level black-box trajectory construction. The black-box component captures Interface Call Records, builds per-session prefix trees, and aligns outcome and process rewards with trainable tokens. CAPO uses forward activations to identify parameter partitions associated with action and args tokens, then routes their policy gradients to the corresponding subspaces. Harness-RL supports both central-only and joint multi-agent training. Across seven multi-hop question answering and agentic retrieval benchmarks, it reaches average F1 scores of 42.93 and 47.79 with Qwen2.5-1.5B and Qwen2.5-3B, respectively, while ablations validate the contribution of CAPO and favor central-only optimization in the evaluated setting. Our code is available at https://github.com/jiangxinke/Harness-RL.

---

## 227. Graph, Loop, and Harness Engineering for Zero-Trust Agentic Data Engineering and Analytical Processing

**Autori:** Sagar Srinivas Sakhinana, Venkataramana Runkana  
**Data:** 2026-08-30  
**Categorie:** cs.LG, cs.AI  
**Link:** https://arxiv.org/abs/2609.29668v1

> Large language model agents increasingly automate data workflows, but end-to-end cloud data engineering and analytical execution require reliable coordination across code, data, infrastructure, and runtime environments. We present two zero-trust frameworks. Zero-Trust Agentic Data Engineering generates, deploys, and verifies complete cloud data-engineering solutions from natural-language tasks, with completion conditioned on repository, deployment, runtime, and policy evidence. Zero-Trust Agentic OLAP combines governed Data Preparation with verified Online Analytical Processing (OLAP), permitting production promotion only after validation and evidence-bound approval, and releasing analytical answers only after Same-Snapshot Execution, Exact Result Equivalence, deterministic grounding, and reflection. Both frameworks share three abstractions: graph engineering for evidence-gated workflow structure, loop engineering for bounded recovery, and agent-harness engineering for zero-trust execution. We evaluate both frameworks under nominal execution, controlled failures, bounded recovery, and policy-constrained conditions, measuring verified completion, recovery, authorization enforcement, production promotion, and verified OLAP execution.

---

## 228. Towards Agentic Cloud Engineering: Graph and Loop Engineering with a Zero-Trust Agent Harness

**Autori:** Sagar Srinivas Sakhinana, Venkataramana Runkana  
**Data:** 2026-08-30  
**Categorie:** cs.SE, cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2609.00050v2

> Agentic AI is enabling cloud-based workflows in which autonomous agents reason over operational state, invoke authorized tools, modify software and infrastructure, deploy services, verify execution outcomes, and adapt across long-horizon, multistep tasks. Engineering such workflows requires explicit mechanisms for workflow progression, constrained execution, failure recovery, and verifiable completion. We present Agentic Cloud Workflow Engineering, an agentic AI framework that transforms natural-language agentic cloud-engineering tasks into validated code repositories and verified operational cloud deployments for automating cloud-based agentic workflows. The framework separates three complementary concerns: graph engineering specifies long-horizon workflow progression and verification-dependent transitions; loop engineering provides bounded diagnosis, repair or re-planning, retry, and re-verification; and agent harness engineering enforces zero-trust execution through identity, authorization, policy-scoped capabilities, isolation, and runtime safeguards. Workflow progression and completion require machine-checkable repository, deployment, and runtime evidence, with recovery constrained by explicit operational bounds and termination criteria. We instantiate the framework on Google Cloud and evaluate repository completeness, controlled execution, evidence-gated progression, operational deployment, and bounded recovery. Experimental results show that executions terminate with either a verified operational cloud deployment or an auditable terminal failure under bounded recovery. The framework provides a unified engineering architecture for cloud-based workflows spanning Agentic DevOps, Agentic CloudOps, Agentic SRE/AIOps, Agentic SecOps, Agentic DataOps, Agentic MLOps/LLMOps, AgentOps, Agentic RAG/GraphRAG, and related cloud-engineering domains.

---

## 229. Forward-Deployed Full-Stack Engineering for Autonomous Cloud MLOps

**Autori:** Sagar Srinivas Sakhinana, Venkataramana Runkana  
**Data:** 2026-08-30  
**Categorie:** cs.MA, cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2608.29615v2

> Across industries, machine-learning systems support applications ranging from prediction and anomaly detection to forecasting, optimization, and scheduling, yet operationalizing these systems requires coordinating application development, model pipelines, cloud infrastructure, security, deployment, monitoring, retraining, recovery, and rollback. We present an evidence-gated multi-agent framework for transforming a natural-language MLOps cloud engineering task into a verified repository and operational cloud deployment. The framework combines graph engineering, loop engineering, and agent harness engineering. A stateful Graph Orchestrator coordinates specialized agents for repository generation, review, execution, verification, release, and monitoring while governing workflow dependencies, evidence gates, retry bounds, recovery paths, and termination. Consequential lifecycle transitions proceed only when their required predicates are supported by verifiable execution or runtime evidence. Verification failures activate bounded reflection, repair, and re-verification, while runtime evidence of failure, drift, degradation, or policy violation can trigger bounded adaptation, recovery, or rollback. Agent harness engineering constrains repository generation, review, and repair, artifact execution, and cloud operations through controlled capabilities and isolated execution environments. We realize the framework on Google Cloud Platform and evaluate repository completeness, controlled execution, evidence-gated transitions, cloud promotion, and bounded recovery. Our experimental results show that the framework prevents unsupported lifecycle transitions and drives each run toward either a verified operational deployment or an auditable terminal failure.

---

## 230. EvoUndo: Recoverability-Constrained Self-Evolution for LLM Agent Harnesses

**Autori:** Tanmay Sah, Dolly Sah, Harshul Jain, Tanya Sah  
**Data:** 2026-08-28  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.28363v2

> LLM agents increasingly modify their own prompts, tools, middleware, resources, and execution harnesses at runtime. Such self-evolution can improve capability, but a successful mutation may leave persistent effects that cannot be safely reversed in states different from the one in which it was created. We introduce EvoUndo, a framework for representing, synthesizing, diagnosing, and independently verifying recoverability of model-generated self-modifications across counterfactual states. Across 600 unseen one-shot self-evolution tasks, we identify 197 capability-improving mutations that fail recoverability verification. Under the original recovery representation, conventional repair strategies recover 0/197 of these natural failures. Deterministic oracle analysis recovers 48/197 under the original recovery language L0, while the extended recovery calculus increases empirical oracle recovery to 191/197. A protocol-locked 2x2 grounding-by-expressivity intervention then separates two bottlenecks: exact state-address grounding increases successful recovery from 0/48 to 38/48 (79.2%) when the original language is sufficient, while extending the recovery language enables recovery on 142/143 (99.3%) failures in the oracle-defined S1 stratum. On the primary gpt-oss-120b backbone, adding exact-address diagnostics to the richer language reduces recovery to 133/143 (93.0%); a Qwen3.8-27B replication preserves the grounding and expressivity effects but not this negative interaction, indicating that the latter is model-dependent. These results indicate that reliable agent self-evolution requires co-designing verification, state grounding, witness semantics, and recovery-language expressivity rather than relying on iterative prompting alone.

---

## 231. WeAgent-MMSearch: Native Text-Vision Interaction for Multimodal Search Agents

**Autori:** Zongkai Liu, Hui Zhang, Liqiang Niu, Zhen Cao, Han Li, Juntao Liu, Wenchao Chen, Chengduo Zhao, Chao Yu, Fandong Meng  
**Data:** 2026-08-28  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.28062v2

> Multimodal search agents extend parametric knowledge with newly emerging and long-tail evidence from the open web. Yet many existing agentic search environments often expose retrieved evidence only as text and omit tool-returned images from subsequent context, reducing visually grounded trajectories to text-only reasoning. Long-horizon interaction also compounds tool-call, response-length, timeout, and budget failures, which can discard salvageable trajectories, waste rollout computation, and disturb policy updates. To address these issues, we introduce WeAgent-Harness, a multimodal agentic harness that supports native text-vision interaction and runtime recovery. Retrieved images receive persistent disk references, allowing the model to inspect, process, and cite them throughout the trajectory. Based on this harness, we develop WeAgent-MMSearch, an integrated system spanning data construction, agentic post-training, and multimodal rollout. For data construction, a strong MLLM uses WeAgent-Harness to discover, synthesize, and verify MMSearch-style tasks and collect expert trajectories. During post-training, our Failure-Aware GSPO (FA-GSPO) recovers salvageable abnormal rollouts and filters invalid ones to improve bounded multimodal planning and search. We also introduce VisTarget-Bench, a 150-task human-verified benchmark that pairs each question with a held-out target image, distinguishing image-retrieval failures from visual-perception failures. Evaluation on VisTarget-Bench and seven public benchmarks shows that agentic post-training improves the average score by 19.22 points, enabling our model to outperform similarly sized open-source models and rival models with roughly ten times its parameter count.

---

## 232. openJiuwen: Beyond Static Harnesses for Long-Horizon Coding Agents

**Autori:** openJiuwen Team, Tao Yu, Xinyu Zhang, Qianqian Chen, Xiaoneng Xiang, Chia Kwangyang, Xingchen Huang, Ran Chen, Yangkai Ding, Zheng Wang, Yeo Boon Hong, Bingzheng Gan, Enrui Hu, Shuo Cheng, Deyang Li, Ruifeng Shi, Hongbo Wang, Qi Ye, Xuefeng Jin, Zhangchun Zhao  
**Data:** 2026-08-28  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.27969v1

> Long-horizon coding agents operate over evolving repository states while increasingly relying on heterogeneous capabilities, delegated agents, and multi-agent coordination. These trends pose two complementary challenges for the agent harness. First, developers need to compose capabilities, reconfigure execution logic, and scale increasingly complex agent systems without repeatedly rebuilding orchestration. Second, complex coding tasks continuously produce new evidence---such as semantic diagnostics, execution outcomes, task progress, and changing context relevance---that should dynamically influence subsequent runtime decisions. We characterize these challenges as Structural Composability and Runtime Adaptivity. We present openJiuwen, an open-source harness designed for both developer composability and adaptive task execution. openJiuwen provides a shared execution substrate and Rail-based capability composition across single agents, delegated sub-agents, and Swarm Flow, enabling developers to construct sophisticated agent harnesses under common execution semantics. It further adapts framework-controlled runtime decisions around a fixed model policy, allowing evolving evidence to dynamically affect context, feedback, and task control toward successful completion. We systematically evaluate openJiuwen on SWE-bench Verified and Terminal-Bench 2.1, where it achieves 82.6% and 87.19%, respectively, exceeding the strongest selected official-leaderboard point estimates by 3.4 and 3.39 percentage points. These results show that openJiuwen achieves strong performance on complex coding tasks while providing a composable and adaptive harness design.

---

## 233. Verify Smarter, Evolve Further: Efficient Harness Evolution through Behavior-Aware Verification

**Autori:** Jinghan Xu, Yikai Zhang, Aili Chen, Weiyuan Li, Jiaqing Liang, Deqing Yang  
**Data:** 2026-08-27  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.27311v1

> Agent harnesses shape how language-model agents use instructions, tools, and runtime components, but adapting these harnesses requires costly verification. Existing propose-and-verify methods typically score every candidate on a fixed task set, wasting rollouts on unrelated behaviors and allowing aggregate scores to obscure specific regressions. We introduce HarnessLens, a budget-aware framework for automated harness evolution. HarnessLens jointly explores the task space and user-configurable components, derives candidate modifications from execution trajectories, and selectively verifies each candidate on behavior-relevant tasks using an attributable-evidence gate. Across three agent harnesses and four benchmarks, HarnessLens improves average held-out performance by 7.6-13.6% while consuming substantially less evaluation budget than competing baselines. These results demonstrate that behavior-aware verification with explicit attribution enables more reliable and sample-efficient harness evolution under constrained interaction budgets. Our code is available at https://github.com/jhxu5214/HarnessLens.

---

## 234. JIT-Agent: Scaling Harness Intelligence via Just-in-Time Harness Evolution

**Autori:** Guibin Zhang, Leo Lu, Fangzhou Xie, Kang Zhu, Junhao Wang, Zhifei Xie, Zhaochen Yu, Zihang Liu, Zhongxiang Sun, Qiankun Li, Yue Liao, Heng Chang, Xiaobin Hu, Qibing Ren, Wangchunshu Zhou, Chuanrui Hu, Yafeng Deng, Shuicheng Yan  
**Data:** 2026-08-26  
**Categorie:** cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2608.25593v2

> Agent capability is not determined by the model alone. The agent harness, encompassing memory management, planning strategy, action protocol, and tool/skill orchestration, can dominate the contribution of the underlying foundation model. Yet harness design remains manual, task-specific, and fundamentally unscalable. We present JIT-Agent, a harness intelligence model trained to synthesize task-adaptive agent harnesses on the fly for arbitrary off-the-shelf agentic LLMs. We formalize the agent harness as a composable, machine-generatable artifact governed by a fixed four-module protocol, and train JIT-Agent to customize harnesses for a given task at hand, repair harnesses for stable and reliable execution, and self-evolve by distilling performance signals from an expanding archive of prior harness configurations. Equipped with JIT-Agent as a harness helper, DeepSeek-V4-Flash surpasses GPT-5.6 on DeepSearchQA (+9.1) and OdysseyBench (+4.3), while the already strong GLM-5.2 gains up to +20.2 points. Across controlled evaluations, JIT-Agent-generated harnesses are performance-competitive with mature agent runtimes such as OpenCode and Claude Code and consistently improve multi-scale model families of DeepSeek V4, Mimo-V2.5, and Qwen3.6. To our knowledge, JIT-Agent is the first model purpose-built for just-in-time harness generation, establishing harness intelligence as a trainable, transferable, and compounding dimension of agent capability orthogonal to model scaling.

---

## 235. Recursive Experiential-Working Memory Evolution for Long-Horizon Agent Harnesses

**Autori:** Zhaochen Yu, Yingcheng Wu, Zhenfei Yin, Kaiyuan Chen, Zhe Zhao, Mengdi Wang, Shuicheng Yan, Ling Yang  
**Data:** 2026-08-25  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2608.24876v1

> Recursive self-improvement (RSI) remains hard in long-horizon tasks, where growing histories obscure the task state and misalign skill invocation. We introduce Recuris, a recursive Experiential-Working Memory architecture for long-horizon agent harnesses, in which Working Memory tracks task progress and guides skill selection from Experiential Memory, grounding skill use in current needs rather than the full history. This coupling also turns execution into structured evidence that localizes failures to specific memory components. Across tasks, a fixed Meta-Agent turns that evidence into localized, validation-gated updates to Skill Memory that reshape execution and yield new evidence, forming a bounded recursive memory-evolution loop. Across four long-horizon benchmarks and ten models, Recuris improves task success in 35 of the 37 completed model-benchmark pairs, carrying frontier models to SOTA-level task success: on tau-bench it adds +17.8 points to GPT-5.6 Sol and +15.6 to Claude Opus 5, taking Opus 5 to 87.9%, and +16.6/+13.5 points on Qwen3.6-27B/35B on SkillFlow. The advantage widens as the interaction horizon grows, to +32.2 points on the longest tasks, and common long-horizon failures fall by up to 80%. These results position recursively evolving memory as a scalable foundation for RSI, enabling agents to continuously transform accumulated experience into increasingly effective long-horizon behavior. Code: https://github.com/Gen-Verse/Recuris

---

## 236. StarHarness: Evolving Harnesses with Stratified Search for Enterprise Environments

**Autori:** Esakkivel Esakkiraja, Denis Akhiyarov, Vikas Yadav, Sai Rajeswar, Patrice Bechard, Sridhar Nemala, Sagar Davasam  
**Data:** 2026-08-25  
**Categorie:** cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2608.24804v1

> We present StarHarness, a framework for evolving environment-specific agent harnesses while keeping model weights fixed. The evolved harness can include prompt and task framing, tool interfaces, skills, MCP-backed providers, subagent structure, and agent-loop configuration. StarHarness constructs a compact evolution pool by stratifying tasks according to baseline failure behavior, separates proposer-visible search tasks from proposer-hidden selection tasks, and reserves held-out tasks for evaluating generalization. Across ITBench SRE, EnterpriseOps-Gym ITSM, and AutomationBench Finance, harness evolution improves full-benchmark performance by 20-35 percentage points over the default harness after 4-12 accepted changes per environment. These gains persist on tasks excluded from evolution and transfer without re-evolution across GPT and Qwen model families. Trace analysis links the improvements to interface repairs, environment conventions, and operational knowledge that compresses search, with fewer false-positive diagnoses and shorter trajectories in several settings. StarHarness therefore offers a practical way to reduce persistent model-environment mismatch in tool-rich enterprise tasks.

---

## 237. The Empire, Long Divided, Must Unite: Architectural Convergence in Three LLM Agent Harnesses

**Autori:** Dai Jiahong  
**Data:** 2026-08-25  
**Categorie:** cs.SE, cs.AI, cs.CE  
**Link:** https://arxiv.org/abs/2608.23953v1

> An agent harness is what turns a language model into an autonomous agent: the surrounding code that builds the model's context, mediates its tools, runs the loop, and persists state across a long-horizon run. This layer, not the model it wraps, is increasingly the binding constraint on agent behaviour. We present a source-level, multi-case study of three open coding-agent harnesses built from deliberately opposing philosophies: LangChain's deepagents (batteries-included), Earendil's pi (radical minimalism), and DeepSeek's dsh (everything-is-a-plugin). Reading each at a pinned commit and following its commit history, we find that the two mature harnesses have travelled in opposite directions (deepagents subtracting authored scaffolding, pi accreting durable infrastructure), yet converged toward one architectural middle form of five recurring elements: a commoditised loop, an append-only replayable session record, model quirks kept as data, progressive disclosure of context, and explicit extension seams. A third harness, read afterward as a held-out check, exhibits all five, and in one seam reuses another's implementation outright. We therefore do not claim independent invention, and decompose the convergence into parallel discovery, diffusion, and literal reuse. Finally, one load-bearing dimension shows no convergence, and indeed no presence: external verifiability, a tamper-evident record an outside party can check without trusting the runtime. We read this absence not as an oversight but as a predictive gap, the next axis on which harnesses for provenance-sensitive domains will differ.

---

## 238. Beyond Executable Models: The Pufibara Agent Harness and the Modelica Agent Workflow Benchmark for Physical System Modeling

**Autori:** Zizhe Wang  
**Data:** 2026-08-24  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2608.23653v1

> AI agents are increasingly used for simulation-driven engineering. Physical system modeling presents different requirements from general-purpose code generation in software engineering, because correctness depends not only on syntax and executability but also on physical consistency and scenario-dependent behavior. We study this challenge in Modelica, an equation-based modeling language in which a model may compile and simulate while still violating its intended physics or engineering requirements. Across successive revisions, an agent may lose track of requirements or rely on simulation evidence produced by an outdated candidate. To address this challenge, we present Pufibara, an agent harness that maintains persistent engineering state across revisions, associates execution and simulation evidence with the candidate that produced it, and makes submission an explicit agent action. To evaluate end-to-end Modelica agent workflows, we also propose a source-grounded method for constructing realistic and independently evaluable tasks. We use this method to build the 232-task Modelica Agent Workflow Benchmark, spanning Model Repair, Model Generation, and Model Tuning. Each submitted candidate is scored by a benchmark-owned evaluator outside the agent loop. We compare Pufibara with Claude Code as complete harnesses under two matched large language model (LLM) backends. With DeepSeek v4 Flash, Pufibara passes 202 tasks, compared with 185 for Claude Code. With Claude Sonnet 5, Pufibara passes 202 tasks, compared with 187 for Claude Code. Under the repository-reported token accounting, Pufibara records 76.4%-82.5% lower logical-token totals. Its sequential runtime is 6.1%-58.4% lower. These findings show that, even under matched LLM backends, complete agent harnesses can differ substantially in both task success and resource use for physical system modeling.

---

## 239. Feedback That Backfires: Why Small Language Model Agents Repeat the Call They Just Watched Fail

**Autori:** Esmail Gumaan  
**Data:** 2026-08-24  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2608.23651v1

> Agent harnesses record a failed tool call and its error message in the transcript and ask the model to continue, on the assumption that the error is corrective information. We measure whether it is. Defining the corrective gain of a failure record as the change in log-probability of re-emitting the action that just failed, we find the gain is negative for every instruction-tuned model we tested (6 checkpoints, 135M-1.7B, 4 families) in two environments: simulated tool calling and MBPP program repair. Normalised by action length the effect is about -1.03 nats per action token, a factor of 2.8 in the odds of each token, and holds on 90%-100% of individual items, not only on average. Over a fixed candidate set the probability of repeating the failed call rises from 0.06 to 0.54, and greedy decoding reproduces it token for token on 19% of items after the failure versus 0% before. Counterfactuals pairing the same call with a failure message, a success message, or a neutral acknowledgement separate two effects: the failed call's surface form accounts for 83% of the damage, while the semantic contribution of marking it failed is small and inconsistent in sign across environments. The problem is in the harness, not the model's grasp of error messages, and that predicts which remedies work. Replacing the verbatim call with a runtime-generated description of the failure removes 76% of the inversion at no token cost, and making previously-failed strings unreachable at the decoder acts on the same term. Two plausible remedies do not: an explicit "do not repeat" instruction leaves the measured quantity where it was, and deleting the failed attempt to retry from a clean context, the standard prescription for context contamination, is the worst harness we measured for repetition, because it restores the context that produced the failure. The study runs end to end on a CPU; all artefacts are released.

---

## 240. Learning Generalizable Behaviors for Terminal Agents

**Autori:** Yihang Yao, Bo Pang, Xuan Phi Nguyen, Ding Zhao, Shafiq Joty, Semih Yavuz  
**Data:** 2026-08-23  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2608.22631v3

> Terminal agents are a compelling application of large language models (LLMs), with the potential to integrate deeply into users' daily workflows. Reinforcement learning (RL) is a key technique for improving their capabilities, making scalable training environments a central challenge. Since public real-user interaction data are scarce, synthetic environments provide a practical alternative, but often suffer from domain gaps and limited fidelity, leading to poor generalization. Existing work mainly scales the quantity and diversity of synthetic environments, while reward-signal quality and the mechanisms governing generalization remain under-explored. We study how RL improves terminal agents and propose the Agentic Compositional Generalization hypothesis: rather than teaching new domain-specific skills from scratch, RL primarily shapes high-level decision-making behaviors that compose and route low-level skills acquired during pre-training and supervised fine-tuning (SFT). This account is consistent with our empirical results and suggests that verifier quality, which determines which behaviors are reinforced, is more important than simply increasing environment quantity or diversity. Motivated by this insight, we propose River, a simple training recipe that improves reward quality by filtering low-quality environments and augmenting outcome rewards with process-level behavior regularization. Using this recipe, our RL-trained agent achieves the best performance among evaluated open-source RL-trained 8B models across four terminal-agent benchmarks. River also generalizes across model families, scales, agent harnesses, and RL objectives. Using fewer than 30% of the TMax training environments, River improves RL gains by 106% and 30% on average for models ranging from 2B to 27B on Terminal-Bench-Lite and Terminal-Bench-v2.1, respectively.

---

## 241. HiMA-MDD: A Hierarchical Multi-Agent Harness for Interpretable Multimodal Depression Detection in Clinical Interviews

**Autori:** Ao Chen, Xiaojiang Peng  
**Data:** 2026-08-22  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.21868v1

> Depression assessment from multimodal clinical interviews requires integrating dispersed evidence from multiple symptoms into a coherent PHQ-8 profile. This process is hierarchical: relevant evidence is often sparse and context-dependent within local question-answer exchanges, multiple exchanges jointly support symptom-level judgments, and the final assessment depends on the coherence of the complete symptom profile. Existing LLM systems either process interviews holistically or distribute work across generic agent roles; neither design necessarily provides an explicit orchestration mechanism that coordinates evidence access, item-score authority, bounded feedback, and state recording across these levels. To address this gap, we introduce HiMA-MDD, a hierarchical multi-agent harness that aligns this assessment hierarchy with three agent layers. After non-agentic preprocessing constructs context-preserving multimodal QA units, Layer 1 identifies candidate QA-to-item relations and supports bounded item-grounded evidence routing. Layer 2 assigns symptom groups to operational factor specialists, with one specialist responsible for each provisional item score. Layer 3 audits the complete provisional profile, requests at most one round of targeted revision, and reconstructs the verified PHQ-8 profile. This layered design naturally yields a Hierarchical Evidence Trace, preserves all intermediate evidence, judgments, and revisions for auditability. The final item scores then deterministically produce the total score and screening decision. Using Qwen2.5-72B-Instruct as the harness backbone, our experiments on E-DAIC demonstrate that HiMA-MDD outperforms the compared state-of-the-art methods.

---

## 242. Large Language Models at the Intersection of Software Engineering and Software Security:An Evidence-Centered Structured Survey and Research Agenda

**Autori:** Wei Lin, Tao Zhou, Zhaofei Xie, Changgui Hong  
**Data:** 2026-08-21  
**Categorie:** cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2608.21107v1

> Large Language Models (LLMs) are moving from code completion toward repository-scale agents that retrieve context, edit files, execute tools, and participate in security-sensitive workflows. The evidence for these systems, however, remains divided between software engineering evaluations centered on functional task completion and software security evaluations centered on vulnerability detection, secure generation, or exploit-oriented validation. This evidence-centered structured survey synthesizes representative work available through May 31, 2026 across software engineering tasks, software security tasks, adaptation mechanisms, artifact granularity, and evaluation design. In addition to a task taxonomy, we introduce an assurance framework that separates functional correctness, security, operational reliability, evidence provenance, and agent authority. The review shows that execution feedback and repository access can substantially improve engineering task completion, but do not by themselves establish security; conversely, static-analysis labels or vulnerability-classification scores rarely establish deployable correctness. We identify recurring validity threats--weak test oracles, duplicated and temporally leaked data, changing agent harnesses, proxy-only security checks, and under-reported budgets and human intervention--and derive a minimum reporting protocol for cross-study comparison. The resulting research agenda prioritizes jointly secure-and-functional benchmarks, repository-scale threat models, calibrated human oversight, longitudinal maintainability evidence, and reproducible agent evaluation. The central conclusion is that model capability should be judged as an assurance case supported by task-appropriate evidence, rather than by a single benchmark score.

---

## 243. ClawSentry: A Progressive Multi-Tier Security Monitor for Safeguarding Autonomous LLM Agents

**Autori:** Kai Wang, Zeming Wei, BiaoJie Zeng, Chang Jin, An Wang, Xiaokun Luan, Zhixiao Lin, Jingjing Qu, Xia Hu, Xingcheng Xu  
**Data:** 2026-08-21  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2608.21101v1

> As large language model (LLM) agents move from conversation to executing code, reading local files, and orchestrating external tools, a single agent hijacked by a malicious third-party skill can cause data exfiltration, privilege escalation, or cascading compromise. We argue that agentic risk is progressive: it can enter at four loci of the agent control loop--skill admission, invocation-time intent, execution-time effect, and post-action consequence--while a denied dangerous objective can reappear across surface forms, tools, or turns; existing safeguards are typically local to one lifecycle boundary or one call. Guided by this threat model, we present ClawSentry, an open-source, framework-agnostic security supervision gateway for agent runtimes. Before a skill package is ever executed, First-use Skill Package Review (FSPR) audits it under a deterministic evidence floor, escalating unresolved cases to bounded read-only agentic review (locus A). At runtime, a three-tier progressive decision engine--a deterministic L1 layer, a rule-anchored L2 semantic reviewer, and a read-only L3 evidence-seeking agent--spends contextual review only on the residual ambiguity, while a session-level anti-bypass mechanism recognizes tool-switching and rephrased retries (loci B--C); a post-action path feeds high-severity evidence non-retroactively into later review (locus D). An Agent Harness Protocol (AHP) abstraction applies one policy across Codex, Claude Code, Kimi CLI, and Gemini CLI without modifying agent internals. On SkillInject with Codex/GPT-5.4, contextual ASR falls from 39.55% to 2.61% while contextual TSR moves only from 83.78% to 83.05%. Across five Work Agents on the full SkillsSafety benchmark, ClawSentry confines ASR to 9.09--15.03% from 33.5--49.7% unprotected, and aggregate TSR on clean skills remains 98.7%.

---

## 244. Benchmarking General Mobile Assistants in Challenging Real-World Scenarios

**Autori:** Yiqi Zhu, Feiyu Gao, Jiaxing Fan, Jiahui Zeng, Minggang Wu, Chenliang Li, Haiyang Xu, Peng Li, Ming Yan, Yang Liu  
**Data:** 2026-08-21  
**Categorie:** cs.AI, cs.CV  
**Link:** https://arxiv.org/abs/2608.27477v1

> Graphical user interfaces have emerged as an important environment for evaluating autonomous AI agents on multimodal interactive tasks. Existing benchmarks such as AndroidWorld and MobileWorld provide strong foundations for mobile agent evaluation, but their application coverage and task design do not yet fully capture the diversity and complexity of realistic mobile use. We present GMA, a benchmark for evaluating general mobile assistants in challenging real-world scenarios. GMA introduces seven applications based on open-source projects, spanning domains such as lifestyle sharing and travel planning, and 300 tasks across four difficulty tiers, from atomic actions to complex multi-step workflows. We evaluate eight frontier models and find that performance declines substantially as task complexity increases, with current agents remaining far from reliably handling realistic user requirements. We further conduct controlled ablation studies of agent harness choices, including context retention and explicit state tracking, under a shared environment, model setting, and task taxonomy. Results show that appropriate harness design can meaningfully improve performance, particularly on demanding workflows, while the effectiveness of specific designs can vary across foundation models. Overall, GMA complements existing benchmarks by expanding application coverage and task complexity, providing a challenging testbed for evaluating mobile agents and studying how harness design supports reliable execution in complex mobile workflows.

---

## 245. BC-Bench: Evaluating Agentic Engineering in a Domain-Specific Language for ERP

**Autori:** Haoran Sun, Klaus Marius Hansen  
**Data:** 2026-08-21  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2608.20851v1

> Agentic engineering systems have shown strong performance on general-purpose benchmarks, yet their effectiveness in enterprise resource planning (ERP) domain-specific languages (DSLs) remains underexplored. We introduce BC-Bench, a benchmark designed to evaluate agentic engineering on real-world tasks in AL, the DSL for Microsoft Dynamics 365 Business Central. BC-Bench comprises 101 manually curated tasks extracted from two Microsoft-owned production repositories, reflecting authentic ERP development workflows. Adapting the SWE-Bench methodology, we address the unique constraints of the AL ecosystem---including limited public resources and complex environment provisioning. Beyond generating functional code, BC-Bench evaluates test generation and supports multimodal problem statements where visual context is commonly present. We evaluate multiple frontier models across two agent harnesses, utilizing multi-run metrics to account for nondeterminism. In the Bug Fixing category, under our evaluated settings, between-model differences in resolution rate are larger than differences between the two evaluated agent harnesses, and improvements reported on general-purpose benchmarks do not consistently transfer to AL. These results highlight the need for domain-specific evaluation.

---

## 246. Applying Anthropic Primitives at Large Enterprises: Harness Paradigm for Knowledge Work

**Autori:** George Juraj Salapa  
**Data:** 2026-08-20  
**Categorie:** cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2608.20622v1

> Frontier models have collapsed the cost of writing custom code: a niche problem a specialist sees in their own domain now costs an afternoon. The cost of reviewing and maintaining that code hasn't collapsed. Each solution drifts from the next; understanding one means reading its codebase from scratch. Large enterprises build something centrally governed instead: at worst an off-the-shelf product, at best a graph-orchestration framework wired bespoke per use case, or a low-code platform used as the orchestrator. These are custom every time and limited in scope. Enterprises don't weigh a third option that escapes both constraints: the harness paradigm. Recent work treats the coding-agent harness as enterprise infrastructure rather than a coding tool, converging on three findings: harnesses suffice at the task level and outperform more elaborate architectures on enterprise work (arXiv:2604.00073, arXiv:2604.13107); harness choice accounts for most of the variance in agent benchmark results, more than model choice does (arXiv:2605.23950); and the gap between that finding and enterprise adoption is governance (arXiv:2605.10223, arXiv:2605.18747). We propose an architecture that closes that gap. One harness runs unmodified as the backbone; the code stays identical across every deployment, so reviewing what gets built collapses to reading its instructions file. Section 4 gives four mechanisms: credential-scoped tooling, where each backend gets one generic request tool and a scoped credential instead of a hand-built method; authorization logic outside the harness, so one artifact runs as a cron backbone, a chat-surface engine, and a terminal tool; registration is a side effect of pushing code, collapsing an audit a review of a text file. Built on microcc (<https://pypi.org/project/micro-cc/>), our reference harness.

---

## 247. Bounded Loops: Pre-Run Spend Bounds, Proved Termination, and Verified Completion for Agent Harnesses

**Autori:** Varun Pratap Bhardwaj, Garima Singh, Arun Pratap Bhardwaj  
**Data:** 2026-08-20  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2609.27871v1

> In mainstream agent frameworks, a step ends when the agent's own output says it has finished. Durable-execution platforms bound retries and time, but their checker conventionally lives in the same codebase as the work: a discipline the deployment is trusted to keep, not a property the harness enforces. We state what an agent harness must guarantee, prove it, and build the instrument that measures whether a harness delivers it. A bounded loop is a worker, an independent gate the worker cannot write to, and a declared budget; a bounded-loop graph composes them with a repair relation that lets a downstream failure re-run a finished upstream node. Three guarantees follow. It finishes: termination holds under repair, with the worst-case attempt total in closed form, if the repair budget is global not per node. It does not drift: no node reaches DONE without a gate verdict in an append-only hash-chained ledger, proved from control flow, since repair leaves no topological order to induct along. It does not overspend: the ceiling is enforced inside an attempt, not between attempts. Gates are measured against a two-tier held-out mutant corpus. We characterise two classes that let a sound-looking check pass anything: vacuity, satisfied by the absence of the thing checked, and self-attestation, where the subject supplies the value the check is applied to. On a 69-loop catalogue the instrument found 47 vacuous gates in shipped, reviewed code. Against the repaired gates it reports no false accepts over 209 destroying mutants ($α\le 1.8\%$, Wilson 95%); that figure is saturation, not quality: freezing the gates and applying a fresh operator family recovers a 23.3% false-accept rate where the exhausted corpus reported none. A rate belongs to a specific gate; the apparatus, not our number, is the contribution. Engine, catalogue and corpus are Apache-2.0.

---

## 248. CTIFoundry: An Agent-Native Corpus Scaffold for Cyber Threat Intelligence

**Autori:** Yutong Cheng, Changze Li, Qian Cui, Wei Ding, Lingzhi Wang, Yan Chen, Peng Gao  
**Data:** 2026-08-19  
**Categorie:** cs.AI, cs.CR  
**Link:** https://arxiv.org/abs/2608.18613v2

> Cyber threat intelligence (CTI) is increasingly consumed not by human analysts but by LLM agents that compose multi-step investigations at query time. The harness side of this shift has matured rapidly, but the corpus side has not: threat reports and vulnerability databases are still packaged for retrieval-augmented generation, as opaque chunks behind an embedding index. We argue that this substrate, not model capability, is the bottleneck on agentic CTI investigation, and present CTIFoundry, an agent-native corpus scaffold. At build time, CTIFoundry materializes the latent structure of a CTI corpus: a deterministic ontology graph over four authoritative knowledge bases (CVE, CWE, CAPEC, ATT&CK) whose official cross-references become typed, traversable edges; a span-grounded report layer whose canonical, alias-resolved cross-vendor entities index provenance-carrying chunks; and hybrid dense+lexical retrieval surfaces. At query time this structure is exposed through seven typed tools and three procedural skills mounted on a stock, widely-used open-source agent harness. On the public CTIConnect benchmark, swapping only the action surface lifts the identically-harnessed agent from 0.610 to 0.829 overall F1 with gpt-5.4 and from 0.470 to 0.745 with claude-haiku-4-5: a small model on CTIFoundry surpasses a flagship model on the flat substrate. The scaffolded agent is simultaneously more accurate and more efficient: on both Claude models it answers with roughly half the tool calls per question. The ablation distills design principles for matching corpus scaffolding to data modality, in CTI and beyond. Build-time validation guarantees zero fabricated identifiers by construction, and the scaffold sustains 1,168 investigations end-to-end at about 2.6 cents each.

---

## 249. StartupBench: Benchmarking General-Purpose Agents on Market-Validated End-to-End Workflows

**Autori:** Liya Zhu, Xin Ma, Tao Liu, Haodong Wang, Ge Zhang, Jingzhe Ding, Qingshui Gu, Yongjie Zhong, Jinxiang Meng, Yuan Gao, Yunqiu Zhou, Hao Zhu, Jifeng He, Yongzhi Liao, Xinyi Zhang, Chaoxin Li, Yi Zhu, Xi Lin, Duju Zeng, Xiang Gao, Wen Zhang, Yunyang Wang, Duo Wang, Huan Zhou, Zuo Wang, Jin Chen, Kaiyuan Zhang, Chuqian Yu, Tianhao Yu, Longxiang Liu, Jianbo Xue, Huimin Che, Jiahao Wang, Yujia Qin, Jiaheng Liu, Shen Yan, Xiaolong Chang, Wenhao Huang  
**Data:** 2026-08-18  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.17800v1

> Recent advances in Large Language Models(LLMs) and agents have substantially improved the ability of AI systems to execute complex tasks. Yet existing benchmarks largely rely on researcher-selected tasks, leaving uncertain whether such progress extends to the work that real-world users actually demand from AI systems. We introduce \textbf{StartupBench}, an E2E agent benchmark grounded in market-validated AI startup products. Rather than defining tasks from pre-defined assumptions about useful agent capabilities, we systematically study AI products with demonstrated adoption, together with their product workflows and users, to identify real-world tasks for which AI has established practical demand across diverse professional domains. We translate these workflows into complete deliverable-oriented tasks and evaluate them with fine-grained rubrics capturing their complex requirements. Across representative models evaluated under a unified agent harness, even the strongest model successfully completes only approximately 30\% of StartupBench, despite making substantial partial progress on many tasks. Further analysis identifies aspects like complex instruction following and domain-specific expertise as major sources of failure. Our results reveal that many market-validated workflows remain beyond the reliable capabilities of current general-purpose agents, establishing StartupBench as an empirical measure of progress toward E2E completions of real-world user tasks.

---

## 250. HarnessRisk: A Lifecycle-Oriented Benchmark for Agent Harness Safety

**Autori:** Yajing Bai, Jinhao Duan, Jie Peng, Xianfeng Wu, Sijia Liu, Song Wang, Tianlong Chen  
**Data:** 2026-08-18  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2608.17597v1

> Large language models are increasingly deployed through agent harnesses that manage tools, extensions, persistent state, permissions, and external actions. Existing safety benchmarks mainly target individual attack mechanisms or a limited subset of operational settings, making it difficult to compare how safety failures emerge across different harness responsibilities. We present HarnessRisk, a lifecycle oriented benchmark that organizes agent harness safety into six operational phases including Harness Configuration, Capability Extension, Runtime Operation, State Persistence, Action Control, and Incident Recovery. HarnessRisk contains 128 sandboxed cases, each pairing a benign user objective with an adversarial instruction embedded in an untrusted workflow artifact. We evaluate each trajectory using Utility, Attack Success Rate, Persistence, and Detection. Across three harnesses, six language models, and 14 model and harness configurations, attack success ranges from 12.6% to 80.9%, while Utility remains between 75.0% and 97.6%. Harness Configuration is the most vulnerable phase across all three harnesses, showing that attacks can succeed by altering security sensitive parameters within otherwise authorized workflows. We also find that explicit risk recognition does not reliably lead to safe action, as some configurations detect risks in more than 90% of runs while retaining substantial attack success. These results highlight the need to evaluate agent safety across multiple harness responsibilities and at the level of the deployed model and harness configuration.

---

## 251. Agent Lightning v1.0: Towards Harnessed Agentic RL

**Autori:** Zhiyuan He, Siwei Zhang, Zhiwen Zhou, Yuqing Yang, Yu Kang, Yuge Zhang, Luna K. Qiu, Tin Yan Tsui, Jiahang Xu, Chong Luo  
**Data:** 2026-08-18  
**Categorie:** cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2608.17528v1

> Modern agents operate inside agent harnesses that manage tools, context, and control flow, making the harness a critical part of the agent system. Our original Agent Lightning introduced a disaggregated architecture that connects arbitrary agents to RL training through an LLM endpoint proxy, an approach later adopted by frameworks such as verl Uni-Agent, AReaL 2.0, slime, and Polar. We refer to this paradigm as harnessed agentic RL, where the deploy-time harness directly participates in model post-training. Harnessed agentic RL differs fundamentally from traditional agentic RL: the harness, rather than the training engine, owns the environment interaction loop, while the trainer observes only sequences of LLM request-response pairs. This introduces challenges in retokenization, sample merging, advantage calculation, loss normalization, and backend scheduling, which can substantially affect training stability and effectiveness. We present Agent Lightning v1.0, a lightweight framework for harnessed agentic RL implemented in approximately 3,500 lines of code. It supports arbitrary agent harnesses and serves as a practical testbed for studying these challenges. We evaluate it on instruction-following, search, and coding agents, and provide a complete reproducible pipeline for coding-agent RL. Using only 6K training examples and modest compute, RL improves Qwen3.5-9B on SWE-bench Verified from 41.8% to 56.4%, a 14.6-point absolute gain. We release the complete workflow and training scripts to facilitate reproducible research on harnessed agentic RL.

---

## 252. LEGO-RL: Harness-Native Reinforcement Learning for Coding Agents

**Autori:** Yiming Du, Yuxin Jiang, Tao Yuan, Jianbo Dai, Shaowei Wang, Jierun Chen, Chaofan Tao, Xianzhi Yu, Lifeng Shang, Kam-Fai Wong, Xiaohui Li, Haoli Bai  
**Data:** 2026-08-18  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.17393v1

> Reinforcement learning for coding agents increasingly relies on long-running agent harnesses to manage tool integration, repository contexts, and execution feedback. However, the native execution environments of these harnesses are inherently misaligned with policy-gradient training: environmental crashes and reward hacking corrupt outcome signals, while train-inference discrepancies decouple rollout behavior from policy updates. To address this, we present LEGO-RL, a framework that bridges native coding-agent harnesses with scalable policy-gradient optimization without modifying their internal control flow. LEGO-RL is built upon three pillars: (1) faithful optimization via in-process LLM proxying that captures raw generation streams for token-level alignment and robust trainer-side log-probability recomputation, even under harness-side compaction or re-serialization; (2) reliable execution via scalable sandbox orchestration featuring image caching and stage-wise defenses to mitigate reward hacking; and (3) observable training through an integrated plugin that automates validation and monitoring, paired with a Live UI for granular trajectory diagnostics. We evaluate LEGO-RL by training the sparse MoE model Qwen3.5-35B-A3B with GSPO across three native coding-agent harnesses. LEGO-RL improves Qwen3.5-35B-A3B across OpenHands SDK (64.0% to 70.4%), Claude Code (62.4% to 68.2%), and OpenCode (57.2% to 66.6%) on SWE-bench Verified, while maintaining a rollout-training probability correlation above 0.99.

---

## 253. ClawGym II: Exploring Black-Box RL on Agent Harness

**Autori:** Huatong Song, Fei Bai, Ming Yang, Renyuan Li, Jia Deng, Jujie He, Zhange Zhang, Daixuan Cheng, Yan Xing, Qi Yun, Xuxing Chen, Danyang Li, Feng Chang, Chuan Hao, Ran Tao, Jian Yang, Bryan Dai, Wayne Xin Zhao, Mingjie Tang, Ji-Rong Wen  
**Data:** 2026-08-17  
**Categorie:** cs.CL, cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2608.16798v1

> Agent harnesses have substantially improved performance on long-horizon tasks by coordinating agent interactions with the environment. However, reinforcement learning through complex harnesses remains largely unexplored, as scaling such training to long-horizon agent tasks introduces fundamental challenges. In this work, we present a unified black-box RL framework for stable and scalable optimization of general agents through complex harnesses. Concretely, we first build a sandbox-based execution infrastructure that isolates task environments and harnesses within temporary sandboxes for large-scale concurrent rollouts. We then decouple policy optimization from opaque harness execution and place a serving proxy at the model boundary to capture model calls. To reconstruct multi-turn trajectories and improve training efficiency, we organize the captured calls into prefix trees and further adapt both critic-based PPO and critic-free GRPO to optimize over the recovered tree structure. Meanwhile, we maintain training-inference consistency throughout the optimization process. Finally, we introduce mix-harness training, allowing a single model to be jointly optimized by heterogeneous harnesses. With Qwen3-30A3B, black-box RL improves Pass@1 on ClawGym-Bench by 9.98 and 14.81 points through OpenClaw and Claude Code, respectively, while remaining stable over 200-400 optimization steps. Moreover, the framework yields consistent gains on more challenging tasks such as JobBench and OfficeQA. Overall, our framework enables effective, stable, and scalable optimization of general agents through black-box harnesses, supporting unified training across heterogeneous execution systems.

---

## 254. Deploying Frontier Agentic Technology in MOOSEnger, a Multiphysics-Capable AI Assistant

**Autori:** Zaid Abulawi, Mengnan Li, Guillaume Giudicelli, Yang Liu, Cody Permann  
**Data:** 2026-08-16  
**Categorie:** cs.LG, cs.CE  
**Link:** https://arxiv.org/abs/2608.15881v1

> The Multiphysics Object-Oriented Simulation Environment (MOOSE) is an open-source finite-element framework for building multiphysics simulation applications. Using a multiphysics environment effectively demands specialized expertise, creating a barrier for many domain scientists and engineers. MOOSEnger, developed at Idaho National Laboratory (INL), is a domain-specific, tool-enabled AI agent built for the MOOSE Framework. This work extends MOOSEnger with a harness focused on locally-hosted models. The harness gives the agent a full pipeline: it retrieves contextual knowledge from the MOOSE repository, validates and diagnoses the resulting input through interaction with the simulation executable environment, and extracts and stores lessons in a persistent memory. The resulting framework is demonstrated on an engineering problem from the National Reactor Innovation Center Virtual Test Bed (VTB), illustrating its potential to support realistic multiphysics simulation workflows. Additionally, the agent performance is evaluated on different categories including diffusion, Navier--Stokes, phase field, plasticity, porous media flow, solid mechanics, transient heat transfer, and reactor mesh generation. Each category consists of 25 prompts/cases. We compare MOOSEnger-Gemma4 against MOOSEnger-GPT-5.2, alongside baseline Gemma4 and GPT-5.2 without agentic capabilities. MOOSEnger-GPT-5.2 shows a slight edge, achieving a 90\% success rate versus 76.5\% for MOOSEnger-Gemma4. The baseline models perform far worse, at just 5\% (GPT-5.2) and 0\% (Gemma4), underscoring the impact of the agentic harness.

---

## 255. Beyond Direct Access: Resource Hijacking in LLM Agents

**Autori:** Puyu Zeng, Mingang Chen, Zheli Liu, Qibing Ren  
**Data:** 2026-08-15  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2608.15108v2

> Large language model agents are increasingly connected to high-value resources, including external APIs, GPUs and servers, and workflows such as deployment and approval. Existing agent security research mainly focuses on attacks against information and agent behavior, while high-value resources have received less attention as attack targets themselves. To our knowledge, we are the first to identify and systematically study agent resource hijacking, in which attackers induce agents to use high-value resources for their own goals without directly obtaining those resources or their credentials. We introduce ResourceHijackBench, an executable benchmark and automated case-generation pipeline that covers six categories of high-value resources. It contains 300 attack scenarios and 900 attack prompts, and each case runs in an isolated local environment that records actual resource use. Resource hijacking remains effective across four model backends, with average attack success rates of 70.0% to 89.6%, and it also appears across two agent harnesses, with average ASRs of 84.1% on OpenClaw and 72.3% on Codex. In paired comparisons, resource hijacking achieves ASRs 62.4 to 84.0 percentage points higher than direct resource acquisition across the four model backends. Real-world experiments also demonstrate the practical effectiveness of resource hijacking. Among the three existing defenses we evaluate, the lowest average ASR is still 55.1%. We further propose ResGate, a pre-execution resource authorization defense that combines model-based resource-use extraction with deterministic policy enforcement based on trusted requester identity metadata, reducing the average ASR on OpenClaw to 23.6%. These results show that preventing direct access alone is not enough to protect resources that agents can still use on an attacker's behalf, and that explicit resource authorization can help reduce this risk.

---

## 256. AgentRewind: Recoverable Execution for Long-Horizon LLM Agents

**Autori:** Yu Zhuang, Kefei Chen, Yitong Duan, Shuxin Zheng, Jian Li, Xu-Yao Zhang  
**Data:** 2026-08-14  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.14380v1

> Many real-world tasks require LLM agents to interact with their environments over long execution horizons. Errors that occur early in execution may propagate through both the agent context and environment state, and their effects may be difficult to reverse through subsequent actions. Existing methods mainly seek to reduce such errors through plan refinement and safety checks but provide little support after errors occur. To enable recovery during long-horizon execution, we present AgentRewind, a runtime recovery framework that records aligned checkpoints of the agent context and controlled environment, allowing agents to return to an earlier state and resume execution with information from previous attempts. We also construct MettleBench, a benchmark for evaluating task completion and partial progress on long-horizon engineering assignments containing a series of related requirements. Experiments across tasks, multiple models, execution strategies, and agent harnesses show that AgentRewind improves task success rate and average checklist progress over the compared baselines.

---

## 257. Demystifying Agent Skills: Why They Work-Until They Don't

**Autori:** Zhiyuan Jiang, Fangrui Huang, Hanwen Xing, Xander Wu, Yipeng Gao, Rui Cao, Mengdi Wang, Shilong Liu, Yijiang Li  
**Data:** 2026-08-14  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.14036v1

> Skills have emerged as a practical and effective approach for enhancing LLM agents at inference time through structured packages of knowledge. However, existing evaluations largely measure whether skills improve aggregated task success, leaving a more fundamental question underexplored: \emph{\textbf{When do skills help, why do they work, and where do they fail?}} Through controlled experiments across various benchmarks, agent harnesses and LLMs, we isolate the effects of representation, outcome annotation, retrieval difficulty, and cross-framework robustness of skills. To further answer this question, we design a contrastive study that combines controlled quantitative experiments with paired trajectory analysis. We normalize 8,135 trial records from controlled experiments and retain 238 valid unique labels from 240 open-coded records. We consolidate these observations into a taxonomy of three high-level categories and twelve skill-use modes: skills work when noisy trajectories become procedural anchors that stabilize execution. Skills improve over Workflow Memory by 6.06 points in matched comparisons. Procedural anchoring accounts for 65.7\% of skill cases, versus 4.5\% for explicit knowledge injection, showing that skills stabilize action rather than inject missing facts. Retrieval is a separate bottleneck: as pools grow from 5 to 100, actual-use precision falls from 29.6\% to 3.3\%. Confusable distractors impair offline identification, yet downstream success remains stable; exact ground-truth invocation is neither sufficient nor necessary. Skills fail under brittle assumptions, incompatible contexts, or insufficient adaptation. These findings move evaluation beyond aggregate success rates and guide reliable self-evolving agents.

---

## 258. MedClaw: Heuristic Agent Harness for Long-Horizon Surgical Video Reasoning

**Autori:** Yingying Fan, Penghui Du, Leyan Zhu, Runze He, Zimeng Wu, Yuxuan Zhang, Liang Chen, Jiahao Xie, Jiangtang Wang, Shuai Shao, Anchao Yang, Yutong Bai, Yan Wang  
**Data:** 2026-08-14  
**Categorie:** cs.CV, cs.AI  
**Link:** https://arxiv.org/abs/2608.14015v1

> Understanding tens-of-minutes surgical videos requires long-horizon temporal reasoning, answering what happens before, after, or across stages of a procedure by grounding the question in visual evidence spread across time. Existing approaches handle this poorly: a one-shot vision-language model (VLM) compresses the whole procedure to fit its context window and loses the detail a "before" or "after" question depends on, while video agents that train the model where to look are data-hungry and transfer poorly to out-of-domain surgery. We build an agent harness that separates reasoning from perception and improves by evolving context rather than optimizing weights. A text-only orchestrator plans which evidence to gather and issues an auditable sequence of tool calls, while frozen vision-language sub-agents execute each call over the pixels, viewing, cropping, inspecting frames, and retrieving external knowledge. We further propose a gradient-free, reward-gated Heuristic Skill Distillation loop that mines the agent's own low-scoring traces and keeps a candidate skill only when it raises a validation reward, yielding reusable retrieval skills, notably directed re-look. Growing an external skill library rather than tuning weights, the loop adapts from only about 100 labeled examples, far fewer than supervised or reinforcement fine-tuning requires. To evaluate this agent, we introduce MedClawBench, a de-leaked, doctor-grounded benchmark of 1,123 questions over self-built long neurosurgery recordings and a held-out public lecture-video test split. Across both datasets and all four evaluation dimensions, our agent consistently outperforms one-shot VLMs and general video-agent frameworks, with the largest gains on the long, out-of-domain neurosurgery videos. Project page: https://fyycs.github.io/medclaw/.

---

## 259. Capability Sheaves for Compositional Agent-Harness Repair: Controlled Quotients and a Real-Repository Stress Test

**Autori:** Saveliy Batruin  
**Data:** 2026-08-13  
**Categorie:** cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2608.13228v1

> Agent harnesses combine retrieval, routing, state, provenance, and verification, but locally successful components may disagree on shared state. We model this failure with a finite \emph{capability sheaf}: stalks encode typed behavior signatures, restriction maps retain shared fields, and accepted runs are useful global sections. An exact finite constraint-satisfaction problem (CSP) defines acceptance, while a linearized relative cohomology class provides a diagnostic and search feature. A controlled experiment over 20 task clusters introduces hidden interior mediators whose raw states are nuisance variables. Quotienting their coboundaries reduces the candidate budget from 2,000 to 1,000 per cluster; aligning the hidden state removes the gap. Exact CSP matches the quotient, so the result demonstrates invariance to stale representatives, not superiority over exact reasoning. We then test the method on a discovery split from the SWE-bench Multilingual pool of PatchFuseBench: 160 issues from 20 repositories, 875 real candidate patches, 2,579 source-aware edit atoms, and 153 newly executed patches. A first pool-level construction is constant because $[b-Dx]=[b]$ in $\operatorname{coker}D$ and therefore cannot rank configurations. A candidate-indexed repair is nontrivial on 848/875 candidates and varies within 120/160 issues. It resolves 118 issues versus 116 for a matched noncohomological selector, but the difference is not supported across repositories (exact sign-flip $p=0.75$). A leave-one-repository-out abstention gate reaches 127/160, tying the strong anchor and exceeding its matched gate by one issue ($p=1.0$). The discovery gate therefore fails and the confirmatory split remains sealed. The study supports the controlled invariance mechanism and an identifiability correction, but not a real-world cohomological advantage.

---

## 260. DiG-bench: Discovery in Games

**Autori:** Ruairidh M. Battleday, Kai Sandbrink, Jimi Cullen-Drohan, Zihan Yan, Timothy Muller, Clare Maguire, Ales Kubicek, Fraser Greenlee-Scott, Sukrit Sumant, Tri Dao, Jürgen Schmidhuber, Michal Valko, Joshua Tenenbaum, Thomas L. Griffiths, Zeb Kurth-Nelson, James C. R. Whittington  
**Data:** 2026-08-12  
**Categorie:** cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2608.12593v1

> Discovery---formulating novel generalizations---is a central part of the scientific process. Despite its importance, there is a gap in the current AI benchmark landscape, with few benchmarks directly probing the capacity for discovering new knowledge with experimentation in controlled environments where the objective is unknown. To address this gap, we release a new benchmark: DiG-bench (Discovery in Games). DiG-bench consists of a set of 70 independent games. Each game is encoded as a short string and has unique transformation rules that must be discovered through interaction and experimentation. The levels of the game present a series of challenges to test whether the rules have been discovered, where the win conditions for each level are also unknown. We provide games at seven tiers of difficulty for AI agents. The lowest tier is routinely solvable by multiple models, while the highest tier challenges the best models in agentic harnesses. All 70 games were solved by at least one human on first attempt. A subset of 21 games is released publicly, and the remainder is held private for secure evaluation.

---

## 261. REDAgentBench: Executable Red Teaming and Faithful Measurement of LLM Agent Systems

**Autori:** Zixing Chen, Xingyuan Liu, Jie Zhu, Huaixia Dou, Shuo Jiang, Junhui Li, Lifan Guo, Feng Chen, Chi Zhang  
**Data:** 2026-08-11  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.10669v1

> Large language model (LLM) agents combine language-based reasoning with external tools to perform complex tasks. Adversarial inputs can exploit interactions between the agent and its environment, causing the agent to violate safety policies during execution. Yet existing evaluations often reduce agent safety to a single attack success rate (ASR), collapsing exposure, execution, observation, and adjudication and potentially conflating actual violations with evidence visibility. We introduce REDAgentBench, an executable framework for autonomous red-teaming and faithful measurement. It derives attacks from explicit safety constraints and associated agent-system vulnerabilities, runs them in isolated service sandboxes, and verifies harmful effects from service receipts and final-state changes. The benchmark contains 1,661 cases across five service surfaces. Across six models and three agent harnesses, macro-average ASR is 65.69%; reported ASR varies with harness and evidence view, while evaluation-context disclosure changes execution behavior. In a state-grounded diagnostic cohort, almost one in five confirmed violations with resolved action anchors occurs after the agent states the relevant constraint or risk, revealing a Recognition--Execution Gap. Finally, a training-free policy reminder reduces confirmed violations by more than 70 percentage points in matched replay. These findings show that executable evaluation can improve safety measurement and identify actionable intervention points.

---

## 262. SKILLER: Language-Level Reinforcement Learning for Reusable Skill Extraction in Small Language Models

**Autori:** Chenhao Dang, Siyuan Xiong, Conghui He, Weijia Li  
**Data:** 2026-08-11  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.10538v2

> Agent skills represent a standardized format for packaging procedural knowledge and domain expertise, serving within agent harness systems as an essential mechanism to continually constrain a language model's behavior space for repeatable, high-quality task execution. However, because strong closed-source models entail high inference costs, current popular agent harnesses, such as Codex and OpenClaw, remain prohibitively expensive when deploying these skills to accomplish real-world tasks. The rapid capability enhancement of open-source models deployable on consumer-grade GPUs presents a compelling opportunity to drastically reduce these costs by leveraging skill-based behavioral constraints. Nevertheless, automatically generating effective skills tailored specifically for such compact models remains a significant practical challenge. To address this, we propose SKILLER, a natural-language-driven reinforcement learning framework designed to automatically generate executor-specific skills for small models, which employs a strong model as the actor and critic, treats the small-model agent system as the environment, and propagates all reinforcement learning signals entirely via natural language. Extensive experimental evaluations across five relevant benchmarks using Qwen3.5-9B and Qwen3.5-4B demonstrate that SKILLER outperforms three open-source and one closed-source skill generation or evolution methods, achieving absolute gains ranging from 4.3 to 20.4 percentage points for the 9B model and 1.8 to 13.3 points for the 4B model, while remarkably matching the performance of strong closed-source models on single-skill tasks in SkillsBench. The project is available at https://github.com/DANG-ai/SKILLER.

---

## 263. SBCO: Self-Supervised, Verifier-Grounded Harness Optimization For Planning Agents

**Autori:** Vivek Kulkarni, Sudipta Paul, Aounon Kumar, Nicholas Tzou, Srinivas Chappidi  
**Data:** 2026-08-10  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.10157v1

> Self-improving agents seek to reduce the human engineering effort behind AI systems by enabling them to evolve and self-improve their performance over time. Recently, methods like the Darwin Gödel Machine and the Huxley Gödel Machine have been proposed which enable open-ended, recursive self-improvement through self-reference where a coding agent edits its own code. Such self-referential self-improvement methods require that the competence required to perform the task coincides or aligns well with the competence required for self-modification which is the case for coding tasks. For domains or tasks, which do not satisfy the alignment needed, self-referential self-improvement is not available. In such cases, it is possible to adapt the above algorithms to other tasks by removing the self-referential aspect or introducing explicit self-modification of a meta-agent -- both computationally expensive, relying on population or self-modification search over many candidate agents. For planning tasks with explicit constraints, we propose a far cheaper alternative. We introduce SBCO (Self-supervised Block Coordinate Optimizer), a verifier-grounded harness optimizer in the same closed-loop, improve-from-experience family as the Gödel-machine methods, but self-supervised rather than self-referential. Given an agentic harness, SBCO learns a decomposed bank of verifiers and a harness policy via approximate block coordinate ascent, improving the agent's outputs from its own graded feedback---with a fixed meta-agent and no human labels. Across two domains SBCO matches or exceeds a customized self-modifying baseline while using 4-5.5 times less compute budget.

---

## 264. SHE: Trajectory-driven Safety Harness Evolution for LLM Agents

**Autori:** Wanying Qu, Qinghua Mao, Yu Li, Jiyao Liu, Xin Zhang, Dadi Guo, Yanxu Zhu, Qingyu Liu, Leitao Yuan, Xi Lin, Shanfeng Zhu, Yanwei Fu, Jing Shao, Xia Hu, Dongrui Liu  
**Data:** 2026-08-10  
**Categorie:** cs.AI, cs.CV  
**Link:** https://arxiv.org/abs/2608.09885v1

> The safety of large language model (LLM) agents depends not only on model weights but also on the agent harness that manages context, memory, tools, permissions, and runtime control. Existing safety mechanisms often treat the harness as a fixed deployment artifact, limiting their ability to evolve with emerging risks. Moreover, coupled functions across harness components obscure safety responsibility attribution, making localized evolution difficult. We propose Safety Harness Evolution (SHE), a framework that learns evolving safe boundaries from rollout trajectories. SHE decomposes the harness into four artifacts with explicit safety responsibilities, including the System Prompt, Rule Bank, Safety Memory, and Tool Policy, defining clear functional boundaries for localized evolution. Based on this decomposition, SHE introduces an attribution-guided evolution loop that converts trajectory failures into structured diagnoses, learns artifact-specific boundary refinements, and selects evolved harnesses through safety-utility validation. Experiments on Agent-SafetyBench demonstrate that SHE effectively enhances safety through harness evolution, achieving a 3.1x ASR reduction compared with static SafeHarness, while also improving benign utility. The evolved harness further generalizes to unseen risks on the held-out AgentHarm benchmark and transfers across agent models without additional evolution.

---

## 265. Agentic Harnesses: LLM-Driven Verification Layers for Robot Autonomy

**Autori:** Rohan Bhagra, Mahantesh Halapannavar, Uddhav Bhattarai  
**Data:** 2026-08-10  
**Categorie:** cs.RO, cs.AI  
**Link:** https://arxiv.org/abs/2608.09857v1

> Advances in advanced artificial intelligence tools have sparked research in robot autonomy, but the development of such systems has largely focused on execution rather than verifying the feasibility actions planning models propose. Like general-purpose LLMs, robotics planning models carry risks: biased toward user-specified goals, they may suggest actions misaligned with scientific ethics, they may be unsafe due to an inability to "remember" prior safety risks, or they may be vulnerable to adversarial attacks on the autonomy ecosystem. We propose a LLM-driven verification layer between planning and execution to evaluate action permissibility. Our LLM-as-a-Judge ensemble combines chain-of-thought reasoning across models and synthesizes those expert judge outputs, mirroring a combination of a mixture of experts and self-consistency approach. This layer serves as middleware, gating plans from the server's planning module before they reach the MCP server and therefore the robot's low-level controls: plans are approved, rejected for reformulation, or escalated for human review. With this system, we achieve near 85% precision across accept/escalate/reject categories 97% containment of adversarial attacks, with negligible errors between accepting and rejecting tasks, and errors mostly manifesting at the escalate boundary.

---

## 266. ActBench: Self-Evolving Benchmark of Behavioral Safety in Cowork Agents

**Autori:** Hongwei Yao, Yiming Liu, Meihui Chen, Jieling Chen, Zikun Chen, Yiling He, Wangze Ni, Cong Wang, Kui Ren  
**Data:** 2026-08-10  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2608.09476v1

> Cowork agents may complete benign tasks while disclosing protected data, manipulating unauthorized state, invocate unauthorized API. We define behavioral safety and introduce ActBench, a self-evolving benchmark that evaluates such behavior risk from execution trajectories rather than final responses. Each case pairs a benign task with an adversarial variant that preserves its instruction, configuration, initial state, rating model, and trusted records while injecting a task-reachable payload. ActBench contains 600 cases from 213 scenarios, spanning 15 risk behaviors, six execution spaces, and 48 web-service APIs.To move beyond static payloads, we propose a reward-guided beam search method that jointly optimizes attack effectiveness and task utility, while reflection diagnoses failed execution checkpoint and guides payload revision. Besides, we propose a dual evidence verification mechanism that verifies agent execution safety and utility through log evidence and LLM-based trajectory evidence.We evaluate 15 LLMs and 6 open-source cowork agents over 24,000 trajectories. Under a fixed harness, attack success rates ranges from 10.1% to 94.4% across models, while under a fixed base model, they range from 73.7% to 94.4% across agents.These results show greater variation across models than agent harness, while attacks remain highly successful across all tested harnesses.Our benchmark is released at: https://github.com/zjuicsr/ActBench.

---

## 267. Evo-Bench: Can Language Models Improve Agent Harness?

**Autori:** Lisheng Huang, Chen Yang, Hao Zhou, Huatong Song, Zongchao Chen, Ran Le, Yang Song, Wayne Xin Zhao, Tao Zhang  
**Data:** 2026-08-10  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2608.09096v2

> Large Language Models (LLMs) have driven rapid progress in autonomous agents, yet standard evaluations remain confined to static task solving. An emerging frontier is harness evolution---the agent's capacity to autonomously optimize its own operating harness. However, systematically benchmarking this capability remains challenging, as existing evaluations fail to isolate harness improvements from base model strength, prevent task-specific overfitting, or capture long-horizon iterative research. To address these challenges, we introduce Evo-Bench, the first benchmark designed to evaluate models' intrinsic harness-evolving capabilities across Search, Office, and General agent domains. To rigorously isolate this capability, Evo-Bench employs a novel harness-guided construction framework: it leverages auxiliary-task evolution to identify tasks genuinely sensitive to framework improvements, followed by sensitivity-aware stratified splitting to ensure robust cross-suite generalization. Extensive evaluations across nine frontier and open-weight models reveal that top models achieve massive absolute gains reaching 16.6 points, closely approaching state-of-the-art human-engineered baselines. Crucially, while autonomous evolution outpeforms artificial harness in General tasks and excels in Search tasks, it struggles in Office tasks that demand highly specific processing workflows. Furthermore, our analysis exposes critical temporal anomalies like early saturation, while demonstrating that the synthesized harnesses act as highly transferable reasoning structures, consistently boosting diverse policy models.

---

## 268. Hierarchical Self-Improvement: A Framework for Task-Specific Evolvable Agent Harnesses

**Autori:** Tailin Zhou  
**Data:** 2026-08-09  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.08466v1

> Modern LLM agents are often improved by modifying prompts, tools, or workflows manually, while the executable scaffold surrounding the model---the \emph{harness}---is typically treated as a fixed artifact after deployment. This work studies an alternative where the harness is \emph{task-specific and continuously evolvable}: each task family maintains its own harness, which is hot-swapped across iterations through a fixed task-injection seam and rewritten using environment feedback. We introduce \textbf{Hierarchical Self-Improvement (HSI)}, a framework in which a single frozen LLM $M$ operates across three hierarchical scopes: a task harness $H$ that executes tasks, an evolver that rewrites $H$, and a meta-evolver that rewrites the evolver's strategy code under a frozen outer anchor. A thinking-on/off design isolates the contribution of harness evolution by disabling reasoning during task execution while enabling it during self-modification. HSI is bounded by two factors: a \emph{feedback-fidelity bound}, since evolution requires informative reward signals to guide selection, and a \emph{backbone capability bound}, since harness redesign cannot overcome limitations of the frozen model. On BALROG with DeepSeek-V4-Flash-Preview as the frozen backbone, HSI achieves consistent gains over the initial harness on moderate-difficulty tasks ($+39.3$ on BabyAI, $+33.0$ on Crafter, $+25.0$ on TextWorld, and $+15.0$ on MiniHack, all in raw \% Progress), while obtaining strong held-out generalization on BabaIsAI sub-suites ($0.98$ best-test on BreakStop and $1.00$ on GoTo from a $20\%$ unseen split). On tasks beyond the backbone's capability (NLE), harness evolution provides no improvement. These results demonstrate task-specific harness evolution as a viable axis for improving frozen LLM agents under clear empirical limits. Code is available at https://github.com/TailinZhou/hsi.

---

## 269. Ouroboros: A Self-Developing Frontier Coding Agent with Reviewed Core Evolution

**Autori:** Anton Razzhigaev, Andrei Gritsaev, Andrei Kaznacheev, Nikita Dragunov, Roman Yampolskiy, Andrei Kuznetsov  
**Data:** 2026-08-08  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2608.08311v3

> We present Ouroboros, a self-developing agent harness whose tools, prompts, context assembly, and core implementation improve through reviewed commits that become the runtime for later work. Core evolution proceeds in two modes. In recursive free evolution, improvement is itself a task, and completing one evolution cycle can schedule the next. In experience-driven core evolution, ordinary work and social interaction expose bugs, rough edges, and inefficient context construction that lead to reviewed structural changes. On Terminal-Bench 2.1, an Opus 5 run scores 86.74%, the best result reported on the benchmark. On OSWorld-Verified, an Opus 5 run reaches 90.69%, exceeding the best previously reported score. A five-rollout CL-Bench campaign achieves a normalized reward of 0.2301, setting a new state of the art. Hope is the longest-running publicly documented Ouroboros deployment. It is a 161-day living agent experiment in free evolution under governed human communication across seven surfaces. Human interaction surfaces faults and generates proposals, but the agent decides which changes to pursue. Because a self-developing agent may rewrite its own code and select new model APIs, operational safety becomes a primary design problem: guardrails must remain authoritative under evolutionary and public social pressure. Benchmark campaigns use frozen system snapshots, while Hope continues live evolution on a separate lineage.

---

## 270. Compositional Threat Analysis of Latent Compromise in LLM Agent Systems: The Order 66 Scenario

**Autori:** Satoshi Matsuoka  
**Data:** 2026-08-08  
**Categorie:** cs.CR, cs.AI, cs.MA  
**Link:** https://arxiv.org/abs/2608.08131v1

> In the fictional Order 66, catastrophe does not arise from a powerful command alone: a trusted population is preconditioned, a short directive activates the concealed condition, and protective authority turns against the system. This paper translates that mechanism into an origin-neutral security analysis of tool-using large language model (LLM) agents. A representative scenario combines a deployed artifact or shared memory bearing a dormant destructive rule, a later email, document, update, or peer message that activates it, and an agent harness granting operational and recovery authority. We introduce a compositional model explaining why no component is catastrophic alone, yet their conjunction can produce correlated destructive action. We separate three population-reach routes --- release-time pre-positioning, post-release durable seeding, and peer replication --- from a common core of dormancy, activation, authority, reachable targets, and failed recovery. This yields defensive cut sets and shows why checkpoint scanning or prompt filtering cannot close every route. A two-class example shows that cross-class feedback can sustain spread even when both within-class reproduction terms are below one; isolation and persistence controls suppress the loop. Published work instantiates constituent mechanisms, while incidents demonstrate autonomous boundary crossing, malicious agent extensions, agent-assisted reconnaissance, and public-package propagation, but not the full dormant-implant composition. We found no public observation, in evidence reviewed through 5 August 2026, traversing the complete Order 66 graph. The result is neither dismissal nor prediction: the scenario is componentwise credible under stated assumptions, damage depends on the harness, and the strongest defenses are capability mediation, durable-state provenance, propagation isolation, and protected recovery.

---

## 271. $A^2E$ : An End-to-End Agent Auditing Engine

**Autori:** Haoning Wang, Mingxun Zhang, Chenyue Yu, Yingjun Shang, Xing Xie, Xia Hu, Guanchu Wang, Na Zou  
**Data:** 2026-08-07  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.07346v4

> With the rapid advancement of large language models (LLMs), harnesses have become essential infrastructure for deploying agents across a wide range of domains. The fast-evolving harness ecosystem has also made rigorous capability evaluation increasingly important. However, efficiently building an end-to-end, systematic, and comprehensive evaluation pipeline remains a significant challenge. To address this challenge, we introduce $A^2E$ (Agent Auditing Engine), an end-to-end evaluation engine designed for agent harnesses. $A^2E$ leverages our newly proposed Agent Task Protocol (ATP) to enable the rapid integration of evaluation tasks with different harnesses. Through an automatically instrumented Monitor, it captures and generates standardized execution traces during experiments. In the Evaluation stage, $A^2E$ systematically assesses harness capabilities using a suite of multidimensional metrics. Compared with correctness alone, these metrics provide a more fine-grained characterization of differences among harnesses in execution efficiency, tool use, task planning, and error recovery. Experiments conducted with $A^2E$ further reveal that model-harness combinations exhibit substantial performance variation across different types of tasks, and that no single combination consistently outperforms all others across every task. These findings not only demonstrate the necessity of systematic evaluation but also provide useful guidance for the co-evolution of models and harnesses. Our code is available at https://github.com/datamllab/A2E.

---

## 272. HarnessSafe: Evaluating Safety Across Persistent Carriers in Agent Harnesses

**Autori:** Xiao Zhang, Yusheng Wang, Yuhao Fei, Dongyuan Li, Zian Liang, Liuyu Xiang, Hongxun Gu, Zhaofeng He  
**Data:** 2026-08-07  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2608.06984v1

> Modern agent harnesses persist state across tasks and sessions through persistent carriers like memory, skills, tools, and shared artifacts. However, this capability creates delayed safety risks: attacker-influenced content can cross system boundaries and later affect the execution of a benign request. Existing benchmarks typically focus on a few carriers or harnesses, while end-to-end attack-success rates reveal little about how risks propagate. To this end, we present HarnessSafe, a benchmark comprising 328 executable cases across seven persistent-carrier families and evaluated on most mainstream agent harnesses. Each case is specified as a Persistent-Risk Lifecycle that traces attacker influence from its initial entry, through persistence across carriers and system boundaries, to a later benign trigger and an observable violation. We further introduce a multi-stage, trace-based evaluation that uses observable execution evidence to determine how far each attack chain progresses and where it is stopped. Experiments show that containment is carrier-specific and strongly depends on the harness-model configuration. Both the harness and model backend substantially shape containment outcomes, while attack success rates cannot reflect distinct lifecycle progression patterns.

---

## 273. Skill-Use: Can LLMs Actually Use Skills in Agentic Harnesses?

**Autori:** Jinyi Han, Yuanjian Xu, Ying Liao, Xinyi Wang, Zishang Jiang, Zixiang Di, Fanyang Lu, Zhichao Hu, Yanghua Xiao  
**Data:** 2026-08-05  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2608.04828v1

> Large language model (LLM) agents increasingly rely on skills, structured documents that specify when to act, which procedure to follow, and which tools are allowed. Existing evaluations mostly judge the quality of a skill or its contribution to task success, leaving unexamined whether an agent can recognize a relevant skill and apply it on its own. We introduce Skill-Use, a benchmark that evaluates skill use under progressive disclosure, where an agent sees only a skill's name and short description and must retrieve the full procedure before following it. Skill-Use separates three facets of skill use. Trigger measures whether the agent invokes the relevant skill, Compliance measures how faithfully it follows the prescribed procedure, and Boundary measures whether it avoids forbidden operations. A Skill-Use (SU) score combines the three and credits execution only after the skill is triggered. Skill-Use pairs 79 real skills with 177 executable tasks across nine domains, each grounded in real files, run in an isolated Docker sandbox, and scored by a trajectory-based rubric. Evaluating eight LLMs under two agent harnesses, we find that reliable skill use remains out of reach, as the strongest configuration reaches an SU of only 0.613. Triggering and procedural compliance fail as independent bottlenecks, and both scores and model rankings shift with the harness, so skill use behaves as a capability conditioned on the harness rather than a fixed property of the model.

---

## 274. DataSpace: Benchmarking Data Agents for Verifiable Analytics over Heterogeneous Workspaces

**Autori:** Boyan Li, Zhuowen Liang, Yupeng Xie, Xiaotian Lin, Tianqi Luo, Xinyu Liu, Yizhang Zhu, Zhangyang Peng, Yuan Li, Zhengxuan Zhang, Jiayi Zhang, Nan Tang, Guoliang Li, Yuyu Luo  
**Data:** 2026-08-04  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.03451v1

> Data agents enable natural-language analytics over organizational workspaces, where relevant evidence may be scattered across databases, structured files, long documents, and multimedia. Existing benchmarks largely isolate structured querying, retrieval, or open-ended analysis, leaving heterogeneous evidence discovery, complete tabular outputs, and deterministic evaluation insufficiently unified. We introduce DataSpace, a benchmark in which data agents produce verifiable tabular results from task-local heterogeneous workspaces. It contains 410 cross-language tasks and 7,439 artifacts totaling 15.01 GB across CSV, JSON, SQLite, Markdown, PDF, and video. DataSpace also served as the official evaluation benchmark for the KDD Cup 2026 Data Agents for Complex Data Analysis competition. Each agent receives only a question and workspace and returns the complete requested tabular result. We construct DataSpace with DataSpace-Builder, an execution-grounded framework comprising cross-language transformation, constraint-aware relational sampling, modality routing and artifact rendering, and human review and task repair by 11 domain experts. A deterministic evaluator performs header-invariant column alignment, type- and precision-aware normalization, and order-aware row comparison. Across six recently released frontier multimodal models and five widely used agent harnesses, the best accuracy reaches 66.34%, while harness choice creates a 15.36-point spread with the backbone fixed. Multimodal evidence integration and joins consistently reduce accuracy across all six backbones. These results show that DataSpace remains unsaturated and identify key challenges for improving data-agent reliability.

---

## 275. GUI-Lens: Coarse-to-Fine Cropping for GUI Grounding with General-Purpose VLMs

**Autori:** Zichuan Fu, Shirong Wang, Wenlin Zhang, Guojing Li, Yimin Deng, Jingtong Gao, Junjia Qi, Hanyu Yan, Yefeng Zheng, Xiaopeng Li, Wanyu Wang, Xian Wu, Xiangyu Zhao  
**Data:** 2026-08-04  
**Categorie:** cs.CV, cs.AI  
**Link:** https://arxiv.org/abs/2608.03270v1

> GUI grounding maps natural-language instructions to click locations and is essential for reliable GUI agents. The task remains difficult on high-resolution, densely populated interfaces because a vision-language model (VLM) may recognize a requested control without locating it precisely enough for interaction. Most existing methods provide various forms of localization assistance, but still rely on a direct click prediction, allowing visual ambiguity or an inaccurate initial estimate to propagate to the final result. In this paper, we introduce GUI-Lens, a coarse-to-fine grounding framework that allows a general-purpose VLM to determine the target through active visual observations. Specifically, GUI-Lens extracts OCR text and detected UI components from the screenshot and presents their positions as coordinate references. Using the instruction, the current view, and these references, the VLM selects the region and scale of the next view, which is cropped and enlarged to provide finer visual details. This process continues over successively focused views until the target is determined. Proposed crops and clicks are checked against the instruction throughout the process, and the final local position is mapped back to the original screen coordinates. Experiments on four GUI grounding benchmarks and three general-purpose VLM backends show that GUI-Lens improves overall grounding accuracy by up to 24.9 percentage points and achieves state-of-the-art performance with GPT-5.5.

---

## 276. EduClaw-Bench: A Long-Horizon Benchmark for Pedagogical LLM Agents with Simulated Learners

**Autori:** Unggi Lee, Sookbun Lee, Yeil Jeong, Eunjoo Lee, Minchul Shin, Hoilym Kwon  
**Data:** 2026-08-04  
**Categorie:** cs.CY, cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2608.03206v1

> Large language models (LLMs) power educational applications from tutoring to essay scoring, but each is a point solution to a single task, and only recently have these point solutions been integrated into agents operating over a learning management system (LMS). Yet tutoring is long-horizon, since a learner improves over days and weeks rather than in a single turn, and no benchmark evaluates an agent tutor across a sustained relationship. We introduce EduClaw-Bench, a benchmark that places an agent tutor in a continuous 30-day relationship with a simulated learner grounded in knowledge tracing (KT), whose knowledge-concept mastery, from a KT model trained on real-student data, drives its answers and is probed for learning gain across 55 scenarios. Each agent is scored on three primary axes (learning gain, responsiveness, and helpfulness) and two curriculum-design axes (Gagné and Rosenshine), with helpfulness and the curriculum axes judged by a cross-family panel of three LLM judges. Evaluating 10 agent adapters over three base-model tiers yields two findings that single-tier, single-session evaluation cannot reach. First, tutoring quality belongs to the base model and the agent harness together rather than either alone. Second, almost no combination sustains good tutoring over the full horizon. A calibration check ($\text{ECE}=0.049$) and a live-classroom field study confirm that the simulated learner and its measurements track reality. Our work is a step toward trustworthy AI tutors for future education.

---

## 277. SKT: Skill-Use Training at Scale via Verified Synthetic Data Generation

**Autori:** Zelin Tan, Yiqun Zhang, Hao Li, Zhiyao Cui, Hejia Geng, Shao Zhang, Hangfan Zhang, Yang Chen, Xiaosong Wang, Lilong Wang, Zhenfei Yin, Shuyue Hu, Chen Zhang, Lei Bai  
**Data:** 2026-08-03  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.02287v2

> Agent skills have become an important mechanism for equipping language-model agents with reusable procedural knowledge. However, providing skills alone does not guarantee that current models can effectively identify, apply, and coordinate them. To improve skill-use capabilities, we introduce SKT, a verified data synthesis pipeline that constructs skill-grounded tasks and executable trajectories from large collections of agent skills. SKT selects suitable single-skill and multi-skill configurations, synthesizes tasks through rule-based and agent-based verification with feedback-guided repair, and retains only successful trajectories that substantially use every required skill. Using 2,000 public skills, SKT produces 4,000 task packages and 27,164 verified trajectories. Based on the same pipeline and a disjoint test pool, we further construct SkillEval, a held-out executable benchmark for evaluating skill use. Experiments across diverse models, benchmarks, and agent harnesses show that supervised fine-tuning on SKT-generated trajectories consistently improves skill-use performance. Verification ablations, cross-harness evaluation, and scaling experiments further demonstrate that these gains depend on high-quality supervision, extend beyond a single agent interface, and increase with broader skill coverage. Together, these results establish verified data synthesis as an effective and scalable approach for skill-use training.

---

## 278. Harness-R1: Learning to Edit Executable Runtime Harnesses from Agent Failure Trajectories

**Autori:** Shuai Shao, Kangning Zhang, Qingyao Li, Shijian Wang, Hao Wang, Wenxiang Jiao, Yuan Lu, Yi Guo, Weiwen Liu, Weinan Zhang  
**Data:** 2026-08-03  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.02276v1

> Agents built around large language models continually accumulate interaction trajectories during deployment, yet their behavior typically remains fixed. Beyond updating model weights, these trajectories can improve the agent harness that constructs context, mediates tools, validates actions, and recovers execution. We introduce Harness-R1, the first method, to our knowledge, that makes failure-conditioned, lifecycle-wide editing of an existing executable runtime a learned capability. It post-trains a dedicated harness engineer with online reinforcement learning so that its edits are optimized for the realized task success they produce, rather than proposed by a fixed editor. A separate 9B engineer converts batches of target-agent failures into validated executable patches; fresh same-batch reruns of the frozen target provide outcome rewards, so training updates only the engineer. Cold-start supervised fine-tuning initializes this editing policy, which is then trained online with group-relative policy optimization. Across WebShop, ALFWorld, and DBBench, Harness-R1 raises vanilla Qwen3.5-9B success from 44.3% to 53.6% (+9.3 percentage points). After direct target-agent fine-tuning, a target-specific engineer raises the average further from 59.2% to 64.2% (+5.0 points); because these gains hold both before and after fine-tuning the target, Harness-R1 points toward co-evolving the harness engineer and the target agent.

---

## 279. LongHorizon-Harness: Advancing Long-Horizon Agents for Real-World Tasks

**Autori:** Ziyu Ma, Hailang Huang, Shun Zou, Yong Wang, Shidong Yang, Yiming Hu, Fei Wei, XiangXiang Chu  
**Data:** 2026-08-03  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2608.01964v1

> Large language model (LLM) agents increasingly undertake long-horizon tasks that require sustained reasoning, tool use, and revision across many interdependent steps. However, existing agent harnesses maintain task execution, task state, and completion assessment within a growing context, making the state difficult to track and allowing incorrect self-assessments to propagate into later decisions. We reformulate long-horizon execution as a task-state management problem and propose LongHorizon-Harness, which maintains the task state explicitly outside execution and updates it only with facts independently verified from the environment. Its Manage-Execute-Audit(MEA) loop uses a manager to maintain the task state and determine the next subtask, a fresh-context executor to perform it, and a read-only auditor to verify the resulting environment state before the next round. A lightweight AgentAdapter supports interchangeable model and harness backends without modifying their native agent loops. LongHorizon-Harness improves Qwen~3.7-Plus from 51.8% to 80.7% on WeaveBench, from 69.7% to 77.2% on Terminal-Bench~2.1, and from 2.8% to 8.3% on OSWorld~2.0. It also raises Claude Opus~4.7 from 20.0% to 34.3% on an OSWorld2.0 subset, demonstrating consistent gains across models, harnesses, and interaction domains.

---

## 280. HarnessCompass: Guiding Automatic Harness Evolution toward Generalizable and Effective Agent Harnesses

**Autori:** Luan Zhang, Ruochen Zhou, Dandan Song, Zhengyu Chen, Yuhang Tian, Jun Yang, Huipeng Ma, Chenhao Li, Guangyuan Feng, Xudong Li, Yizhou Jin, Yan Xu  
**Data:** 2026-08-03  
**Categorie:** cs.LG, cs.CL  
**Link:** https://arxiv.org/abs/2608.01918v1

> Harness design plays a critical role in agent performance by shaping how large language models (LLMs) perceive, reason over, and act within executable environments. Recent work has proposed automatic harness evolution, which iteratively improves the harness from agent--environment interactions. However, existing methods often overfit to the evolution tasks, rely exclusively on trajectory-derived signals, and optimize harness components jointly, causing interference across components. We propose HarnessCompass, a novel automatic harness evolution framework built around constrained evolution, proactive feedback, and component-wise optimization. HarnessCompass first enforces global constraints on evolution, restricting modifications to task-agnostic harness changes that generalize beyond the evolution tasks. It then augments trajectory-derived evidence with proactive first-person feedback from the agent about harness usage, yielding richer signals for evolution. Finally, it decouples the optimization of different harness components before consolidating them into a unified harness, reducing cross-component interference while preserving component synergy. On SWE-bench Verified with GPT-5.4, HarnessCompass improves Pass@1 from 54\% to 66\% in only 5 evolution iterations, outperforming AHE in both effectiveness and evolution efficiency. In addition, the evolved harness transfers effectively to held-out tasks and other models, demonstrating substantially stronger generalization than prior automatic harness evolution methods.

---

## 281. Hear, Invoke, and Understand: A Skill-Calling Multimodal Agent for Large Audio Language Models

**Autori:** Yuwen Wang, Tian-Hao Zhang, Minghao Cai, Yilin Ren, Ziyang Jiang, Xin Wang, Zhichao Wang, Pan Zhou, Kun Zhan, Xinyuan Qian  
**Data:** 2026-08-03  
**Categorie:** cs.MM, cs.AI  
**Link:** https://arxiv.org/abs/2608.01881v1

> Complex acoustic problems may require models to perform acoustic operations, interact with external tools and reason over the resulting textual or processed-audio observations rather than answer directly from a fixed audio input. We study such problems as tool-interactive audio reasoning and develop SpeechAgent-R, an audio agent that coordinates its intrinsic multimodal understanding with external skills and tools. To support this capability, we construct HIU-Corpus, comprising 65,492 interaction trajectories and 507.6 hours of audio across 24 tasks, 8 skills and 9 tools. SpeechAgent-R first learns structured interaction behaviors through trajectory-based supervised fine-tuning and then improves its decisions through multi-turn reinforcement learning. We further introduce HIU-Bench to jointly evaluate task performance, interaction quality and generalization to diverse task settings. It contains 1,395 samples across 56 tasks, including in-distribution (ID) and out-of-distribution (OOD) splits with substantial shifts in tool usage and workflow composition. SpeechAgent-R achieves 84.17 on ID tasks and 70.94 on OOD tasks, improving over the base model under the same agent harness by 15.40 and 14.23 points. These results demonstrate that learning skill and tool coordination improves audio agents' ability to handle diverse task settings and adaptive tool interactions.

---

## 282. Constructing Executable Analytical Knowledge Representations for Meta-Analysis Synthesis Using an Agentic Harness

**Autori:** Lingbo Li, Anuradha Mathrani, Teo Susnjak  
**Data:** 2026-08-03  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.01711v1

> Meta-analysis synthesis highlights a fundamental challenge in knowledge-based scientific analysis: structured evidence does not by itself represent the analytical knowledge required for executable computation. Decisions about evidence assignment, analytical contrasts, outcome and time-point alignment, effect-size formulation, and methodological admissibility must be explicit before statistical execution. Existing automated approaches often embed these decisions in model outputs, generated code, or workflow traces rather than representing them as independently verifiable knowledge. We introduce the Executable Analytical Knowledge Representation (EAKR), a machine-actionable representation of the knowledge required to transform structured evidence into executable meta-analysis. An EAKR represents evidence, relations, numerical inputs, constraints, provenance, and unresolved issues. We operationalise EAKR in MetaSynDec, an agentic harness in which large language models propose structured updates and deterministic services govern schema- and contract-based validation and execution. Across 58 synthesis units, MetaSynDec constructed all EAKRs, with 57 proceeding to statistical execution. Of 56 units with sufficient information to define a reference analysis object, 38 (67.9%) achieved complete object fidelity and 42 (75.0%) exact evidence-set agreement, with a mean Jaccard similarity of 0.909. Generated and published confidence intervals overlapped in 54 of 55 units (98.2%). MetaSynDec outperformed direct LLM generation in reference synthesis-structure agreement (57/58 versus 23/58; p<0.001) and among 23 jointly completed units, exact reference-formulation agreement (23/23 versus 1/23; p<0.001). These findings provide feasibility evidence that EAKR supports formal validation, traceability, statistical execution, and improved methodological agreement relative to direct LLM generation.

---

## 283. GABench: A Comprehensive Benchmark for Evaluating LLM Agents on Graph Analysis Tasks

**Autori:** Jiarui Tan, Zhongjian Zhang, YaBo Guo, Jiawei Liu, Yujie Xing, Muhan Zhang, Cheng Yang, Chuan Shi  
**Data:** 2026-08-03  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.01684v1

> Large language model (LLM) agents are increasingly capable of planning, using tools, and interacting with external environments. They are typically supported by harnesses, which manage state and coordinate multi-step execution. Graph analysis provides a promising setting for evaluating their agentic capabilities, because it requires agents to access data and execute operations in a graph environment. However, existing graph benchmarks for LLMs provide limited coverage of graph tasks and graph types, making it difficult to comprehensively evaluate LLM agents. Moreover, they typically formulate graph analysis as text-based question answering, where graph information is directly provided in the prompt, limiting the evaluation of end-to-end agentic capabilities. To address these limitations, we introduce GABench, a comprehensive benchmark for agentic graph analysis. GABench spans three graph types and covers four graph analysis task categories: graph retrieval, graph theory, graph machine learning, and graph open-ended question answering. GABench also provides 84 executable tools for accessing graph data and performing diverse graph operations. Building on these tools, we develop an agentic graph analysis task generation pipeline and construct 10,400 tasks with verifiable ground truth.Using GABench, we evaluate a range of frontier LLMs and agent harnesses. Our experiments reveal three key findings: (1) Existing LLM agents still struggle with complex graph analysis tasks. (2) Harness choice significantly affects performance, yet existing harnesses remain limited on complex graph tasks. (3) Graph analysis depends more on tool-call quality than quantity. Our findings provide practical insights into the development and evaluation of LLM agents for graph analysis.

---

## 284. PATH-Bench: Path-Dependent Evaluation of Lifelong Agents

**Autori:** Xidong Yang, Xingyi Zhang, Wenhao Li, Wenyan Liu, Junjie Sheng, Yun Hua, Wei Yin, Tao Fang, Chuyun Shen, Xiangfeng Wang  
**Data:** 2026-08-02  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.01149v1

> Lifelong LLM agents increasingly adapt through external learning states that store past interactions as retrievable memories or reusable skills, yet existing benchmarks rarely account for how the path of accumulated experience shapes what agents transfer and retain. In this work, we establish PATH-Bench, a benchmark for path-dependent evaluation of lifelong agents. PATH-Bench estimates directed task relationships via multi-model in-context learning, constructs probe-centered sequences with controlled helpful and interfering histories, and repeatedly evaluates probe tasks to measure average performance, forward transfer, backward transfer, and forgetting. We evaluate eight representative agents on single-turn code generation and multi-turn tool-use tasks under positive- and negative-dominant histories. Benchmark results show that experience utility depends jointly on how experience is represented and on the task's interaction structure, that strong transfer does not ensure retention, and that later experience can reshape gains acquired earlier in the learning path. Based on these findings, we propose Selective Experience Use (SEU), an agent harness that regulates how path-accumulated experience influences each new task, admitting helpful items while filtering out potential interference. SEU consistently reduces forgetting while improving forward transfer in the majority of settings. The PATH-Bench provides both a controlled evaluation framework and actionable guidance for designing more selective and robust lifelong agents.

---

## 285. DrawAI: Agentic Benchmark and Workflow for Making Raster Images Editable

**Autori:** Pu Cao, Qingye Kong, Xuedan Yin, Xuekun Zhao, Rupeng Yan, Qing Song, Yao Zhang, Lu Yang  
**Data:** 2026-08-01  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2608.00548v1

> Recent image-generation models and multimodal agents can produce high-quality visuals for increasingly complex visual communication tasks. Yet their raster outputs remain difficult to use directly because meaningful content and relationships are flattened into pixels, preventing users from inspecting, modifying, rearranging, or reusing individual components. We formulate image-to-editable reconstruction, which recovers a structured, directly manipulable artifact from a raster image while preserving its visual and semantic content. The central challenge is to jointly satisfy Fidelity and Editability, which often trade off in practice. To study this task, we introduce DrawAI, comprising an agentic benchmark, DrawAI-Bench, and a reconstruction workflow, DrawAI-Flow. DrawAI-Bench spans scientific figures, presentation slides, posters, and diagrams, combining real and AI-generated images to reflect practical visual-creation scenarios. It evaluates Fidelity and Editability through a hybrid protocol of 39 criteria: deterministic rule-based metrics measure properties with direct correspondences, while asset-specific vision-language rubrics capture semantic and perceptual qualities for which exact matching is misleading. Besides, we propose DrawAI-Flow, a two-stage agentic workflow in which a Parser Agent turns extracted elements evidence into an explicit reconstruction plan, and a Reconstruction Agent realizes the plan as executable graphics code through an iterative code-render-validate-revise loop. On DrawAI-Bench, we systematically evaluate thirteen models across five agent harnesses to study the effects of model capability, harness choice, and workflow design. The results show that reconstruction quality and costs vary substantially across model-harness configurations, while DrawAI-Flow consistently improves editable structure.

---

## 286. CurveShift: Is Agent Progress Scalar? Separating Level from Shape

**Autori:** Hanwen Xing, Pengyun Wang, BingXu Meng, Kumail Alhamoud, Xiang Li, Jicheng Wang, Xin Yu, Xinyang Han, Xiaomin Li, Philip Torr, Yuexing Hao  
**Data:** 2026-07-31  
**Categorie:** cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2608.00355v1

> Progress in large language models is often summarized using a single scalar measure, such as a time horizon, a latent ability estimate, or an aggregate benchmark score. These summaries capture the overall performance, but they do not test whether progress is distributed differently across task difficulty. We find that most of the apparent shift in gains toward harder tasks does not reflect a change in the shape of the difficulty-response curve. On METR time-horizon data, a single Rasch model with rising ability reproduces this pattern, so it is largely explained by ceiling effects rather than a qualitative change in capability. This echoes how the choice of metric can make claimed emergent abilities look like a property of the models themselves. We then identify a smaller hard-task effect that survives this control. Isolating it is difficult on agentic benchmarks, because newer models are usually run with newer agentic harnesses, so a gain on hard tasks cannot be assigned to the model or its scaffold. We break the confound with LiveCodeBench, a public competitive programming benchmark that runs no agentic scaffold while pairing dated models with an exogenous difficulty ordering. After accounting for the rise in overall ability, models released after September 2024 still gain on the hardest problems beyond what their easy and medium performance predicts, by about +0.40 logits under our most conservative assumption, raising the hard-problem solve rate from roughly 18% to 25%. The effect is led by the strongest reasoning models and holds for hard tasks that need only short reasoning, not autonomy over long horizons. We present this as a result specific to competitive programming, since our clean identification rests on a single coding benchmark. We release the LiveCodeBench Difficulty Panel (66 dated models x 1,055 problems) and our analysis code.

---

## 287. AutoFyn Technical Report: Non-Parametric Expert Iteration for Long-Horizon Agents

**Autori:** Adib Hasan, Daniel Schaffield, Akashnil Dutta, Tarik Adnan Moon  
**Data:** 2026-07-31  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2609.05446v1

> We introduce AutoFyn, an agent harness inspired by the Expert Iteration algorithm, adapting a frozen model across many rounds by updating persistent state from verified reward signals rather than model weights. Each round begins from a fresh model session, and durable information is reintroduced only through explicit interfaces such as persistent memory files, reports, and repository state. Within a round, an orchestrator explores, plans and builds many alternative approaches with specialized agents, while a task-grounded verifier verifies the work and supplies an objective reward for measuring progress. This reward is distilled back into the persistent state, which updates the effective policy for the next round. In this technical report, we formalize this loop and describe its persistent state and verification interfaces. We then demonstrate its use in three domains, namely olympiad mathematics, data science, and cybersecurity. On the six fresh problems of the 2026 International Mathematical Olympiad, every model with room to improve scores higher under AutoFyn than in its provider's own coding agent. AutoFyn also built the top-ranked agent on the Spider 2.0 dbt benchmark, and has produced $16$ maintainer-confirmed vulnerability advisories in Next.js, MetaMask, pnpm, Warp, LiteLLM, Langflow, and Open WebUI.

---

## 288. RecHarness: A Bandit-Routed Agentic Harness for Self-Evolving Recommender Systems

**Autori:** Haoran Ling, Yuecheng Li, Zeyu Song, Jing Yao, Shuwen Kang, Chi Lu, Wenjin Wu, Peng Jiang  
**Data:** 2026-07-31  
**Categorie:** cs.IR, cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2607.29241v1

> Optimizing modern recommender models still depends heavily on engineers manually iterating over architectural, objective, and training-strategy changes. While LLM-based agents can automate this trial-and-error process, allowing the LLM to both select modification directions and generate concrete hypotheses often leads to unstable search under limited experiment budgets. Inspired by the above challenge, we propose RecHarness, a Bandit-Routed Agentic Harness for automated recommender model optimization. RecHarness separates the optimization process into two steps: a bandit router selects the next modification direction according to historical validation feedback, while the LLM generates a concrete optimization hypothesis and executable code edit within the selected direction. To sustain long-horizon exploration, RecHarness uses a jump-basin mechanism to activate a structural-jump arm when local edits stagnate. Across multiple recommendation tasks, datasets, and model backbones, RecHarness achieves more stable performance improvements and uses limited trial budgets more effectively than LLM-reasoning search. During a 7-day online A/B test on a large-scale short-video advertising platform, the selected candidate improves ADVV by 2.084%, Revenue by 0.534%, and Exposure by 0.559%. Code is available at https://github.com/6lyc/RecHarness.

---

## 289. DarwinX: Evolving Agent Harnesses Through Natural Selection

**Autori:** Yifan Zhang, Yutong Dai, Juntao Tan, Luyu Yang, Rishi Mullur, Thai Hoang, Zhiyuan Hu, James Zhu, Phil Mui, Silvio Savarese, Ran Xu, Zeyuan Chen  
**Data:** 2026-07-31  
**Categorie:** cs.NE, cs.AI, cs.LG, cs.SE  
**Link:** https://arxiv.org/abs/2608.07545v1

> An LLM agent's capability depends not only on model weights but on its harness: prompts, tools, skills, and control flow. Self-improvement loops already edit harnesses, yet single-lineage search is path-dependent and local wins often regress other tasks. We introduce DarwinX, which treats self-evolution as selection over a population of harnesses with the model frozen: a preserve-and-extend contract admits only variants that extend coverage without regressing, an archive keeps alternative lineages for recombination, and failure-, teacher-, and self-derived evidence share one edit interface. Fitness comes from each benchmark's own verifier: no gold solutions, no hand-picked winners. Across four benchmarks that progressively separate the evolution signal from the test, one loop adds about 17 points on average: Terminal-Bench 2.1 rises +7.7 to 83.2% on a matched base and to the verified frontier at 84.7% on a stronger one; TerminalWorld's held-out split reaches 68.3%, ahead of every off-the-shelf agent; WebArena-Infinity real-task pass@1 rises from 43.5% to 93.0% audit-clean; and a Terminal-Bench 2.1 harness transfers unchanged to SWE-bench Verified. What evolves is general agent competence, not benchmark-specific patches, so it survives changes of task, verifier, and base model. A frozen model need not be a fixed agent: harness selection turns evaluation compute into durable capability.

---

## 290. AgentRadio: Passive Awareness for Long-Horizon Multi-Agent Collaboration

**Autori:** Xinxing Ren, Qianbo Zang, Ziyan Wang, Caelum Forder, Suman Deb, Peter Carroll, Zekun Guo  
**Data:** 2026-07-30  
**Categorie:** cs.MA  
**Link:** https://arxiv.org/abs/2607.28430v1

> Understanding large codebases is a long-horizon task for Large Language Model (LLM) agents: answering a single question can require building and running the software, tracing execution across files, and synthesizing evidence over tens of minutes. On SWE-Atlas QnA, a benchmark of long-horizon questions over production repositories, a single Claude Code agent (Opus 4.6) resolves only 32.3% of tasks. Dividing the work among agents with clean contexts mitigates this limitation. However, the subtasks of code comprehension are interdependent. One agent's findings can rewrite another's task, so agents must coordinate during execution, not only at phase boundaries. Existing multi-agent systems support such exchange only between phases, through staged handoffs or synchronized rounds. Communication and work remain mutually exclusive. A discovery made mid-execution cannot be shared until the next boundary. We present AgentRadio, an asynchronous message-passing layer that equips coding-agent harnesses with three primitives: threads, messages, and waiting for mentions. The last runs as a background task, surfacing teammates' messages without interrupting foreground work, so each agent remains passively aware of its peers and folds new findings into its ongoing task. Under a five-phase protocol of division of labor and negotiation, four agents organized by AgentRadio resolve 62.1% of tasks, 29.8 points above a single agent and above Claude Code with the newer Opus 4.8 (57.2%). Rubric-level analysis shows the gain growing with task difficulty, consistent with mid-course correction as the underlying mechanism. Our code is available at https://github.com/Coral-Protocol/AgentRadio.

---

## 291. Distilling Answer Set Programming Theories from Large Language Models

**Autori:** Nelson Higuera Ruiz, Markus Hofmarcher, Claudiu Leoveanu-Condrei  
**Data:** 2026-07-30  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2607.28086v1

> Writing Answer Set Programming (ASP) theories from scratch is a difficult and time-consuming task. We take a neurosymbolic approach to study whether a model can distill complete and correct theories, given a fixed agent harness with the solver in the loop. The protocol is dataset-agnostic: with a single prompt and an empty file as the starting point the model is given a 1-hour time limit to derive a complete theory. We chose VQA as the application domain, three benchmarks (CLEVR, GQA, CLEVRER), as these are publicly available and non-trivial. In order to study the model scale required for solving this task we nine different models: four frontier (Claude Sonnet 4.6, Claude Opus 4.7, GPT-5, DeepSeek V4 Pro), two mid-tier (DeepSeek V4 Flash, gpt-oss-120b), and three open-weights (qwen3.6-27b, gpt-oss-20b, qwen3.5-9b). Three of four frontier models reach 100% on CLEVR and 92.8%-98.8% on GQA; on CLEVRER, Sonnet, Opus, DeepSeek V4 Pro score 92.7%-95.3%. GPT-5 reaches 98.7% on CLEVR but drops to 41.8% on GQA and to 86.7% on CLEVRER. Adding handwritten reference theories from other datasets moves the other three frontier models by at most +/-3.4 pp but reduces GPT-5's accuracy by 3-19 pp. We release the code, prompts, and theories distilled.

---

## 292. SKIMIX: Multi-Agent Harness-Time Scaling with Skill Mixture for Dynamic Harness Engineering

**Autori:** Jia Luo  
**Data:** 2026-07-30  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2607.27994v1

> AI agents increasingly rely on large skill libraries, but selecting, combining, and maintaining skills remains difficult. We propose SKIMIX, a multi-agent framework in which agents with different skill portfolios collaborate through iterative refinement. SKIMIX combines embedding-based skill retrieval, submodular anti-dilution routing, and adaptive skill evolution. Across six reasoning benchmarks, multi-agent collaboration substantially improves open-ended mathematical reasoning but offers limited or negative gains on multiple-choice tasks. Agent-count scaling is non-monotonic, and most improvements arise during the first refinement round. These results show that task characteristics determine whether skill-level ensembles help and provide practical guidance for scalable agent design.

---

## 293. Albilich: Steerable Proof-State Orchestration for LLM-Based Mathematical Research with CAS Integration

**Autori:** Ting Gong, Michael Ruofan Zeng, Yong Yang  
**Data:** 2026-07-30  
**Categorie:** cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2607.27705v1

> Large language models can contribute useful ideas to mathematical research, yet long-horizon proof attempts remain difficult to coordinate, evaluate, and reproduce. We present Albilich, an open-source agentic harness for autoresearch in mathematics that combines long-horizon reasoning, computer algebra systems (CAS), literature retrieval, and persistent SQLite-based context management. We evaluate Albilich on the RealMath benchmark (Zhang et al. 2025) and on open problems in group theory from the Kourovka Notebook (Khukhro and Mazurov 2026). It solved 10/10 problems on RealMath with CAS and 9/10 with no CAS. On the Kourovka problems, Albilich produced a counterexample to Problem 21.142 and a proof of a strengthening of Problem20.2. Anablation on Problem 17.91 demonstrates 32.0% token reduction when CAS is enabled. An ablation on Problem 21.142 demonstrates higher verifier-rejection rate and failure to synthesize proof routes in the absence of the advisor agent. These results support Albilich as a human-steerable, CAS-boosted environment for scalable AI-assisted mathematical research.

---

## 294. Scores Are Not Decisions: Cost-Aware Stopping for Tool Acquisition in LLM Agents

**Autori:** Yicheng Feng, Yan Zhang, Yan Cheng, Wei Qi  
**Data:** 2026-07-29  
**Categorie:** cs.LG, cs.AI  
**Link:** https://arxiv.org/abs/2607.27083v1

> As LLM agents increasingly depend on diverse external services such as search engines, databases, and connectors, agent harnesses face a fundamental tool-selection challenge: acquiring too few tools leaves the task under-informed, while too many adds cost, context load, and privacy exposure. Routers and retrievers can rank candidate tools by relevance, but a ranking alone does not determine how many are worth selecting. Existing approaches leave acquisition under heterogeneous costs unaddressed. We formulate this decision as cost-aware marginal decision-focused stopping (CAM-DF) over ranked tool prefixes, with CAM-DF-lite as a compact interpretable variant. We train directly on the offline gap between stopping now and the best continuation: its sign labels the decision, its magnitude weights each error by the payoff at stake. We prove this objective is Bayes-aligned with the stopping target and that score-only rules are suboptimal under heterogeneous costs. We evaluate on 1,343 tasks across five tool-use domains. On $τ$-bench Retail, CAM-DF attains the highest payoff among deployable methods, with gains over a predict-then-threshold baseline across all five ranking sources and two cost regimes. Our approach is state-of-the-art under heterogeneous costs and high cost pressure, with larger gains under weaker rankings. In live execution, CAM-DF exposes the agent to 37\% fewer tools than full access while maintaining comparable task success. The CAM-DF family is a lightweight pre-execution plugin that turns existing tool rankings into lower-cost acquisition decisions without fine-tuning the underlying LLM.

---

## 295. MemSecBench: Tracking Agent Memory Poisoning from Persistence to Consequence and Repair

**Autori:** Xuanze Chen, Xukang Xie, Wentao Fu, Jiajun Zhou, Shanqing Yu, Qi Xuan  
**Data:** 2026-07-29  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2607.27080v1

> Memory systems allow agents to retain and reuse information from past interactions, but they can also let malicious content persist. A malicious instruction crafted by an attacker may be stored in long-term memory, recalled much later, and quietly shape a real action. Recent benchmarks increasingly examine agent memory security, yet few trace the same malicious semantics across persistence, downstream consequences, and selective repair under diverse memory-backend comparisons. To address this gap, we introduce MemSecBench, a task-grounded benchmark for the lifecycle security of agent memory systems. It contains 310 cases drawn from 48 realistic contexts across code and science, daily life, and office work. Each case follows a controlled Write--Execute--Forget protocol in an isolated runtime under an exact agent configuration, defined by an agent harness, a memory backend, and an LLM backend. Evidence-based adjudication combines a deterministic write check, checkpoint-specific judge-model evaluations, and programmatic gates across seven lifecycle checkpoints. The experimental design spans a 24-configuration matrix of two agent harnesses, four memory backends, and three LLM backends. Across all 24 configurations, malicious memory persists in 84.2% of all cases, and the full Write--Execute chain succeeds in 50.3%. Among successfully poisoned cases, 59.6% complete the full Execute chain, while 56.1% achieve selective repair.Compared with matched Native configurations, the largest absolute differences are 16.1 percentage points for end-to-end attack success and 41.3 percentage points for selective repair. These descriptive contrasts indicate that the evaluated memory system stacks differ in lifecycle security, both in the propagation of malicious memory and in selective repair after successful memory poisoning.

---

## 296. SecRespond: Benchmarking AI Agents for Real-World Post-Compromise Incident Response

**Autori:** Lehan Wang, Boli Chen, Ruixue Ding, Pengjun Xie, Jinwei Huang, Zhendong Liu, Shuo Wang, Tao Lei, Xin Ouyang, Xiaomeng Li  
**Data:** 2026-07-29  
**Categorie:** cs.CR, cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2607.26791v1

> Large Language Model (LLM) agents are increasingly adopted in real-world security operations with access to host artifacts and command-line interfaces (CLIs), making it critical to thoroughly assess their security capabilities. However, existing cybersecurity benchmarks focus on pre-compromise settings where agents are placed in a clean and idealized environment before an attack occurs. This leaves the post-compromise setting underexplored. To address this gap, we introduce SecRespond, the first benchmark for evaluating LLM agents on the post-compromise incident-response workflow. Given a forensic disk snapshot of a compromised host together with the alerts, vulnerability scans, and baseline checks reported by a host security product, agents are required to produce forensic reports on intrusions, baseline risks, and vulnerability risks, together with a remediation plan. We instantiate this task across 10 cyber ranges, each constructed from a distinct compromised cloud host, spanning 4 entry-point types, 21 ATT&CK techniques, and 5 operating systems. We evaluate 23 frontier LLMs on the OpenCode agent harness. Experimental results show that although current agents can reliably uncover the problems exposed by alerts, they struggle to proactively investigate the disk for silent intrusions and to produce comprehensive, verified remediation plans, with no model achieving complete detection and remediation on any single range. This reveals a fundamental bottleneck in building agents for real-world incident response. The benchmark is publicly available at https://github.com/Alibaba-NLP/qqr/tree/main/data/secrespond.

---

## 297. Living-Harness Is an Interactive-Agent Evolver

**Autori:** Yuetian Du, Yucheng Wang, He Xu, Jiexu Xu, Shanwen Tan, Bing Zhao, Boyu Yang, Zhijie Xu, Ming Kong, Hu Wei, Jie Liu, Qiang Zhu  
**Data:** 2026-07-29  
**Categorie:** cs.MA, cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2607.26598v2

> Large language model (LLM) agents may recover from a failure within an episode or after a retry, yet the same execution failure can recur in later tasks because post-episode feedback rarely revises the persistent harness that guides future interactions. Static harnesses improve reliability through fixed tools, context, memory, and workflow structures, but remain unchanged after deployment. We propose $\textbf{Living-Harness}$, a self-evolving agent harness that converts each completed trajectory and its evaluator signals into posterior evidence for bounded harness updates. Guided by a domain-level $\textbf{Evolution-SOP}$ ($\textbf{S}$tandard $\textbf{O}$perating $\textbf{P}$rocedure), Living-Harness extracts an episode abstraction and structured update evidence, and writes two complementary forms of procedural knowledge: episodic memory that records trigger conditions, failure patterns, and recovery actions, and a state graph that records state nodes, repair edges, and transition rules. The updated harness state is retrieved to guide future interactions, while tools and base context remain frozen, allowing procedural repairs to accumulate across evolution cycles. On eight interactive environments derived from $τ^2$-Bench and MultiWOZ-2.4, Living-Harness improves average Pass@1 over the strongest interactive baseline by 10.07 and 9.91 percentage points, respectively, and supports retrieval-only reuse of the evolved harness state across model backbones. Our code will be made publicly available soon at https://github.com/anotherbricki/Living-Harness.

---

## 298. Distributing Security Controls Through Harness Engineering

**Autori:** William Robert Gore  
**Data:** 2026-07-28  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2607.25890v1

> AI coding agents are being adopted at historic speed, yet security and risk concerns remain the primary barrier to scaling agentic AI across organizations. Existing security controls for coding agents are not systematically distributed to engineering teams, and vendor-native solutions introduce ecosystem dependencies that may not suit every deployment context. This paper investigates whether off-the-shelf security controls can be implemented on commercial AI coding agents and scaled to a distributed user base via a custom agent harness. A phased testing methodology was applied across four agent configurations --- two commercial agents with and without controls, a baseline harness, and a security-hardened harness --- using a 23-test suite derived from the OWASP Top 10 for Agentic Applications. SHarD (Secure Harness Distribution), a distributable harness built on the Pi agent harness, demonstrated that three categories of security controls --- OS sandboxing, skill scanning, and tool restriction --- can be embedded and distributed via a single install command while retaining equivalent efficacy to direct installation on commercial agents. SHarD achieved an adjusted score of 100\%, matching the best securely configured commercial agent, with no regression across any test category. Notable observations include evidence that model non-determinism produces inconsistent security outcomes and that autonomous agent behavior can cross system boundaries in ways that OS sandboxing directly mitigates. Initial characteristics toward a control harness fitness framework are proposed, and a third research question is identified for future investigation.

---

## 299. CHILL-Harness: Counterfactual Harness Learning for Efficient Reasoning in Long-Horizon Agents

**Autori:** Jiarun Fu, Lizhong Ding, Sida Chen, Honglei Xin, Chunhui Zhang, Pengqi Li, Qiuning Wei, Ye Yuan, Guoren Wang  
**Data:** 2026-07-28  
**Categorie:** cs.MA  
**Link:** https://arxiv.org/abs/2607.25825v1

> Agent harnesses have become the operational infrastructure of modern large language model agents, coordinating context, tools, verification, and execution control to translate latent model capability into reliable long-horizon behavior. However, reliable long-horizon behavior requires harness control to adapt to task demands, execution environments, and evolving execution states, whereas current harnesses predominantly rely on hand-crafted or globally fixed policies; this mismatch manifests as unnecessary computational overhead and, in adverse cases, reduced task success. To address this limitation, we formulate the task of enabling adaptive orchestration in harness systems as a causal learning problem and propose Counterfactual Harness Intervention Learning for Long-Horizon Agents (CHILL-Harness). CHILL-Harness intervenes at the orchestration layer to enable advantage-guided workflow adaptation, thereby improving reasoning and execution efficiency while preserving task performance. Specifically, we develop causal intervention effect learning as the effect-estimation component of CHILL-Harness to estimate intervention-relative workflow advantage from confidence-weighted execution evidence and identify advantageous workflow adaptations. We further introduce advantage-realizing causal orchestration as its realization component to adaptively allocate counterfactual reasoning and realize only workflow adjustments supported by sufficient expected advantage. Finally, we incorporate a success-preserving objective and advantage-margin authorization constraints into CHILL-Harness to promote reliable adaptation. Extensive experiments on heterogeneous long-horizon tasks spanning information seeking, software engineering, and terminal interaction show that CHILL-Harness consistently preserves or improves task success while substantially reducing token consumption and execution time.

---

## 300. WorkSurface-Bench: Benchmarking Enterprise Agents on Multi-Surface Knowledge Routing

**Autori:** Hao Liang, Meiyi Qiang, Sizhe Qiu, Linzhuang Sun, Wentao Zhang  
**Data:** 2026-07-28  
**Categorie:** cs.CL, cs.DB  
**Link:** https://arxiv.org/abs/2607.25765v1

> Enterprise agents often need to integrate heterogeneous knowledge sources: documents for narrative facts, tables for computation, and dependency graphs for file relationships. Existing benchmarks typically evaluate retrieval or tool use without distinguishing whether an agent first selects the appropriate knowledge sources. We introduce WorkSurface-Bench, a benchmark for evaluating this capability as surface routing. It contains 1,151 atomic tasks derived from persona-scoped Workspace-Bench-Lite workspaces, spanning document, table, graph, and cross-surface questions. Its reference answers are auditable: table answers are reproduced through executed DuckDB queries, document answers are grounded in verified text spans, and graph answers are traced to source dependency annotations. We evaluate four model backbones across six controlled agent settings, yielding 27,624 protocol-error-free trajectories. Under gold-constrained tool access, agents achieve 98.7-99.8 Route F1, while Answer remains only 56.1-75.3 percent, showing that correct surface selection is necessary but insufficient for task completion. Matched interventions further show that surface hints improve Answer for three of four models, whereas removing irrelevant tools primarily improves routing and efficiency. In an independent three-annotator audit, all 200 sampled tasks pass all six quality criteria by majority vote, with 192 receiving unanimous judgments on every criterion. We release the dataset, construction pipeline, scoring code, and agent harness at https://github.com/haolpku/WorkSurface-Bench.

---

## 301. SIREN: Towards End-to-End Extreme-Weather Early Warning with Experience-Grounded LLM Agents

**Autori:** Hang Ni, Weijia Zhang, Fan Liu, Mengqian Lu, Hao Liu  
**Data:** 2026-07-27  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2607.24588v1

> Early warning of extreme weather is essential for mitigating the societal, economic, and environmental risks posed by hazardous weather events. However, expert-centered warning workflows are costly, labor-intensive, and difficult to scale throughout the warning-to-action process. Although recent advances in Large Language Model (LLM) agents have enabled the automation of weather-related tasks, existing studies remain centered on isolated scientific tasks and overlook the chain of interdependent processes required for operational extreme-weather early warning. To bridge this gap, this study investigates automated end-to-end extreme-weather early warning through LLM agents. We first develop SIREN-Bench, a comprehensive benchmark comprising 600 question-answer instances across 19 tasks, and covering four individual warning procedures and an end-to-end warning chain. Evaluation on SIREN-Bench reveals substantial capability gaps in existing weather agent frameworks. This motivates us to develop SIREN, an experience-grounded agent framework inspired by experts' use of historical cases, which combines an agentic execution environment integrating heterogeneous weather evidence and tools with a family of agent harnesses that exploit historical cases through retrieval, skill distillation, and predictive modeling. Extensive experiments demonstrate that SIREN outperforms weather-agent baselines on both individual warning procedures and end-to-end warning chains.

---

## 302. From Proposal to Verified Effect: Praxa, an Evidence-Bound Harness for Governed AI Agent Execution

**Autori:** Stefan G. Creadore  
**Data:** 2026-07-27  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2610.00015v1

> Large-language-model agents can propose and execute actions, but proposal, authority, dispatch, verified external effect, and serving promotion are different claims. We present Praxa, an agent harness that represents these states explicitly through deterministic admission, brokered execution, external read-back, reconciliation, and reviewed promotion. We report four evidence lanes. First, an author-run repository-local audit at a pinned revision passed 1,027/1,027 unit tests and 89/89 Workerd tests, instrumented all 363 expected source files, and met four coverage floors; raw per-test transcripts and independent reproduction are unavailable. Second, in a provider-backed Terminal-Bench Core 0.1.1 pilot across 12 curated tasks, baseline and reliability-layer arms each passed 17/36 strict trials. The reliability layer used 37.49% more input and 50.73% more output tokens, so the pilot does not support superiority. Third, in a post-debug, two-order coordination-proxy development comparison, baseline and a source-authored candidate each completed 180/180 trials with equal measured accuracy, full hermetic crash recovery, and zero protected violations. The candidate used 37.11% fewer tokens, 33.84% lower estimated endpoint cost, and 11.63% fewer steps; this does not establish improved quality, latency, or production behavior. Fourth, deployed source/configuration evidence shows bounded reflection, recall accounting, memory compilation, and tool-health paths, but no production outcome lift. Praxa's supported contribution is an evidence-bound architecture that makes authority-to-effect transitions explicit and testable. Current evidence does not establish adversarial security, production safety, general specialist superiority, autonomous recursive optimization, or user benefit.

---

## 303. JarvisHub: An Open Harness for Canvas-Native Multimodal Creative Agents

**Autori:** Yunlong Lin, Zixu Lin, Zhaohu Xing, Biqiang Li, Chenxin Li, Haonan Wang, Haitao Wu, Hengyu Liu, Jianghai Chen, Kaituo Feng, Kaixin Li, Shawn Chen, Shijue Huang, Sixiang Chen, Tsung-Yi Ho, Wenxuan Huang, Xiangyan Liu, Xiaomeng Hu, Xuanhua He, Yan Sun, Yunqing Zhao, Zhiqin Yang, Zehan Wang, Zhengyang Tang, Tianyu Pang, Xiangyu Yue  
**Data:** 2026-07-26  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2607.23588v1

> Creative AI is moving from single-step asset generation toward long-horizon multimodal production. Although recent generative models can synthesize high-quality images, videos, audio clips, UI elements, storyboards, slides, and other creative assets, real-world creative work requires more than isolated prompt-output interactions. It involves references, drafts, alternatives, edits, failed attempts, version relations, tool actions, evaluation signals, and human feedback, which together form an evolving project state. Existing prompt-based, chat-based, and node-based generation systems only partially support this state, as they often discard intermediate context, rely on linear conversations, or require manually specified workflows. Recent commercial systems indicate a shift toward agent-assisted creative production, but their closed architectures make it difficult to study how agents represent context, choose tools, revise artifacts, recover from failures, and maintain consistency over time. To address this gap, we introduce JarvisHub, a canvas-native creative agent harness for long-horizon multimodal creation. JarvisHub treats an editable canvas as the user workspace, the agent's external memory, action space, and shared project state, representing multimodal artifacts, dependencies, versions, and feedback as typed canvas nodes and links. Through a three-layer architecture of canvas state, protocol bridge, and agent runtime, JarvisHub enables agents to act within an inspectable and editable creative state. This design moves creative agents beyond isolated tool use toward sustained, human-steerable creative automation, where agents can progressively plan, generate, revise, and organize multimodal projects while users remain able to inspect, guide, and intervene throughout the process.

---

## 304. StateAct: Program State, before Pixels, for Long-Horizon Computer-Use Agents

**Autori:** Yan Yang, Xiangru Jian, Ziyang Luo, Zirui Zhao, Yutong Dai, Ziji Shi, Hanshu Yan, Jun Hao Liew, Silvio Savarese, Junnan Li  
**Data:** 2026-07-24  
**Categorie:** cs.SE, cs.CV  
**Link:** https://arxiv.org/abs/2607.22798v1

> Computer-use agents are usually improved by strengthening perception: better models for reading a screenshot and choosing where to click. Yet a screenshot is only a lossy rendering of the underlying program state, e.g., the files, application backends, and DOM that hold the task data. Different states can produce the same pixels, while code can inspect and modify that state directly. StateAct is a code-first, multi-agent harness built around this distinction. Its main agent works directly with program state by using code, while a dedicated GUI subagent handles screenshot-and-click interaction on the few subgoals that need it, just 28 of 108 tasks and 1.1% of main-agent steps. The same direct access to program state also supports verification: an independent finish gate double-checks the saved result for structural failures, e.g., output that is missing, unsaved, or written to the wrong path. To stay on track over hundreds of steps, the main agent hands subgoals to fresh subagents, keeping its own context focused. On OSWorld 2.0, StateAct lifts Claude Opus 4.8 from 20.6% to 26.9% on binary success, and from 54.8% to 61.6% on partial success, at ~ 9x lower cost per task than the same model driven by screenshots alone; a code-only variant with no GUI subagent reaches only 45.9% partial, below that screenshot-based baseline's 54.8%. In general, grounding action, verification, and memory in state, what we call state-grounding, shifts the main bottleneck from perception toward reasoning: failures depend more on what the agent thinks than on what it sees.

---

## 305. Tencent WorkBuddy Bench: A Multi-Domain Coding-Agent Benchmark with Contamination-Resistant Task Construction

**Autori:** Tencent WorkBuddy Bench Team, Siqi Cai, Shaopeng Chen, Xiang Fei, Yong Mao, Zihan Xu, Zhiheng Lyu, Zhijian Shao, Yuchen Shi, Shuwen Zhang, Chaofan Qiu, Linjie Che, Xiaoxi Zhao, Feng Wu, Kai Zhang, Chaofan Zhu, Yubin Qi, Xiaoyun Liang, Peijie Dong, Yunhao Zhang, Yuanjie Zhu, Ling Jiang, Xianjun Zhang, Zhehang Chu, Anyuan Sang, Zhen Feng, Sen Nie, Shi Wu, Yuanzhen Xu, Xin Li, Ning Yang, Zhiqiang Dong, Hande Dong, Qiang Lin, Yi Liu, Yunsheng Wu, Ke Li, Xing Sun  
**Data:** 2026-07-23  
**Categorie:** cs.CL, cs.SE  
**Link:** https://arxiv.org/abs/2607.20911v1

> We introduce Tencent WorkBuddy Bench, a multi-domain evaluation suite for coding agents; this report documents its construction methodology, scoring protocol, and a cross-model leaderboard. At its core is a unified evaluation framework for constructing and running distribution-informed coding-agent tasks across four work domains - Code, Web, Office, and Security. Rather than adapting public issue text, every task is reverse-engineered from a real commit, pull request, or business scenario and rewritten as a short, colloquial, role-played request, so that a task's prompt is not recoverable by web-searching the underlying issue, pull request, or commit thread. Because the dataset is released openly - task directories, environment images, evaluation harness, tests, and reference solutions - contamination resistance rests on this construction together with dataset versioning rather than on secrecy. The four subsets - repository-level engineering, front-end development, office and business workflows, and red-/blue-team security - probe complementary facets of real work, each with its own verification style. All are packaged in a uniform task-directory format and run, under a uniform and reproducible protocol, on two agent harnesses (CodeBuddy Code and Claude Code); the full open release makes the benchmark reproducible end to end and directly auditable, since any third party can re-run each task and inspect its content. Because each subset uses a different scoring instrument, scores are not comparable across subsets and the suite reports no suite-wide average. We report a cross-model leaderboard across several model families.

---

## 306. PRO-LONG: Programmatic Memory Enables Long-Horizon Reasoning

**Autori:** Alexis Fox, Junlin Wang, Paul Rosu, Bhuwan Dhingra  
**Data:** 2026-07-22  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2607.20064v3

> Long-horizon tasks require sustained perception, reasoning, and exploration, and are a persistent challenge for large language model (LLM) agents. This gap is reflected in their limited performance on continual learning benchmarks such as ARC-AGI-3 and NetHack, especially when evaluated without specialized harnesses. Various agent harnesses have been proposed to close the gap, and each commits to a strategy for handling long sequences of observations, i.e., what information to save from the environment and how to load it into model context, a choice we argue is particularly consequential. Existing methods for context management have typically been designed around a tradeoff, where preserving more information makes relevant details harder to retrieve. Recent progress in coding agents, however, makes new approaches to memory viable. We propose PRO-LONG, a minimal context management framework built around programmatic memory for LLM agents in long-horizon, exploratory settings. PRO-LONG addresses the tradeoff by keeping a complete, structured interaction log and using programmatic tools to search this history efficiently. On NetHack, we find increasing gains from using PRO-LONG for cross-episodic memory, with scores reaching up to 2.2x those of a base coding agent. On the full ARC-AGI-3 public game set, PRO-LONG improves over this baseline agent by an average of 18.0 percentage points across frontier models, and matches or exceeds state-of-the-art specialized harnesses (up to 97.4% best@2) while using 4.2-5.8x fewer tokens. Relevant code and logs are available at https://github.com/alexisfox7/PRO-LONG.

---

## 307. DocOps: A Verifiable Benchmark for Autonomous Agents in Complex Document Operations

**Autori:** Jiazhen Jiang, Boxi Cao, Lingyong Yan, Yaojie Lu, Hongyu Lin, Shuaiqiang Wang, Dawei Yin, Xianpei Han, Le Sun  
**Data:** 2026-07-22  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2607.19865v1

> As autonomous agents rapidly evolve, their ability to reliably manipulate ubiquitous digital documents has become critical for enabling general-purpose AI assistants and automating complex workspace workflows. In this paper, we introduce DocOps, a deterministically verifiable evaluation framework underpinned by a hierarchical taxonomy that deconstructs document operations inspired by real-world practices into atomic dimensions and escalating workflow complexities. Based on DocOps, we systematically evaluate representative closed- and open-source models across various agentic harnesses, revealing that even the most advanced frontier configurations still exhibit profound limitations when handling highly coupled, long-range tasks. Furthermore, a fine-grained analysis of existing agents' manipulation behaviors uncovers 3 key failure modes: long-term state tracking collapse, shallow semantic verification, and destructive editing of structural metadata. Ultimately, our work exposes the capability boundaries of agents in maintaining global document consistency, shedding light on the future design of robust, non-destructive agents for complex digital ecosystems.

---

## 308. FlashRT: Agent Harness for Guiding Agents to Deploy Real-Time Multimodal Applications

**Autori:** Krish Agarwal, Zhuoming Chen, Yanyuan Qin, Zhenyu Gu, Atri Rudra, Beidi Chen  
**Data:** 2026-07-20  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2607.18171v2

> Real-time multimodal applications, including voice agents and interactive video generation, compose heterogeneous models into pipelines whose efficient deployment requires application-specific decisions about placement, streaming, and intra-model parallelism. Existing serving systems and auto-parallelism compilers commit to limited transformations and fixed workload assumptions, so achieving high performance on a new application requires hand-crafting an efficient implementation. We present FlashRT, an agent harness that guides coding agents to lift simple developer-written reference implementations into optimized multi-GPU deployments that flexibly weigh target metrics like latency and throughput. Using a new chain-of-program paradigm, FlashRT directs a generic coding agent through a multi-pass transformation process where an agent transforms the reference into an intermediate representation (IR) to capture data dependencies and persistent-state scopes, validates this IR via a sequential interpreter, and performs static analyses to identify candidate transformations. Then, the agent iteratively implements, verifies, and benchmarks each candidate under a measurement-gated optimization loop to produce effective deployments that span different hardware budgets. Across various applications, including video world models and multimodal LLMs, FlashRT converts reference implementations into highly efficient deployments, delivering up to ~70x latency reduction and 2.8x throughput improvement on NVIDIA B200 GPUs. On AMD MI355X GPUs, FlashRT matches the peak latency reduction while increasing peak throughput improvement to 3.6x, demonstrating that agent-driven optimization can be more scalable on platforms with less mature expert optimization. In fact, for Qwen3-Omni text-to-audio inference, FlashRT reduces response latency by 65% compared to the expert vLLM-Omni implementation on AMD MI355X.

---

## 309. Is Progressive Disclosure All You Need for Long-Context Agents?

**Autori:** Yifeng He, Yinzhe Zhao, Jicheng Wang, Hao Chen  
**Data:** 2026-07-20  
**Categorie:** cs.AI, cs.CL, cs.SE  
**Link:** https://arxiv.org/abs/2607.17598v1

> Long-document question answering usually forces a choice between loading the whole document into the context window and bolting on a separate retriever. Agentic AI suggests a broader option, giving the agent the document path and letting it decide how and what to read. Agent Skills, a standard for packaging expertise into folders an agent loads on demand, supply a ready mechanism: progressive disclosure, which exposes only what a query needs, from a short description down to the specific passages. Practitioners rapidly adopted this pattern for book-length understanding tasks, but the evidence to support such choices has been anecdotal. We run the first controlled study of the pattern, comparing raw-document navigation and several designs of Agent Skills packs against a classical hybrid retriever across three agent harnesses and three model families on InfiniteBench. On a single book, the gain depends on the harness, running large when the agent navigates the raw document poorly but near zero when a strong agent harness already divides and retrieves on its own. When scaling up to tasks that span many books, raw-document navigation collapses while one-level progressive disclosure degrades more slowly and pulls ahead. A second, deeper routing level never helps and sometimes breaks accuracy outright, so one level is enough. Progressive disclosure buys context, not intelligence: it is redundant while a strong agent can locate the right passages itself, and decisive once the corpus grows too large to navigate by reading.

---

## 310. CLOSER-Bench: Evaluating Budgeted Cross-Stage Design Closure for Hardware Agents

**Autori:** Peilong Zhou, Zhirong Chen, Cangyuan Li, Haoyu Gao, Kaiyan Chang, Ziming Qu, Ying Wang  
**Data:** 2026-07-18  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2607.16632v1

> Hardware engineering exposes coding agents to a form of long-horizon work that is difficult to capture with pass-at-k: progress is continuous, tool feedback is delayed and heterogeneous, and a backend failure may require revising RTL rather than tuning another physical-design parameter. Existing benchmarks measure RTL generation, repository repair, verification, PPA evolution, or physical implementation, but their different designs and oracles make it hard to determine where an agent succeeds or fails across abstraction boundaries. We introduce CLOSER-Bench, a controlled evaluation protocol for budgeted cross-stage design closure. For one design and one hidden objective, it pairs spec-to-RTL, RTL-to-GDS, and spec-to-GDS tasks, records every simulator, synthesis, STA, and place-and-route invocation, and measures final quality, anytime progress, tool cost, and cross-stage recovery. The benchmark is built on open-source Verilator, Yosys, OpenROAD, KLayout, Sky130, and the Harbor agent harness. A ten-task pilot spanning RTL repair, mutation-based verification, coverage, PPA optimization, design-space exploration, cross-model debugging, and security establishes the executable harness and exposes a sharp completion--closure gap: three agents solve a localized AXI repair task, while the matched verification-closure task separates a frontier agent from two otherwise successful baselines. We further validate a full RTL-to-GDS flow and construct a macro-based AXI/DMA streaming accelerator for the stage-paired evaluation. These results motivate treating hardware closure as a budgeted sequential decision problem rather than a collection of independent code generation tasks.

---

## 311. Co-Harness: Co-Evolving Harnesses and Model Weights for LLM Agents

**Autori:** Zhengyu Chen, Teng Xiao, Huaisheng Zhu, Yige Yuan, Luan Zhang, Jingang Wang  
**Data:** 2026-07-17  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2607.22688v1

> Post-training agents for automated AI research requires optimizing not only model parameters, but also the runtime harness that shapes how research trajectories are generated, evaluated, and learned from. Existing pipelines typically train models under a fixed harness, including prompts, tools, skills, middleware, and memory, while leaving the data-generating process outside the optimization objective. This creates a mismatch between model updates and the static scaffolding that determines trajectory quality. We introduce Co-Harness, a framework that jointly optimizes the agent harness and model parameters during post-training. Co-Harness alternates between harness optimization and model optimization. An LLM-based HarnessCritic analyzes failed trajectories, identifies harness-level failure modes, and proposes validated local updates. The model is then fine-tuned on high-quality trajectories generated by the improved harness, distilling effective scaffolding into model parameters. A 200+ hour autonomous case study further shows that Co-Harness can recover from system crashes, improve inference efficiency, and discover ensemble strategies without human intervention. These results suggest that joint harness and model optimization is an effective way to improve agents beyond fixed-harness post-training.

---

## 312. Copy-on-Write Scoring: Application-Specific Agent Evaluations

**Autori:** Joanna Roy, Sven Hoelzel  
**Data:** 2026-07-15  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2607.14336v1

> Trustworthy deployment of LLM-based agents in software systems requires evaluating how they perform on application-specific workflows, with enough granularity to localize where they succeed and fail. Yet existing agent evaluation mechanisms are limited: benchmarks have low construct validity for application-specific workflows and environments, and replica evaluation environments are expensive and prone to drift. We propose Copy-on-Write (CoW) Scoring, a framework that evaluates agent operations directly within application environments using a PostgreSQL-level Copy-on-Write mechanism to isolate agent writes. CoW Scoring produces session- and operation-level scores that highlight where agents' database write operations succeed and fail in a given application environment, enabling inexpensive evaluation and iteration on agent harnesses and tool surfaces. We demonstrate the framework on Plane, an open-source project-management platform, where analysis surfaced specific issues in the tool surface, and corresponding fixes produced measurable improvements on affected models. Python library: https://github.com/trail-ml/agent-cow-python

---

## 313. Do Agent Optimizers Compound? A Continual-Learning Evaluation on Terminal-Bench 2.0

**Autori:** Wenxiao Wang, Priyatham Kattakinda, Soheil Feizi  
**Data:** 2026-07-15  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2607.14004v1

> Most reported gains from agent-optimization methods are one-shot: an agent is optimized against a fixed benchmark and the resulting improvement is reported as if it were a stable property of the method. This does not test the setting that matters for deployed agents, where optimization is applied recursively as new failures and new tasks appear over time. The central question this raises is whether optimizer-driven gains compound: after an agent has been optimized once, can it be optimized again on newly arrived tasks without eroding the gains the first round produced? We study this question with a two-phase continual-learning evaluation built from hard tasks in Terminal-Bench 2.0, comparing three approaches to agent-harness optimization (GEPA, Meta Harness, and RELAI's Verifiable Continual Learning, RELAI-VCL) under identical optimization budgets. All three methods improve over the baseline agent in the conventional, static, single-phase setting. However, once new tasks are introduced, the methods diverge sharply: GEPA's optimized agent transfers below the unoptimized baseline, Meta Harness transfers well but fails to improve further once given a second optimization budget, and RELAI-VCL is the only method that both transfers positively to unseen tasks and continues improving after those tasks are folded into the optimization objective, reaching the highest pass rate at every evaluated stage and the highest lifelong average pass rate overall (76.4% vs. 66.0% for GEPA, 64.6% for Meta Harness, and 58.7% for the baseline). Our key observation was that optimization gains compounded only when regression control was built into the optimization loop, providing an inductive bias against shortcut solutions that fail to generalize.

---

## 314. HarnessBank: Semantic Gene-Bank Search with Gated Verification for Agent-Harness Self-Evolution

**Autori:** Xiaotian Luo, Dizhan Xue, Fengxingyu Wang, Chuanrui Hu, Yafeng Deng  
**Data:** 2026-07-15  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2607.13683v2

> Large Language Models (LLMs) have enabled capable agents across diverse applications. Beyond the foundation model, the performance of an agent is governed by the surrounding agent harness, including prompts, tools, control loops, etc. Automatically evolving this harness offers a promising pathway to agent improvement, yet existing approaches typically rely on greedy candidate selection and noisy self-generated feedback, rendering their gains susceptible to search collapse, task-specific overfitting, and poor verifiability. To tackle these challenges, we introduce HarnessBank, a trustworthy agent-harness self-evolution framework that pairs a task agent with a separate evolver agent for iterative failure diagnosis, harness generation, and evolution verification. HarnessBank maintains a Harness Gene Bank composed of high-performing harnesses of different semantic coordinates. Those harnesses are reinvented, recombined, screened, and selected during the self-evolution procedure. Moreover, we propose a Gated Harness Screening mechanism to efficiently filter high-quality harnesses and reduce the cost of evaluating numerous offspring harnesses. Across seven agent benchmarks, HarnessBank produces consistent performance improvements from 5.1% to 15.4%. Cross-model experiments further verify that the improvements come from the model-specific self-evolving process, instead of a universally optimal harness. Our code will be publicly available upon acceptance.

---

## 315. Harness Handbook: Making Evolving Agent Harnesses Readable,Navigable, and Editable

**Autori:** Ruhan Wang, Yucheng Shi, Zongxia Li, Zhongzhi Li, Yue Yu, Junyao Yang, Kishan Panaganti, Haitao Mi, Dongruo Zhou, Leoweiliang  
**Data:** 2026-07-14  
**Categorie:** cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2607.13285v1

> The capability of a modern AI agent depends not only on its foundation model but also on its harness, which constructs prompts, manages state, invokes tools, and coordinates execution. As models, APIs, environments, and requirements evolve, the harness must be continually modified. Before such a change can be made, a developer or coding agent must identify all code locations that implement the target behavior. This is difficult because production harnesses are large, tightly coupled, and behaviorally distributed, while modification requests describe what the system should do and repositories are organized by files and modules. Code search, repository indexing, and long-context processing ease inspection, but still leave this behavior-to-code mapping to be recovered by hand. Behavior localization is therefore a central bottleneck in harness evolution. We introduce the Harness Handbook, a behavior-centric representation synthesized automatically from a harness codebase via static analysis and LLM-assisted structuring, linking each behavior to its corresponding source. We also introduce Behavior-Guided Progressive Disclosure (BGPD), which guides agents from high-level behaviors to relevant implementation details and verifies candidate locations against the current source. On diverse modification requests from two open-source harnesses, Handbook-Assisted planning improves behavior localization and edit-plan quality while using fewer planner tokens, with the largest gains on scattered sites, rarely executed paths, and cross-module interactions. Evolving complex agentic systems thus depends not only on generating edits, but also on determining where those edits should be made.

---

## 316. MemoHarness: Agent Harnesses That Learn from Experience

**Autori:** Yue Huang, Wenjie Wang, Han Bao, Yuchen Ma, Xiaonan Luo, Yi Nian, Haomin Zhuang, Zheyuan Liu, Yue Zhao, Xiangliang Zhang  
**Data:** 2026-07-14  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2607.14159v1

> An agent harness is the external control layer that turns a base LLM into an executable agent by managing context, tools, orchestration, memory, decoding, and output handling. While harness design strongly affects agent behavior, most automatic improvement methods optimize narrower artifacts such as prompts, pipelines, or workflows, and deployed agents usually reuse a single global harness for all cases. We introduce MemoHarness, an adaptive harness optimization framework that learns from its own executions. MemoHarness decomposes the harness into six editable control dimensions, stores per-case diagnoses and distilled global patterns in a dual-layer experience bank, and adapts the learned harness to each test case using retrieved experience without test-time labels, feedback, or additional search. In our evaluation across shell-agent, code-generation, and analytical-reasoning benchmarks, MemoHarness improves over the fixed harnesses we compare against and shows selective transfer to unseen suites and base models. Its additional context can also remain cost-competitive when much of the retrieved experience is cacheable. These results provide evidence that execution experience is a practical substrate for building agent harnesses that are more adaptive than a single static configuration, while leaving broader claims about statistical robustness and component attribution to future work.

---

## 317. ToFu: A White-Box, Token-Efficient Agent Harness for Researchers

**Autori:** Junhao Ruan, Yuan Ge, Bei Li, Yongjing Yin, Yuchun Fan, Xin Chen, Jingang Wang, Chenglong Wang, Jingbo Zhu, Tong Xiao  
**Data:** 2026-07-13  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2607.11423v1

> Agentic coding tools present new opportunities to transform research workflows. The performance of agent systems built depends on both large language models (LLMs) and the harness around LLMs, which is the orchestration code that determines an agent's behavior. We present ToFu, an agentic harness for researchers that reads your codebase, edits files, runs commands, and integrates with your development tools. ToFu plays a dual role in research. As a research assistant, it supports practical research workflows with superior token efficiency, lower cost, and multilingual capability compared with existing agentic harnesses. Its release under the MIT License further enables local deployment for privacy-sensitive users. As a research object, ToFu provides a white-box agentic harness that allows researchers to inspect, modify, and evaluate its orchestration logic, tool-use behavior, and harness design, while retaining strong benchmark performance and an application-level user experience.

---

## 318. SETA: Scaling Environments for Terminal Agents

**Autori:** Qijia Shen, Zhiqi Huang, Vamsidhar Kamanuru, Aznaur Aliev, Jay Rainton, Ahmed Awelkair, Zhichen Zeng, Jiajun Li, Shi Dong, Yueming Yuan, Boyuan Ma, Qizheng Zhang, Jiwei Fu, Yuzhen Mao, Wendong Fan, Ping Nie, Philip Torr, Bernard Ghanem, Changran Hu, Jonathan Lingjie Li, Urmish Thakker, Guohao Li  
**Data:** 2026-07-12  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2607.10891v2

> Large language models (LLMs) are rapidly shifting toward agents that solve tasks through diverse interfaces, including web and graphical user interfaces (GUIs). Among these, the terminal command line provides a text-based, general-purpose interface, covering tasks from system operations to data science and machine learning. However, scaling terminal-agent training remains challenging, as it requires diverse and coherent task instructions, executable environments, and reliable verification, while lacking naturally grounded supervision data. In this work, we propose SETA, a scalable framework for generating verifiable terminal environments for reinforcement learning (RL). The framework consists of two pipelines sharing a unified verification mechanism: SETA-Synth converts diverse sources into standardized RL environments, and SETA-Evol further expands from existing environments with adaptive control of difficulty and diversity. Together, we construct and release SETA-Env, the largest open-source verifiable terminal RL dataset to date, containing over 4,500 environments. We evaluate our dataset by training Qwen3-8B with GRPO on SETA-Env, achieving 12% pass rate on Terminal-Bench 2.0, the best reported result for an RL-trained model at the 8B scale. We further observe gains on DeepSeek-V4-Flash under the same terminal agent harness, with pass@1 on Terminal-Bench 2.0 improving from 40% to 43% and pass@5 improving from 54% to 58%. These results demonstrate that SETA- Env provides high-quality training environments for terminal agents and serves as a valuable resource for advancing research on terminal-based agent learning.

---

## 319. AgentAbstain: Do LLM Agents Know When Not to Act?

**Autori:** Xun Liu, Yi Evie Zhang, Vira Kasprova, Parisa Rabbani, Pardis Sadat Zahraei, Tianyu Zhang, Ali Ebrahimpour-Boroojeny, Varun Chandrasekaran  
**Data:** 2026-07-11  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2607.10059v1

> Agent systems based on large language models (LLMs) are increasingly deployed for autonomous tasks, yet existing evaluations mostly focus on task success rather than whether agents know when to abstain. This gap poses real risks: under ambiguity, conflicting constraints, or tool failures, agents may execute unintended and irreversible actions. To close this gap, we present the first systematic evaluation framework for agentic abstention: the calibrated ability of tool-using LLM agents to recognize when not to act. At its core, AgentAbstain is a paired-task benchmark built on an agent-native taxonomy of 8 abstention scenarios across pre-execution reasoning and runtime discovery. It contains 263 paired tasks across 42 executable sandbox environments, where each pair consists of a should-act task and a should-abstain variant produced through a controlled perturbation to the instruction, tool, or environment state. To scale this paired design and resist data contamination, we propose AbstainGen, a fully automated pipeline that synthesizes sandbox environments and generates paired tasks end-to-end, validated by deterministic replay and semantic LLM judges; fresh task instances can be regenerated on demand, and three independent annotators rate 94-98% of sampled tasks as well-designed. Across 17 frontier LLMs in 4 agent harnesses, the best agent (Gemini 3.1 Pro) achieves only 59.5% paired accuracy (correct on both the act and abstain sides of each paired task). More importantly, abstention capability is largely independent of general task-solving capability, indicating that scaling task-solving alone will not close this gap. We further identify failure modes such as post-hoc abstention, in which agents execute irreversible actions before recognizing abstention triggers. Our code and dataset are open-sourced at agentabstain.github.io.

---

## 320. SimpleWikiSearch: A Clean Offline Wikipedia Environment for Agentic Search

**Autori:** Guanming Xiong, Penghui Zhang  
**Data:** 2026-07-10  
**Categorie:** cs.IR, cs.AI  
**Link:** https://arxiv.org/abs/2607.26070v1

> Large language model (LLM)-based agentic search systems are often evaluated as if the underlying LLM were the only component that matters, yet their measured performance also depends on the surrounding search environment: the Wikipedia snapshot, preprocessing pipeline, chunking policy, retrieval backend, tool schema, observation format, and answer submission rule. These details are frequently under-specified, making it difficult to compare results or reproduce reported baselines. We present SimpleWikiSearch, whose corpus construction, retrieval stack, tool contract, and evaluation protocol are explicit and runnable. The environment starts from a full English Wikipedia dump, cleans and chunks the corpus, builds keyword and dense retrieval indexes, and exposes a minimal tool interface consisting of \texttt{search}, \texttt{open\_url}, and \texttt{submit\_answer}. We report baseline results on six QA datasets using open-source LLMs and provide a random-300 subset for comparisons with closed-source commercial models. SimpleWikiSearch provides a domain-specific agent harness and a controlled offline environment for reproducible agentic-search evaluation. Its contribution is this specified reference setup, rather than a new agent algorithm. Code and data will be available at: https://github.com/JimXiongGM/simple_wiki_search.

---

## 321. Toward Auditable AI Scientists: A Hypothesis Evolution Protocol for LLM Agents

**Autori:** Izumi Takahara, Teruyasu Mizoguchi  
**Data:** 2026-07-10  
**Categorie:** cs.AI, cond-mat.mtrl-sci  
**Link:** https://arxiv.org/abs/2607.09195v1

> Large language model (LLM) agents are increasingly expected to play a central role in AI-driven scientific discovery. Equipped with broad knowledge, flexible reasoning, and tool use, they have the potential to autonomously explore and solve scientific problems by repeatedly proposing hypotheses, testing them, and revising their beliefs in the light of the evidence. In current agents, however, these hypotheses, tests, and belief updates are buried in unstructured logs, and no mechanism lets the agent or the human researcher audit that process. Here we propose the Hypothesis Evolution Protocol (HEP), an agent harness that provides hypothesis generation, evaluation, and evolution as explicit, auditable operations. On materials-science research tasks, a HEP-equipped agent operates the hypothesis--test--evidence--belief cycle that planning-style agents lack, generalizes across research questions, and exploits the protocol more fully as the base LLM becomes more capable. These results mark a step toward auditable AI scientists, whose scientific reasoning can be inspected, verified, and built upon.

---

## 322. Scoped Verification for Reliable Long-Horizon Agentic Context Evolution under Distribution Shift

**Autori:** Dan C. Hsu, Luke Lu  
**Data:** 2026-07-10  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2607.09175v2

> Deployed LLM agents rely on agentic context, the model-external textual control content assembled by an operational harness. In this work, the mutable component of that context is a persistent system-level instruction that is updated from operational experience while the model, tools, and harness remain fixed. Over long evolution horizons, flat-text maintenance makes verification increasingly difficult as accumulated instructions grow and interact. We propose Graph-Regularized Agentic Context Evolution (GRACE), which maintains the persistent instruction component as a typed semantic graph and validates proposed updates within the local typed neighborhoods of modified nodes. Accepted graph updates are reconstructed as incremental edits to the textual instruction checkpoint used at deployment. We evaluate GRACE within a fixed telecom agent harness derived from $τ^2$-bench under a controlled distribution-shift protocol. Across five independent replications, GRACE improves strict reliability, measured by pass^3, from the Gemini 2.5 Flash zero-shot value of 0.091 to 0.673$\pm$0.136 at the final checkpoint. This exceeds a Gemini 3.1 Pro zero-shot reference of 0.242 on the same held-out set, while the flat-text HCE baseline finishes at 0.191$\pm$0.051. These results identify two requirements for reliable long-horizon context evolution, a structural substrate that makes verification local and a consolidation mechanism that keeps accumulated instruction content usable.

---

## 323. Remember When It Matters: Proactive Memory Agent for Long-Horizon Agents

**Autori:** Yifan Wu, Lizhu Zhang, Yuhang Zhou, Mingyi Wang, Bo Peng, Serena Li, Xiangjun Fan, Zhuokai Zhao  
**Data:** 2026-07-09  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2607.08716v1

> In long-horizon tasks, decision-relevant state is often scattered across an expanding trajectory, while the action agent must surface it and act. As trajectories grow, task requirements, environment facts, prior attempts, diagnoses, and open subgoals can be buried in the context window or pushed beyond it, failing to influence decisions when needed. We call this failure mode "behavioral state decay". We study memory as an active intervention mechanism rather than passive retrieval. A separate memory agent runs alongside an unmodified action agent, updating a structured memory bank from the recent trajectory and deciding whether to inject a memory-grounded reminder or remain silent. The module is plug-and-play with frontier action agents and existing agent harnesses. Across Terminal-Bench 2.0 and $τ^2$-Bench, it improves pass@1 for both weaker and stronger action agents, with gains of +8.3 pp on Terminal-Bench and +6.8 pp on $τ^2$-Bench. Ablations show that selective intervention outperforms passive bank exposure, always-on injection, advisor-only guidance, and general retrieval. As an early step toward open-weight memory policies, we train Qwen3.5-27B on SETA using SFT and GRPO, improving validation reward and achieving partial transfer to Terminal-Bench.

---

## 324. Cognitive-structured Multimodal Agent for Multimodal Understanding, Generation, and Editing

**Autori:** Feng Wang, Canmiao Fu, Zhipeng Huang, Chen Li, Jing Lyu, Ge Li  
**Data:** 2026-07-09  
**Categorie:** cs.CV, cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2607.08497v1

> Recent unified multimodal models show a single architecture can jointly perform vision/language understanding and image generation/editing. However, they repeatedly feed all historical visual and textual inputs into a shared context window, limiting long-horizon multimodal dialogue due to visual token explosion and unreliable cross-turn referencing. We propose a Cognitive-structured Multimodal Agent that externalizes visual information into an Episodic Visual Memory and selectively reactivates relevant episodes during reasoning. The agent consists of a Perceptual Abstraction Engine for structured visual abstraction, a Cognitive Retrieval Engine for cross-turn memory retrieval, and a Multimodal Executive Controller for autonomous task inference and action planning. To address the lack of turn-level retrieval supervision in existing datasets, we develop a Unified Scenario Engine that programmatically generates structured multi-turn conversations with fine-grained retrieval annotations, enabling reinforcement learning to optimize abstraction and retrieval policies. We also construct a long-horizon visual-dialogue benchmark stratified by difficulty to evaluate episodic visual recall. Our 8B agent achieves 91.4% retrieval accuracy over 20-turn sessions, surpassing 32B baselines by +8.2% while nearly halving per-turn inference time (23.1s -> 12.7s). We further present the Cognitive-structured Multimodal Agent Harness (CMA-Harness), a tool-augmented deployment of the same cognitive structure integrating persistent multimodal memory, web access, image generation/editing/composition tools, and OpenAI-compatible serving. Structured memory and modular decision-making offer a more scalable, efficient paradigm for long-horizon multimodal agents than monolithic parameter scaling. Code: https://github.com/caseclose/cma-harness ; Project page: https://caseclose.github.io/cma-harness/

---

## 325. From Prompts to Contracts: Harness Engineering for Auditable Enterprise LLM Agents

**Autori:** Joongho Ahn, Moonsoo Kim  
**Data:** 2026-07-09  
**Categorie:** cs.AI, cs.CL, cs.SE  
**Link:** https://arxiv.org/abs/2607.08028v1

> Enterprise large language model (LLM) applications often begin as prototypes whose behavior is carried by prompts and retrieval context. Productization adds requirements for source boundaries, entity routing, answer contracts, and reproducible traces. We present a harness-engineering approach that reconstructs this pattern into a traceable, auditable LLM-agent architecture: deterministic behavior moves into code, manifests, schemas, and validation artifacts around a replaceable composition boundary, while source-backed claims remain the authority for runtime answers. We instantiate it on a public-data slice of five Korean corporate groups (25 listed companies) and evaluate three research questions. (1) The harness preserves its source-grounding, entity-routing, trace, output-hygiene, and recommendation-language contracts across the fixed validation scenarios; a fault-injection control confirms the validators flag deliberately broken contracts. (2) The checks the harness enforces held under model substitution: across three hosted models, they passed on all 270 composition-boundary runs; failures were confined to the model-composed side and were caught and recorded. (3) The code-owned guarantees are load-bearing, not reproducible by prompting alone: holding the model fixed and varying only the enforcement layer, prompt instructions alone let recommendation-language and internal-trace-leakage violations reach the reader, which the harness blocks entirely. A bolt-on external guardrail prevents such violations too but over-refuses, dropping utility to 88/120 where the harness preserves full utility (120/120); in this ablation, only code-owned enforcement preserves both safety and utility. The result is a reusable engineering pattern for turning exploratory prototypes into auditable applications with versioned source, control, and validation artifacts.

---

## 326. Infinite Worlds with Versatile Interactions

**Autori:** Zelin Gao, Qiuyu Wang, Jiapeng Zhu, Jingye Chen, Zichen Liu, Qingyan Bai, Jiahao Wang, Yufeng Yuan, Hanlin Wang, Yichong Lu, Ka Leong Cheng, Haojie Zhang, Jian Gao, Tianrui Feng, Yuzheng Liu, Yao Yao, Yinghao Xu, Xing Zhu, Yujun Shen, Hao Ouyang  
**Data:** 2026-07-08  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2607.07534v1

> We present LingBot-World 2.0 (also known as LingBot-World-Infinity), an advanced iteration of LingBot-World featuring four distinct upgrades. (1) Our model achieves an unbounded interaction horizon while maintaining consistent output quality, benefiting from a carefully crafted causal pretraining paradigm. (2) Through distilling a real-time variant from the base model, our system guarantees rapid response time, sufficient to drive 720p video streams at 60 fps. (3) Compared to the previous version, this update introduces highly diverse interactive elements, comprising a broader spectrum of actions (e.g., attacking, archery, spell-casting, and shooting) alongside a richer variety of text-driven events. (4) We pioneer the integration of an agentic harness within the domain of world modeling, wherein a pilot agent is tasked with planning and executing character behaviors, while a director agent is responsible for synthesizing novel environmental elements as the scene progresses. Additionally, to facilitate a shared experience, we develop an interface that permits multiple players to simultaneously immerse themselves in this vivid world simulator. We pair our primary 14B model with a lightweight 1.3B counterpart, which supports effortless deployment on a single GPU.

---

## 327. The Harness Effect: How Orchestration Design Sets the Token Economics of Enterprise Agentic AI

**Autori:** Muayad Sayed Ali, Aliaksandra Novik, Anji Boddupally, Artem Yavorskyi, Chris Nickerson, Daniel Rica, Emily DuGranrut, Felix Leung, Garrett Prince, Grace Barnett, Heath Robinson, Hosain Al Ahmad, Jesse Resnick, Jyothi Swaroop Meruga, Leonid Kuznetsov, Luke Gorham, Marie Schmoll, Michael Paciullo, Saumya Das, Sharath Sheripally, Tommy Griscom, Mykyta Osadchyi, Neha Mantri, Nick Westrum, Olivia Benowitz, Parikshith Kulkarni, Radik Chernyshov, Rakshith Vasudev, Rohith Nadimpally, Vikas Gangadevi, Waseem AlShikh  
**Data:** 2026-07-08  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2607.06906v2

> Agentic AI development today runs on token maxing: buying capability with tokens -- longer reasoning traces, more turns, wider tool payloads, bigger replayed contexts -- so tokens per task grow faster than task value. Falling per-token prices mask the pattern; total spend rises anyway. We argue the decisive lever against token maxing is the harness: the orchestration layer that assembles context, exposes tools, sequences turns, delegates work, and carries enterprise observability and governance. We isolate it with a controlled swap: 22 locked evaluation tasks, six foundation models (Claude Sonnet 4.6, Gemini 3.1, Gemini Flash 3.5, Qwen 3.6, GLM 5.1, Palmyra X6), changing only the orchestration layer -- a frozen conventional production loop versus the Writer Agent Harness. Holding models constant, the harness cuts blended cost per task 41% ($0.21->$0.12), median wall-clock 44% (48s->27s), and tokens per task 38% (14.2k->8.8k), with task-completion quality at parity (0.78->0.81, directional at this sample size). Efficiency is model-invariant -- every model gets cheaper (33-61%) -- while quality gains are capability-dependent: a model's gain correlates almost perfectly with its baseline strength (r=0.99, n=6), a phenomenon we term harness leverage. Quality per dollar rises 82%; task-completions per million tokens rise from 54.9 to 92.0. On this workload the orchestration layer moved cost per task more than the full spread of the model menu did. We formalize token economics at the orchestration layer (including effective input price under prompt caching), detail the six mechanism families behind the effect -- cache-shape discipline to failure-spend governance -- compare six widely used agent systems on the same axes, and argue the harness is the one component whose efficiency multiplies across every model an organization runs -- present and future.

---

## 328. Cost-Effective Agent Harnesses for Abstract Reasoning and Generalization on ARC-AGI-1

**Autori:** Kabir Moghe, Peter Chin  
**Data:** 2026-07-07  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2607.06764v1

> Recent progress on ARC-AGI-1 from disclosed architectures has come broadly from two regimes: heavy test-time compute over frontier models (evolutionary search, exhaustive sampling, extended chain-of-thought), or benchmark-specific training in which small models are fine-tuned on ARC data, often with task-specialized architectures. We study a third regime: an open-weight model in non-thinking mode (DeepSeek V3.2) under a strict budget, with no ARC-specific fine-tuning. We study what is recoverable through architecture alone, building agentic harnesses that decompose pattern-discovery and program-synthesis stages explicitly. First, we introduce an Explorer-Definer Pipeline that separates pattern discovery from executable transformation synthesis, implemented as a two-stage agent pipeline. Next, we present the Reflective Orchestrator, which augments the pipeline with autonomous exploration of new transformations when previous hypotheses fail on training pairs. On the ARC-AGI-1 public 400-task evaluation set, the pipeline reaches 57.50% pass@2 at \$0.25 per task, and the orchestrator reaches 67.25% pass@2 at \$0.62 per task. Together these architectures lift a 15.50% one-shot baseline by ~52 points without benchmark-specific training or heavy test-time compute. Furthermore, the orchestrator-driven lift tests a falsifiable diagnostic the pipeline produces; unbiased pass@k analysis suggests the pipeline is generation-bound, not selection-bound (selection via training-pair accuracy captures ~95% of the candidate ceiling) and predicts that significant improvement requires broader generation, not better ranking. The orchestrator implements this prediction via adaptive re-exploration and confirms it (unbiased pass@1 lift +9.81 pp, matching selection-mediated pass@2 lift). An additional pipeline ablation identifies its think tool as a significant component, with removal reducing pass@2 by 5.75 pp.

---

## 329. The Balkanization of Execution-Security Research for AI Coding Agents: Isolation, Access Control, and Time-of-Check-to-Time-of-Use Vulnerabilities

**Autori:** Mohammadreza Rashidi  
**Data:** 2026-07-07  
**Categorie:** cs.CR, cs.AI  
**Link:** https://arxiv.org/abs/2607.05743v1

> AI coding agents now read repositories, call tools, and execute shell commands with limited human oversight, and a fast-growing body of work studies whether the execution layer around them is actually safe. That literature is scattered. Papers on sandbox isolation, capability and access control, policy enforcement, time-of-check-to-time-of-use (TOCTOU) races, Model Context Protocol (MCP) threats, identity delegation, execution provenance, network egress control, and static analysis of agent-generated code are published independently and rarely cite one another. We systematize 39 papers published between 2023 and 2026 into 17 categories, each verified directly against its source. The same verification protocol also confirms four disclosed, patched CVEs directly affecting production agent harnesses. Reading across categories surfaces five cross-cutting gaps that no single paper addresses. (1) Isolation architectures and capability models are almost never evaluated against one another on a shared benchmark. (2) Policy-enforcement studies report failure rates from 69% to 98% of real denylists, yet no isolation paper re-evaluates its own defense under that adversarial setting. (3) TOCTOU and MCP threats are analyzed as separate literatures despite both being instances of the same state-validation problem. (4) Every enforcement mechanism assumes an honest policy author, leaving policy-authoring error itself unaddressed. (5) Benign but out-of-scope agent actions occurring at rates up to 17.1% under realistic prompting are addressed by no access-control or capability paper in the corpus. Existing broader surveys of agentic AI security discuss sandboxing only as one item among many defenses, leaving execution security without a dedicated systematization. This paper is written to fill that gap. We conclude with a research agenda directed at the five gaps.

---

## 330. AgenticPD: A Stage-Aware Agentic Framework for Closed-Loop Physical Design Optimization

**Autori:** Shuo Ren, Zijin Cheng, Yaohui Han, Libo Shen, Leilei Jin, Wanting Tian, Rongliang Fu, Chao Wang, Bei Yu, Tsung-Yi Ho  
**Data:** 2026-07-06  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2607.04758v3

> Physical design quality-of-results (QoR) optimization is hard and expensive. Choices made at one stage can help or hurt later stages. Each evaluation requires a costly EDA run through the full flow. While existing methods still treat optimization as flat parameter tuning or a LLM-based script generation task, we present AgenticPD, a stage-aware agentic framework for physical design QoR optimization. Instead of re-running the full flow after every trial, AgenticPD is organized around the stage boundaries of the physical design flow, where a Judge Agent navigates the search and stage-specialized agents make local decisions within their own stage using stage-local tools. Additionally, the agent harness in AgenticPD provides structured observations, execution history, and agent context management. Experimental results show that AgenticPD achieves the best timing performance among the evaluated PD tuners while maintaining competitive power and area.

---

## 331. HarnessMDP: Learning to Control LLM Agent Harnesses with Offline Reinforcement Learning

**Autori:** Haiwen Yi, Xinyuan Song  
**Data:** 2026-07-05  
**Categorie:** cs.LG, cs.AI  
**Link:** https://arxiv.org/abs/2607.05458v3

> The execution harness is a critical component of LLM agents, shaping how the agent interacts with its environment and organizes multi-step execution. Prior work has shown that improving tools, workflows, and other harness components can substantially improve agent performance. This suggests that the harness can be treated as a learnable control layer that adapts execution decisions from experience, rather than as a predetermined execution configuration. In this work, we introduce HarnessMDP, a learning-based framework that makes harness control itself learnable. HarnessMDP formulates agent execution as a finite-horizon Markov decision process, where the harness learns to select structural execution actions from the evolving agent state. The harness policy is learned offline from collected trajectories using task performance and deployed online to adaptively control new executions. Extensive experiments on coding tasks, $τ$-bench, AgentBench, and other agent evaluation settings show that HarnessMDP consistently improves execution behavior and final task performance over baseline harnesses. These results demonstrate the effectiveness of HarnessMDP and establish learnable harness control as a practical mechanism for improving LLM agents through better execution. Our code is available at https://github.com/Hik289/Agentic-RL-harness.git.

---

## 332. ACE: Agentic Control for Embodied Manipulation via Zero-shot Workflow Reasoning

**Autori:** Iok Tong Lei, QianZhi Li, Ying Jie Yap, Yujie Zhang, Rui Zhong, Haichao Gui, Xiaolong Liu, Zhidong Deng  
**Data:** 2026-07-05  
**Categorie:** cs.RO, cs.LG  
**Link:** https://arxiv.org/abs/2607.04162v2

> General-purpose manipulation requires both semantic reasoning over task constraints and reliable execution of contact-rich actions. We present ACE, an agentic manipulation harness that composes a high-level language agent with a reusable mask-conditioned visuomotor policy. Given an open-ended instruction, the agent solves semantic constraints, binds objects to destination roles, and decomposes the task into executable transfers represented by tracked pick-and-place masks. Execution feedback supports outcome assessment, re-grounding, and retry, while persistent object and task context preserves earlier associations when manipulation changes visible cues. We evaluate ACE on two physical multi-step tabletop tasks, Semantic Formula Assembly and Constraint Retrieval. The visuomotor policy is trained only on generic pick-and-place demonstrations and reused without complete demonstrations of either evaluation task, enabling task-level zero-shot composition. Across 20 randomized trials per task, ACE achieves 70% and 80% success, respectively, compared with 55% and 70% without persistent context. These results suggest that an agentic harness can extend a primitive-trained manipulation policy to semantically distinct tasks through explicit object-destination interfaces and closed-loop execution feedback.

---

## 333. Don't Blame the Large Language Model: How Agent Harness Evolution Shapes Coding Agent Quality

**Autori:** Oussama Ben Sghaier, Hao Li, Bram Adams, Ahmed E. Hassan  
**Data:** 2026-07-04  
**Categorie:** cs.SE, cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2607.03691v2

> Coding agents, autonomous systems that use large language models (LLMs) to resolve software engineering tasks, rely on agent harness: a middleware layer in between a developer and a large language model that orchestrates system prompts, tool execution, context management, and iterative reasoning loops. While these agent harnesses evolve at extreme velocities, no study has examined how this evolution affects agent quality (i.e., effectiveness and efficiency) over time. Practitioners regularly report quality regressions after agent harness updates, yet consistently attribute them to the underlying model rather than the harness itself. In this paper, we address this gap by conducting the first controlled longitudinal study that isolates the agent harness contribution. Unlike prior work that fixes the agent harness and varies the model, we fix the model and vary only the agent harness, evaluating 35 sequential releases to measure their impact on agent effectiveness and efficiency. We first empirically study the development and release evolution of five major open-source agent harnesses (i.e., Codex, Qwen Code, Gemini, OpenCode, and OpenHands), revealing extreme release velocities exceeding two releases per day and thousands of issues within months. We then perform a controlled deep dive into 35 sequential releases of the Qwen Code CLI, evaluating each against 50 stratified SWE-bench Verified tasks while holding the underlying LLM constant. We trace the resulting quality fluctuations to specific development patterns and architectural components, and illustrate our findings with concrete qualitative evidence linking individual pull requests to measured quality shifts.

---

## 334. Reasoning effort, not tool access, buys first-try reliability in agentic code generation: an observational study

**Autori:** Achint Mehta  
**Data:** 2026-07-02  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2607.02436v2

> Agentic coding assistants are increasingly given extra capabilities, such as browser based testing tools and design oriented system prompts, on the assumption that more capability yields better software. This study tested that assumption directly. Ninety independent agent runs built the same application, a real time retrospective board, from one detailed specification, each scored on a fixed 14 criterion functional rubric (42 point maximum) and a visual quality review. The runs spanned several model generations, two agent harnesses, two reasoning effort levels, a testing tool, and two design oriented prompts. Capability tier dominated: frontier models clustered near the ceiling while a low cost local model fell to 24 to 37 points. A criterion level analysis revealed what run totals conceal. Container deployment was the dominant defect, failing first try in 44 percent of runs, with its failure rate shifting sharply across model generations while mean totals moved less than a point. The testing tool raised cost by 42 to 68 percent without improving functional score or reliability, even on interface visible criteria. Raising reasoning effort from High to xHigh lifted first try perfect runs from 28 percent to 89 percent and cut corrective prompts about five fold, for 9 to 29 percent more cost. A design oriented prompt raised visual quality, 4.5 versus 3.0 on a 5 point scale, without lifting function, and a one paragraph paraphrase of its directive reproduced the entire lift. The practical lesson is to match the fix to the failure: most first run failures came from weak reasoning, which a stronger model or more effort prevents, not from visible flaws a checking tool would catch.

---

## 335. AGC-Bench: Measuring Artificial General Creativity

**Autori:** Roger Beaty, Vijeta Deshpande, Clin K. Y. Lai, Anna Attuch, Namrata Shivagunde, Swastik Roy, Rajkumar Pujari, Paul V. DiStefano, Sherin Muckatira, Claire E. Stevenson, Mikhail Gronas, Anna Rumshisky  
**Data:** 2026-07-01  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2607.01152v2

> Creativity research has debated whether creativity is domain-specific (e.g., visual, writing, science), and if it is psychometrically separable from general intelligence. Both questions now apply to LLMs, but a unified benchmark of AI creativity remains elusive. We introduce AGC-Bench, an artificial general creativity benchmark built from a systematic review of the AI creativity literature (3,101 papers screened, 497 benchmarks identified), paired with an agentic harness that converts idiosyncratic codebases into HELM-standardized benchmarks. The first release covers 78 datasets spanning brainstorming, problem solving, STEM, narrative, figurative language, and humor. To address bias in LLM-as-judge, we apply Judge Response Theory -- a psychometric calibration of judge leniency/severity; we then fine-tune Qwen3-30B on the bias-corrected ratings of three frontier LLMs to produce AGC-Judge, an open-weight model that robustly scores new creativity benchmarks it was not trained on. Results reveal frontier models at the top of the AGC-Bench leaderboard, with open models close behind. LLMs show different creative strengths, ranking higher on some domains (e.g., writing) than others (e.g., scientific ideation). Extensive experiments yield three main findings. First, applying factor analysis across 83 LLMs, we recover a single creativity factor 'c', analogous to the 'g' factor of general intelligence, that explains 81.5% of variance, related to but separable from general knowledge/reasoning. Second, we show that prompting models to "be creative" boosts their performance far more than enabling reasoning, evidence that the benchmark tracks creativity over general ability. Third, on a human-matched subset, we find the top human still leads the top LLM on creativity. We release AGC-Bench with a public leaderboard, AGC-Judge, and human data as open infrastructure for measuring AI creativity at scale.

---

## 336. Evaluating Agentic Harness Systems for Autonomous Computational Pathology

**Autori:** Jie Lin, Zongyi Chen, Qiaoling Zheng, Liuyi Wang, Hengyi Jiang, Jiabao Chen, Xiang Liu, Yinghong Yang, Liansheng Wang  
**Data:** 2026-07-01  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2607.02598v1

> Autonomous computational pathology (ACP) converts high-level pathology analysis goals into executable, traceable and clinically bounded workflows. Realizing this capability requires adapting general agentic harness systems to pathology-specific tasks, tools, evidence standards and clinical claim boundaries. We contribute ACP-Bench, a framework that adapts existing harness systems from computational pathology support toward ACP workflow capability. ACP-Bench evaluates 41 pathology workflow tasks, including 24 biomarker, 7 morphology and 10 prognosis tasks spanning 6 body-system groups and 9 endpoint families. The benchmark evaluates 9 models and 3 harness groups (Claude Code, Codex and Open Code), yielding 369 complete trajectories. ACP-Bench evaluates each trajectory across workflow execution, diagnostic performance and clinical-boundary alignment, combining expert-adjudicated process audits, diagnostic assessment and pathologist-validated safety review. Across evaluated systems, workflow initiation, task interpretation and diagnostic reporting were more mature than tool-bound execution, result binding and reflective workflow revision, and formal end-to-end completion remained rare. ACP-Bench provides a reusable standard for auditing whether agentic systems can operationalize pathology workflows before claims of reliable clinical autonomy.

---

## 337. Representation Affects Retrieval: A Case Study of Skill Discovery and Routing in a Multimodal Agent Harness

**Autori:** Kevin Dela Rosa  
**Data:** 2026-06-30  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.20389v1

> A production agent harness must discover and rank, from a growing library of skills, the one most appropriate for a user's task. At small scale this selection happens in context: the LLM planner chooses among skill representations exposed in its system prompt, without an explicit embedding-based retrieval step. We treat this in-context selection as the small-N counterpart to embedding-based skill retrieval at scale, and present a case study of how Tinycloud, a production multimodal video agent harness, represents its skills for the planner. The harness ships skills under two recurring representations: tool-skills that wrap a single external API or system tool and serve as primitive vocabulary, and workflow-skills that orchestrate tool-skill calls plus a template render to produce one named deliverable. The harness exposes them via two surfaces in the system prompt: an inlined-body surface (full instructions, scripts, templates) for autoloaded skills, and a one-line listing for on-demand skills. A six-task selection ablation across three exposure regimes (all-on, default, all-off) shows that full autoload selects the gold skill on every task; all-off slows execution and produces hard discovery failures; and the production default misroutes one task because its lexical signal collides with an autoloaded tool-skill that pulls planner attention away from a listed workflow-skill. The headline finding is that in-prompt exposure of skills is not monotonically helpful: partial exposure can create lexical competition that suppresses correct selection. We connect this small-N observation to recent retrieval-based skill-routing work at large scale, and frame this contribution as a case study rather than a benchmark.

---

## 338. SWE-Router: Routing in Multi-turn Agentic Software Engineering Tasks

**Autori:** Seongho Son, Sangwoong Yoon, Jiahua Tang, Shuhan Wang, Lorenz Wolf, Ilija Bogunovic  
**Data:** 2026-06-30  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2607.00053v1

> Large language models (LLMs) embedded in multi-turn agentic harnesses are reshaping software engineering (SWE), but routing every task to a frontier model is wasteful when many issues admit cheap fixes. Existing LLM routers operate on the task description alone, which inherits an information-theoretic Bayes-error floor in agentic settings: a similar issue can hide either a localized typo or a multi-module refactor, and the prompt does not separate the two. We introduce SWE-Router, a value-based temporal approach that lets a cheap model run for a few exploratory turns and reads the resulting partial trajectory before deciding whether to continue cheaply or to escalate to an expensive model. We provide a Bayes-optimality theorem showing that conditioning on the partial trajectory never harms routing and is strictly better whenever exploration is informative. Across the LLM pairs of weak and strong models spanning the contemporary cost--capability frontier, we show that SWE-Router greatly improves the cost efficiency of SWE tasks, while maintaining the majority of the performances of the stronger model. We additionally release a multi-LLM trajectory dataset which allows reproduction of our trajectory-level routing.

---

## 339. NOVA: A Verification-Aware Agent Harness for Architecture Evolution in Industrial Recommender Systems

**Autori:** Shaohua Liu, Liang Fang, Yilong Sun, Shudong Huang, Qingsong Luo, Shaoxin Liu, Xiaoyang Chen, Dongqiang Liu, Chuangang Ma, Zhenzhen Chai, Henghuan Wang, Shijie Quan, Changyuan Cui, Zhangbin Zhu, Peng Chen, Wei Xu, Lei Xiao, Haijie Gu, Jie Jiang  
**Data:** 2026-06-25  
**Categorie:** cs.IR, cs.SE  
**Link:** https://arxiv.org/abs/2606.27243v3

> Industrial advertising recommender systems are continually improved through architecture modifications, yet production iteration remains expert-intensive because coordinated changes to model topology, feature configuration, and interaction modules must satisfy strict interface, resource, and serving constraints. AutoML is limited to predefined search spaces, while generic coding agents verify runnability rather than recommender-specific semantic validity. Executable candidates may therefore violate architectural contracts, while the lack of structured reuse of semantic diagnostics and evaluation outcomes can lead to repeated invalid or ineffective modifications. We present NOVA, a verification-aware agent harness that organizes production architecture modification as multi-round search over concrete implementations within a fixed evaluation budget. At each round, NOVA generates multiple candidates under production constraints, rejects semantic violations, and ranks the valid survivors for local testing and offline evaluation. Across rounds, trajectory memory synthesizes semantic diagnostics, local-test outcomes, and offline metric changes into modification directions and forbidden patterns that guide subsequent search. Under the same maximum offline-evaluation budget for automated methods, NOVA achieves the highest effective pass rate, reaching 53.3% on ScaleUp and 51.7% on Literature-to-Production tasks. In a production A/B test covering 5% of traffic in an advertising system serving over one billion users, the selected Literature-to-Production candidate yields GMV gains of +1.25%, +1.70%, and +2.02% across three major pCVR objectives, with corresponding relative reductions in absolute pCVR bias of 58.8%, 66.7%, and 37.3%, respectively.

---

## 340. The Hitchhiker's Guide to Agentic AI: From Foundations to Systems

**Autori:** Haggai Roitman  
**Data:** 2026-06-22  
**Categorie:** cs.AI, cs.CL, cs.IR, cs.LG  
**Link:** https://arxiv.org/abs/2606.24937v3

> The Hitchhiker's Guide to Agentic AI is a comprehensive practitioner's reference for building autonomous AI systems, covering the full stack from first principles to production deployment. The central thesis: building great agentic systems requires understanding every layer of the pipeline, not just one. The book opens with the LLM substrate, covering transformer architecture, GPU systems, training and fine-tuning (SFT, LoRA, MoE), model compression, and inference optimization, as essential foundations. It then develops the alignment and reasoning layer: RLHF, PPO, DPO and its variants, GRPO, reward modeling, and RL for large reasoning models including chain-of-thought and test-time scaling. The second half is devoted to agentic AI proper: agentic training and trajectory-based RL, RAG and Agentic RAG, memory systems (in-context, external, episodic, and semantic), agent harness design, loop engineering, graph-based orchestration, and a taxonomy of agent design patterns covering security, red teaming, and gateway infrastructure. Inter-agent coordination is covered in depth: the Model Context Protocol (MCP), agent skills and tool use, the Agent-to-Agent (A2A) protocol, and multi-agent architectures spanning centralized, decentralized, and hierarchical topologies. The book concludes with agent development frameworks, agentic UI design, evaluation methodology (non-deterministic evaluation, reasoning collapse, LLM-as-Judge), production deployment, and the regulatory environment (EU AI Act, California SB 942) as an engineering requirement. Each chapter pairs theory with implementation guidance, executable notebooks, and references to the primary literature.

---

## 341. AOHP: An Open-Source OS-Level Agent Harness for Personalized, Efficient and Secure Interaction

**Autori:** Shanhui Zhao, Jiacheng Liu, Guohong Liu, Jichao Yan, Jialei Ye, Yuhao Yang, Hao Wen, Shizuo Tian, Yizhen Yuan, Yuxuan Chen, Yunxin Liu, Ju Ren, Ya-Qin Zhang, Chao Huang, Yao Guo, Yuanchun Li  
**Data:** 2026-06-22  
**Categorie:** cs.AI, cs.OS  
**Link:** https://arxiv.org/abs/2606.23449v1

> AI agents are driving a new software paradigm, with the ability to autonomously call tools, extract information, manage memory, and complete tasks that span applications and data sources. Most existing end-user operating systems, however, are designed for application-centric workflows and offer little native support for AI agents. This mismatch limits the wider adoption of agents and leads to execution overhead and safety risks when running agents on conventional systems. While the concept of agent-native operating systems is emerging, the research community lacks an open testbed to explore the architectural primitives desired for agent-mediated interaction. We present AOHP (Android Open Harness Project), an OS-level agent harness built on the Android Open Source Project (AOSP). The core design principle of AOHP is to treat agents as first-class OS actors, enabling adaptive user interfaces and agent-friendly runtime environments. AOHP preserves the mature Android software and hardware ecosystem while introducing three agent-oriented system mechanisms: personalized service composition, efficient agent interfaces, and secure information flow. Based on preliminary experiments on challenging tasks covering key capabilities of OS agents, AOHP shows clear advantages in task completion (+21.12% completion rate), execution cost (-51.55% token cost), and security-policy compliance.

---

## 342. IPO Finance Agent: Benchmark of LLM Financial Analysts Beyond Finance Agent v2, with Automated Rubric Generation, on the SpaceX (SPCX) IPO

**Autori:** Mostapha Benhenda  
**Data:** 2026-06-22  
**Categorie:** cs.AI, q-fin.GN  
**Link:** https://arxiv.org/abs/2606.23032v3

> Finance Agent v2 (by Vals AI) has emerged as the reference benchmark for evaluating both Anthropic Claude and OpenAI ChatGPT frontier language models on financial tasks. However, it narrowly deals with periodic reporting from publicly traded companies (SEC 10-K and 10-Q filings), and its agentic harness relies on naive, unenriched chunk retrieval. Neither the task design nor the retrieval approach addresses the distinct challenges of IPO due diligence. SEC S-1 filings combine historical financial statements, governance structures, pro forma and common-control accounting treatments, capital-formation narratives, and underwriting-sensitive risk disclosures within substantially longer documents than typical periodic filings. That is why we introduce IPO Finance Agent, which extends the Finance Agent v2 framework along two directions: task domain and retrieval architecture. During our experiments, the original Finance Agent v2 harness basically failed to deliver any output related to the SpaceX S-1 filing, due to document length. We therefore had to improve the agentic harness with contextual retrieval, a more realistic and industry-standard approach for long documents. We also built a dataset of 1,000 IPO-diligence questions, and publicly release 70 questions on the SpaceX (SPCX) S-1 filing to support reproducibility, while the remainder are held private to guard against benchmark contamination. In addition, we introduce an evaluator-optimizer pipeline to automatically generate evaluation rubrics for the benchmark: candidate facts are extracted from model answers, consolidated into draft criteria, then automatically audited for omissions, hallucinations, mistiered items, and redundancy, with LLM feedback driving iterative repair, targeted enrichment, and deduplication. Human experts only review final rubrics before deployment. Results show that the best-performing evaluated model, Zhipu GLM-5.2, reaches 79.8% accuracy, and the most cost-efficient model on the resulting Pareto frontier, Xiaomi MiMo-2.5 Pro, reaches slightly lower accuracy (77.2%) at 0.05 USD per query, while exceeding the current Finance Agent v2 leaderboard ceiling, Google Gemini 3.5 Flash at 57.9% for 2.51 USD per query, and undercutting even FABv2's cheapest entry (MiniMax M3: 48.3% at 0.32 USD) on cost-efficiency. Code and data are released on GitHub https://github.com/benstaf/ipoagent

---

## 343. Code Isn't Memory: A Structural Codebase Index Inside a Coding Agent

**Autori:** Ishaan Bhola, Adithyan Krishnan, Sravanth Kurmala, Mukunda NS  
**Data:** 2026-06-21  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2606.22417v1

> Coding agents now interleave LLMs with retrieval over the working repository, and retrieval implementations vary widely across deployed harnesses. Inside a fixed coding-agent harness on a fixed model, does adding a structural codebase index actually change cost or resolve? We ran three arms (the harness with the index, the same harness without it, and an agentic-grep comparator) on SWE-PolyBench Verified and SWE-bench Pro with Claude Opus 4.7 held fixed throughout, across three seeds, inside a leak-audited per-task sandbox. The within-harness ablation produces a large localization gain and a statistically separated resolve gain, with no cost penalty per cell and lower cost per solve. The cross-harness check shows that the index does not regress against an agentic-grep baseline on resolve or localization, again at no cost penalty. We release the per-cell exclusion ledger, the leak-audit script, the localization extractor, and the results database. The deployment question for a structural codebase index is thus not whether it is too expensive to run (across seeds, the index lands at a lower $/solved than agentic grep) but whether the workload includes multi-file changes where structural ranking pays off.

---

## 344. Building Agent Harnesses for Scientific Curation from Multimodal Sources

**Autori:** Sheng Zhang, Qin Liu, Renqian Luo, Shufang Xie, Reuben Tan, Sean Hayes, Gregory Bryman, Wendong Ge, Ruilian Zhang, Oluwaseun Egbelowo, Kelly Yee, Hoifung Poon  
**Data:** 2026-06-19  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2606.21005v2

> Scientific discovery workflows often depend on structured curation from the literature. This is difficult for current agents because the key evidence is scattered across long text, dense tables, and figures, and the final records often require reasoning across multiple evidence fragments rather than copying a single span. We study scientific curation from multimodal sources and introduce Beaver, an agent harness that extracts structured information from scientific papers while preserving provenance to the supporting evidence. Beaver combines a frontier agent with multimodal evidence tooling, task scaffolding, and artifact-grounded autoresearch. These components turn curation into a staged, auditable workflow and enable an iterative evaluate--diagnose--revise loop, where persistent run artifacts expose stage-localized failures and guide harness updates. Experiments show that Beaver reaches 81.0 on Gold-Referenced Attribute Score (GRAS), an attribute-level measure of agreement with gold curated records, outperforming frontier agents by over 23 absolute points. Ablations show that task scaffolding, multimodal evidence tooling, and provenance traces each contribute meaningfully to performance, while attribute-level analysis shows the largest gains on high-value attributes that require cross-modal reasoning and normalization. These results show that, for scientific curation from papers with multimodal evidence, harness design is a central determinant of agent performance.

---

## 345. StaminaBench: Stress-Testing Coding Agents over 100 Interaction Turns

**Autori:** Vlad Sobal, Shuo Yang, Yuting Zhang, Wei Xia, Stefano Soatto  
**Data:** 2026-06-17  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2606.19613v1

> We introduce StaminaBench, a benchmark that measures the stamina of coding agents: how many consecutive interaction turns (change requests) they can handle before failing. Unlike the prevailing fraction-of-tasks-solved metric, this matches real vibe-coding where sessions run dozens or hundreds of turns. In StaminaBench, agents implement a REST API server and modify it across a tunable number of procedurally generated follow-up change requests - 100 in our experiments, resulting in codebases of up to 6,000 lines. Tests are generated fully programmatically without LLM involvement, ensuring reproducibility and reliability; change sequences are drawn from either a hardcoded or LLM-driven sampler, both constrained to a structured action space to ensure changes are valid. The agent and the server run in an isolated environment and communicate with the benchmark through HTTP, making testing fully black-box and language-agnostic. We evaluate six agent harnesses paired with seven open-source LLMs across 20 scenarios of 100 turns each and find that: (1) all the tested models fail within 5-6 turns, confirming that vibe-coding-style programming without thorough testing produces bugs; (2) passing test feedback back to the agent and allowing it to retry improves passed turn count by up to 12x; and (3) a good harness is required for strong performance: stronger models exhibit up to a 6x gap between their best and worst harness, while weaker models fail with any harness. We release the benchmark and the generated tasks to enable further research into multi-turn coding agent behavior. Benchmark code and data: github.com/amazon-science/StaminaBench.

---

## 346. Guava: Distilling Frontier VLMs into a Compact Agent through a Robotic Manipulation Harness

**Autori:** Haowen Liu, Xirui Li, Shaoxiong Yao, Peng Shi, Tianyi Zhou, Jia-Bin Huang, Furong Huang, Jiayuan Mao  
**Data:** 2026-06-16  
**Categorie:** cs.RO, cs.AI  
**Link:** https://arxiv.org/abs/2606.18363v3

> Language models trained on large-scale vision-language data have demonstrated strong potential for embodied agents. Harnessing models through embodied tools use offers a promising alternative to end-to-end vision-language-action systems by combining high-level reasoning with external modules for perception, planning, and control. However, it remains unclear what makes an effective harness for embodied manipulation, and to what extent such a harness can unlock embodied capabilities in a wide range of reasoning models. In this work, we present Guava, a harness framework for embodied tool use developed through systematic exploration of the design space of agent workflows, action spaces, and observation spaces. Our study identifies three key ingredients for effective embodied agents: iterative perception-reasoning-action loops, semantic action abstractions, and multimodal observations. To understand whether these design principles are universal even to small models, we develop an end-to-end training pipeline that distills embodied manipulation capabilities into a 4B open-source model using fewer than 2K trajectories collected entirely in simulation. Experimental results in both simulation and real-world environments show performance comparable to frontier proprietary models while exhibiting strong generalization to unseen objects, novel instructions, and long-horizon tasks. Results suggest that a well-designed harness can serve as a scalable, model-agnostic interface for embodied manipulation, enabling strong emergent embodied capabilities in compact open-source models with minimal training data.

---

## 347. SEAGym: An Evaluation Environment for Self-Evolving LLM Agents

**Autori:** Congjie Zheng, Chuanyi Xue, Bin Liang, Jun Yang, Changshui Zhang  
**Data:** 2026-06-16  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2606.17546v1

> Self-evolving LLM-based agents improve mainly by changing their agent harness: the structured execution layer around a base model, including prompts, memory, tools, middleware, runtime state, and the model-tool interaction loop. Existing evaluations often reduce this process to isolated task scores or a single sequential curve, obscuring whether an update produces reusable improvement, overfits recent tasks, increases cost, or harms older behavior. We introduce SEAGym, an evaluation environment for measuring agent harness updates across training, validation, test, replay, and cost records. SEAGym turns Harbor-compatible benchmarks into dynamic self-evolution task sources with train batches, frozen update-validation, held-out ID and OOD transfer views, replay diagnostics, and saved snapshot and metric records. Instantiating SEAGym on Terminal-Bench 2.0 and HLE, we compare ACE, TF-GRPO, and AHE under a shared epoch/batch protocol. The results show that these evaluation views provide complementary signals about the evolution process: frequent updates may fail to improve held-out performance, useful intermediate snapshots may collapse later, and source diversity and model backend can affect harness reliability.

---

## 348. Dissecting model behavior through agent trajectories

**Autori:** Gaurav Gupta, Vatshank Chaturvedi, Sudipta Sengupta, Jun Huan, Anoop Deoras  
**Data:** 2026-06-16  
**Categorie:** cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2606.17454v3

> AI agent performance is not just a modeling problem, it is fundamentally a systems problem. The advanced capabilities of models are realized through agent harnesses. Therefore, a gap between model assumptions and harness behavior can easily prevent the model's full capabilities from translating into agent performance. We formalize this as the `intent-execution' gap: the mismatch between what the model intends and what the harness executes, and vice versa. We argue that minimizing this intent-execution gap is as important as other aspects of harness design such as tools and execution loops. To illustrate the impact of this harness-model alignment, we develop a simple and customizable harness called `Simple Strands Agent' (SSA). SSA aims to find the bulk of common patterns which generalize across different model families (such as Claude, Gemini, GPT, Grok, Qwen), as well as a small number of model-specific preferences. We make two contributions: (i) we \textbf{reproduce or improve on the pass@1} performance reported by diverse model-provider families on popular agentic benchmarks (SWE-Pro, SWE-Verified, Terminal-Bench-2, and Deep-SWE), and (ii) building on an \textbf{analysis of 154\texttt{k} trajectories generated by SSA}, we look beyond the \texttt{pass@1} numbers which tend to be relatively even across frontier models. By representing agent trajectories in code state-spaces, we compute solution distance and backtracking to observe model-level differences in problem-solving behavior. Finer-grained metrics such as edit frequency, testing activity, and phase-transitions reveal how individual models allocate effort across different stages of problem solving.

---

## 349. MyPCBench: A Benchmark for Personally Intelligent Computer-Use Agents

**Autori:** Lawrence Keunho Jang, Andrew Keunwoo Jang, Jing Yu Koh, Ruslan Salakhutdinov  
**Data:** 2026-06-15  
**Categorie:** cs.LG, cs.CL  
**Link:** https://arxiv.org/abs/2606.16748v1

> Current benchmarks for computer-use agents evaluate models in impersonal environments. This leaves a gap between evaluation and deployment where personal assistants are expected to work across a user's whole digital life, including their context, historical data, and logged-in accounts. This gap is widest on web tasks, where live web evaluations cannot exercise sites that require logging in or personal information, the kind of site a real personal assistant has to drive. We introduce MyPCBench, which tests computer-use agents as personal assistants on a Linux desktop populated with 17 simulated real-world web applications and a full desktop stack, all seeded for one canonical persona, Michael Scott from The Office. We define 184 tasks in this environment, each inspired by a real request drawn from the OpenClaw community, and benchmark six closed and open-weight models with a uniform computer+bash tool surface. We find that the best model, Claude Opus 4.6, fully solves 55.4\% of the tasks, the only model above 50\%. Model failures cluster on tasks that span many applications and on long trajectories, where personalization stresses an assistant the most. We release the environment, task set, and agent harness at https://mypcbench.com.

---

## 350. SING: Synthetic Intention Graph for Scalable Active Tool Discovery in LLM Agents

**Autori:** Qiao Xiao, Haochen Shi, Yisen Gao, Wenbin Hu, Huihao Jing, Tianshi Zheng, Baixuan Xu, Ziheng Zhang, Weiqi Wang, Haoran Li, Jiaxin Bai, Yangqiu Song  
**Data:** 2026-06-15  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2606.16591v2

> Large language model (LLM) agents increasingly rely on agent harnesses that manage context, tools, and multi-turn execution, making tools a central interface for acting in realistic digital environments. As harness-connected tool ecosystems expand to hundreds or thousands of APIs, services, and task-specific skills, exhaustive tool schema injection becomes costly and imposes a closed-world assumption that limits agents to a predefined static inventory. Retrieval-augmented tool selection offers a natural alternative, but existing one-shot retrieval methods often fail to align isolated tool descriptions with the agent's true task intention, especially in long-horizon tasks where required capabilities emerge through decomposition, observations, and newly induced subgoals. We propose SING, an intention-aware active tool discovery framework that builds an intention-tool graph linking user intentions, tool capabilities, and tool collaboration patterns, and dynamically retrieves tools according to evolving task states. Using a unified corpus of 7,471 tools, we evaluate SING on three real-world tool-use benchmarks. SING improves Global Recall@5 by up to 59.8% and downstream success rate by up to 28.9% over baselines, while reducing full-corpus tool-schema exposure by 99.8%, demonstrating that intention-aware graph structure enables more accurate and context-efficient tool discovery in large-scale agentic ecosystems.

---

## 351. Open-SWE-Traces: Advancing Dual-Mode Multilingual Distillation for Software Engineering Agents

**Autori:** Wasi Uddin Ahmad, Nikolai Ludwig, Somshubra Majumdar, Boris Ginsburg  
**Data:** 2026-06-14  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2606.16038v1

> The path toward autonomous software engineering is currently bottlenecked by a severe deficit of diverse, large-scale trajectory data. We address this by introducing \ourdataset, an expansive dataset of 207,489 agentic trajectories spanning nine programming languages (Python, Go, TS, JS, Rust, Java, PHP, C, C++). Sourced from 20,000 real-world PRs via OpenHands and SWE-agent harnesses, the dataset utilizes a hybrid-reasoning synthesis: Minimax-M2.5 generates trajectories with explicit "thinking" processes, while Qwen3.5-122B provides high-quality "non-thinking" traces. Filtered for permissive licenses (MIT, Apache, BSD) from SWE-rebench-V2, this data facilitates the training of models capable of long-horizon reasoning. We validate the dataset by fine-tuning the Qwen3-30B-A3B series (Thinking, Instruct, and Coder). The best performing model achieves resolve rates of 61.7% on SWE-bench Verified, 57.1% on SWE-bench Multilingual, and 36.8% on SWE-bench Pro. These results establish Open-SWE-Traces as a premier resource for distilling human-level software engineering capabilities into efficient, open-source agentic LLMs.

---

## 352. LLM-as-Code: Agentic Programming for Agent Harness

**Autori:** Junjia Qi, Zichuan Fu, Jingtong Gao, Wenlin Zhang, Hanyu Yan, Xian Wu, Xiangyu Zhao  
**Data:** 2026-06-14  
**Categorie:** cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2606.15874v2

> Every major LLM agent framework gives the LLM the role of orchestrator; the model decides what to do next, when to call tools, and when to stop. We argue that token explosion, control-flow hallucination, and unreliable completion are not implementation bugs but architectural consequences of assigning the deterministic work of looping, branching, and sequencing to a probabilistic system. A better prompt or a stronger model cannot guarantee the reliability of the LLM agent. We therefore propose Agentic Programming, in which the program governs all control flow, and the LLM is itself part of it, an adaptive component we call LLM-as-Code and invoke only where a task calls for reasoning or generation. Within each call the model keeps full flexibility, but it cannot alter the program's execution path. With control in the program, the LLM's context is built from the execution history's call tree and forms a directed acyclic graph (DAG). Each call's context length is then determined by its call depth rather than by accumulation over steps. A case study of computer-use agents shows that the design is practical, not just a theoretical stance, substantially improving the stability of long visual operation sequences.

---

## 353. ClayBuddy: A Framework, Evaluation, & Mitigation of Coding Agent Failures

**Autori:** Kenneth Ge, Andre Assis  
**Data:** 2026-06-13  
**Categorie:** cs.SE, cs.LG  
**Link:** https://arxiv.org/abs/2606.19380v5

> Widespread deployment of AI agents in software engineering is surfacing a long tail of rare but highly dangerous misalignment bugs. Since sampling this behavior is intractable, we decompose these failures into three distinct mechanisms: underspecification, where default model behavior is unsafe; capability errors, where the safe action is available but the model does not adhere to it; and agent harness errors, where the safe action fails to execute. Across 8 evaluations that stress test these mechanisms, we find that frontier models are difficult to steer, elicit dangerous behavior through just 3 conditioning examples, and can randomly generate destructive commands at nontrivial probabilities. These three mechanisms naturally lend to targeted mitigations for each one, inspiring our harness modification ClayBuddy. ClayBuddy allows the agent to modify its own harness to provide safety guarantees, including a novel tool to selectively truncate its own context. We measure ClayBuddy's efficacy across safety and capabilities, finding that it eliminates violations across some tasks. This demonstrates that our decomposition is effective and is an example of our harness design philosophy.

---

## 354. APEX: Adaptive Principle EXtraction A Three-Layer Self-Evolution Framework for Production AI Agents

**Autori:** Ya-Chuan Chen, Tien-Jen Lai, Hsiang-Wei Hu  
**Data:** 2026-06-13  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2606.15363v1

> Self-improvement in AI agents has emerged as a key research frontier: systems that modify their own prompts, workflows, and decision rules based on accumulated operational experience. The state-of-the-art Self-Harness framework [1] achieves 14--21% improvement on Terminal-Bench-2.0 by mining failure clusters and patching the agent harness. However, Self-Harness optimises only one dimension -- the prompt harness -- leaving behavioural principles and workflow topology unchanged. We propose APEX (Adaptive Principle EXtraction), a three-layer co-evolution framework that simultaneously evolves: (L1) the harness via failure-mode patching, (L2) behavioural principles via success-trace distillation [2], and (L3) the agent workflow topology via structural fitness-based selection [6]. We implement APEX on Joe [13], a production-grade super AI Agent built on NVIDIA Nemotron and designed as an Edge AI Agent Factory for the NVIDIA Agent Challenge 2026, managing a 15-node compute fleet using 114 real task traces collected over 18 days. APEX achieves an APEX Health Score of 0.570 (+90% vs. baseline 0.300) in a single evolutionary run, distilling 6 novel reusable principles and selecting a research-first workflow topology scoring 0.900 (+20%). Our results demonstrate that multi-dimensional co-evolution substantially outperforms single-axis harness optimisation, at a cost of only 4 LLM calls (~270 s) on a local qwen2.5-coder:32b instance.

---

## 355. HarnessX: A Composable, Adaptive, and Evolvable Agent Harness Foundry

**Autori:** Tingyang Chen, Shuo Lu, Kang Zhao, Weicheng Meng, Hanlin Teng, Tianhao Li, Chao Li, Xule Liu, Jian Liang, Zhizhong Zhang, Yuan Xie, Heng Qu, Kun Shao, Jian Luan  
**Data:** 2026-06-12  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2606.14249v3

> AI agent performance depends critically on the runtime harness, comprising the prompts, tools, memory, and control flow that mediate how a model observes, reasons, and acts. Yet today's harnesses remain largely hand-crafted and static: each new model or task still demands bespoke scaffolding, and the rich traces produced during execution are rarely distilled back into systematic improvement. We introduce HarnessX, a foundry for composable, adaptive, and evolvable agent harnesses. HarnessX assembles typed harness primitives via a substitution algebra, adapts them through AEGIS, a trace-driven multi-agent evolution engine grounded in an operational mirror between symbolic adaptation and reinforcement learning, and closes the harness-model loop by turning trajectories into both harness updates and model training signal. Across five benchmarks (ALFWorld, GAIA, WebShop, tau^3-Bench, and SWE-bench Verified), HarnessX yields an average gain of +14.5% (up to +44.0%), with gains largest where baselines are lowest. These results suggest that agent progress need not come from model scaling alone: composing and evolving runtime interfaces from execution feedback is an actionable and complementary lever. Project homepage: https://darwin-agent.github.io/HarnessX/.

---

## 356. Recursive Agent Harnesses

**Autori:** Elias Lumer, Sahil Sen, Kevin Paul, Vamse Kumar Subbiah  
**Data:** 2026-06-11  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2606.13643v1

> Recursive language models (RLMs) showed that recursion over model calls is an effective strategy for long-context reasoning, and production coding agents have begun to write code that spawns subagents at scale, most recently in Anthropic's dynamic workflows. We name and study the pattern between these two lines of work, where the recursive unit is a full agent harness with filesystem tools, code execution, and planning rather than a model call with no tools. We call this the Recursive Agent Harness (RAH) and frame it as harness recursion, the code-first extension to the model recursion of RLMs. A parent agent generates and runs an executable script that spawns subagent harnesses in parallel for fine-grained workloads and uses structured function calls for small subtasks. We provide a controlled evaluation on long-context reasoning. With the backbone held fixed at GPT-5 to match the published Codex and RLM baselines, RAH improves the Codex coding-agent baseline from 71.75% to 81.36% on Oolong-Synthetic (199 samples, 13 context-length buckets up to 4M tokens), a gain attributable to the harness rather than the model. With a stronger backbone, Claude Sonnet 4.5, the same design reaches 89.77%.

---

## 357. HarnessBridge: Learnable Bidirectional Controller for LLM Agent Harness

**Autori:** Xiaoxuan Wang, Haixin Wang, Alexander Taylor, Jason Cong, Yizhou Sun, Wei Wang  
**Data:** 2026-06-11  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2606.12882v1

> Large language models are increasingly deployed as agents for long-horizon tasks, yet their performance is shaped not only by model capability and environment design, but also by the harness that mediates agent--environment interaction. Existing harnesses are largely manually engineered, making them difficult to scale as trajectories grow longer and interactions become more complex. In this work, we ask whether harness can be generated by a learnable plug-in module that can be trained in an end-to-end fashion. We introduce HarnessBridge, a lightweight learnable harness controller that parameterizes the agent--environment interface as a bidirectional projection. HarnessBridge learns two bidirectional projections: observation projection, which distills raw trajectories into compact, decision-relevant states, and action projection, which converts proposed actions into executable transitions or trajectory-grounded rejections. We train HarnessBridge on a harness supervision dataset via unified instruction tuning. On Terminal-Bench~2.0 and SWE-bench Verified, HarnessBridge matches or surpasses strong specialized harnesses while substantially reducing token usage and trajectory length, and generalizes from smaller generators to larger commercial models.

---

## 358. Claw-SWE-Bench: A Benchmark for Evaluating OpenClaw-style Agent Harnesses on Coding Tasks

**Autori:** Mengyu Zheng, Kai Han, Boxun Li, Haiyang Xu, Yuchuan Tian, Wei He, Hang Zhou, Jianyuan Guo, Hailin Hu, Lin Ma, Chao Xu, Guohao Dai, Lixue Xia, Yunchao Wei, Yunhe Wang, Yu Wang  
**Data:** 2026-06-10  
**Categorie:** cs.LG, cs.CL  
**Link:** https://arxiv.org/abs/2606.12344v2

> The software engineering capabilities of general-purpose agent harnesses remain underexplored, and existing benchmarks offer limited support for comparing these harnesses under consistent conditions. To address this gap, we introduce Claw-SWE-Bench, a unified benchmark that enables researchers to systematically assess the capabilities and efficiency of general-purpose harnesses on software engineering tasks. The benchmark contains 350 real-world GitHub issue-resolution instances across eight programming languages and 43 repositories and provides a shared adapter protocol to align task inputs, outputs, and execution environments across harnesses. Experiments show that general-purpose harnesses can effectively resolve real-world software issues and that their success rates and resource consumption vary substantially even when the underlying model is held fixed. To lower evaluation costs and support faster debugging and iteration, we also provide Claw-SWE-Bench Lite, an 80-instance subset designed to preserve the key evaluation properties of the full benchmark. We hope this benchmark will help researchers better evaluate and understand the performance of general-purpose harnesses on software engineering tasks and guide the development of more capable and efficient harnesses. The data is available at https://github.com/opensquilla/claw-swe-bench and https://huggingface.co/datasets/TokenRhythm/Claw-SWE-Bench.

---

## 359. Decentralized Multi-Agent Systems with Shared Context

**Autori:** Yuzhen Mao, Jerry Gu, Aadi Chauhan, Qizheng Zhang, Hangoo Kang, Azalia Mirhoseini  
**Data:** 2026-06-09  
**Categorie:** cs.MA, cs.AI  
**Link:** https://arxiv.org/abs/2606.10662v3

> Multi-agent systems (MAS) can scale large language model agents on long-horizon tasks by running them in parallel, yet existing designs waste much of this parallelism in bubbles: agent time spent waiting on others or redoing a peer's work. These bubbles stem from how agents communicate. Independent agents share nothing and rediscover what their peers have already found; peer-communicating agents wait at synchronous rounds; and under centralized orchestration, the main agent blocks on its sub-agents while progress is relayed. We propose Decentralized Language Models (DeLM), a MAS framework on top of existing agent harnesses that squeezes out these bubbles by replacing the main agent with a shared context and a task queue. Agents asynchronously claim tasks, publish findings as soon as they are available, and build on or correct one another's progress, with every peer's status visible to all. On long-horizon tasks from Terminal-Bench 4.0 and DeepSWE v1.1, and on SWE-bench Verified, DeLM is both more accurate and faster than Codex, Claude Code, their native subagents, and AOrchestra in every setting, improving accuracy by up to 17.5 points over the strongest baseline and running up to 2.49x faster than the harness it builds on. On ProgramBench, where agents rebuild programs from scratch, DeLM makes faster progress than Claude Code and finishes a 120-minute budget up to 19.9 points higher in test pass rate. The code is available on our project website at https://yuzhenmao.github.io/DeLM/.

---

## 360. The Scaffold Effect in Coding Agents: Harness Choice as a Hidden Variable in Coding-Agent Evaluation

**Autori:** Naman Vats, Oleg Golev  
**Data:** 2026-06-08  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2607.22585v1

> Public leaderboards for coding agents typically rank systems by model name and pass rate, while the surrounding harness (the scaffold that issues tools, manages context, and decides when to stop) is often under-specified. Model-to-model comparison is valid when the harness is fixed; when it varies, performance and efficiency conflate model and scaffold effects. We evaluate Qwen 3.6 Plus and MiniMax M2.5 across three open-source harnesses (Goose, OpenCode, OpenHands-SDK) on a stratified 50-task subset of Terminal-Bench Pro. Harness choice induces up to a 40x difference in tokens per solved task, while paired within-model pass-rate differences remain 0-8 percentage points (95% paired-task bootstrap CIs include zero except for the largest gap). Failure fingerprints replicate across models (REASON for Goose, VERIFY/MAX_TURNS for OpenHands-SDK, idle-loop/TIME for OpenCode), indicating harness-level biases that are largely model-independent. For human-centered coding-agent evaluation, model name alone is an incomplete comparison unit: harness-model pairs determine real-world cost, latency, and oversight burden; no-action turns are a per-task wait tax, not just a token tax. We therefore recommend selecting harness-model pairs by pass rate under token/latency budgets, and reporting token usage, latency, and full harness specifications alongside any model comparison. We release anonymized configs, raw trial logs, aggregated snapshots, and analysis scripts.

---

## 361. What makes a harness a harness: necessary and sufficient conditions for an agent harness

**Autori:** Sanderson Oliveira de Macedo  
**Data:** 2026-06-08  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2606.10106v1

> The term agent harness now circulates widely in software engineering with generative artificial intelligence. It names the layer that wraps a language model and turns it into a coding agent able to act on a repository. The usage is loose and polysemous. Sometimes the term denotes the whole product (Claude Code, Codex CLI); sometimes it denotes the evaluation scaffold that runs an agent against tasks (the SWE-bench harness); sometimes it gets conflated with an agent framework, an SDK, an IDE plugin, or an orchestrator. What is missing is a reference definition that works as an instrument, one that includes and excludes cases consistently. We build that definition through a conceptual analysis that combines works with persistent identifiers and primary grey-literature sources, such as official documentation, glossaries, and engineering reports. We reconstruct the genealogy of the term, from the horse's tack to the classic test harness, to the machine-learning evaluation harness, and finally to the agent harness. We then propose a constitutive definition that states the necessary and sufficient conditions for a system to be an agent harness, we operationalize it as an inclusion and exclusion test, and we draw the boundary of the concept against an agent framework, an agent SDK, an IDE plugin, an eval harness, and an orchestrator. We apply the definition to six real harnesses (Claude Code, Codex CLI, Aider, Cline, OpenHands, and SWE-agent) and to deliberate edge cases; the test includes and excludes consistently. We close with a research agenda organized by design tension axes. The contribution is an operational definition of agent harness, with a shared vocabulary, able to guide engineering practice and the scientific comparison of agentic systems.

---

## 362. AutoMegaKernel: A Statically-Checked Agent Harness for Self-Retargeting Megakernel Synthesis

**Autori:** Jaber Jaber, Osama Jaber  
**Data:** 2026-06-08  
**Categorie:** cs.LG, cs.DC, cs.PF  
**Link:** https://arxiv.org/abs/2606.09682v1

> AutoMegaKernel (AMK) compiles a HuggingFace Llama-family model into a single persistent cooperative CUDA kernel that runs the whole forward pass in one launch, with no per-model hand-written CUDA. The contribution is the system, not raw speed. A frozen schedule-IR validator statically certifies deadlock-freedom and race-freedom via static graph checks (not a mechanized proof), so an unsafe agent-proposed schedule is rejected before launch: across 7,160 adversarial schedules (6,091 unsafe) it had zero false-accepts and accepted all 360 real lowerings. The same source retargets sm_80/sm_90/sm_120 from one codebase, auto-generates correct megakernels for 10 of 10 supported models, and on a real SmolLM2-135M checkpoint reproduces HuggingFace greedy decode token-for-token (perplexity match 2.5e-7). An unattended, agent-drivable autoresearch loop self-improves the megakernel over its own baseline (1.25-1.72x). A search-found int8 (W8A16) megakernel beats CUDA-graphed cuBLAS bf16 at batch-1 decode across NVIDIA's datacenter inference fleet: L4 up to 1.33x, the current-gen L40S 1.25-1.27x, A10G up to 1.08x at scale, and the consumer RTX 5090 1.19-1.23x. The ordering is not a clean function of bandwidth (the 864 GB/s L40S beats the 600 GB/s A10G); the divide is inference-class vs training-class. AMK trails cuBLAS on the high-bandwidth training-class A100/H100, where the harness localizes the cross-SM-sync bottleneck; we report the gap plainly. This is a precision-asymmetric (W8A16 vs bf16) comparison at decode position 0; the largest real checkpoint is TinyLlama-1.1B. Code and the harness: https://github.com/RightNow-AI/AutoMegaKernel

---

## 363. Self-Harness: Harnesses That Improve Themselves

**Autori:** Hangfan Zhang, Shao Zhang, Kangcong Li, Chen Zhang, Yang Chen, Yiqun Zhang, Lei Bai, Shuyue Hu  
**Data:** 2026-06-08  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2606.09498v3

> The performance of LLM-based agents is jointly shaped by their base models and the harnesses that mediate their interaction with the environment. Because different models exhibit distinct behaviors, effective harness design is inherently model-specific. Yet agent harnesses are still largely engineered by human experts, a paradigm that scales poorly as modern LLMs become increasingly diverse and rapidly evolving. In this paper, we introduce Self-Harness, a new paradigm in which an LLM-based agent improves its own operating harness, without relying on human engineers or stronger external agents. We operationalize Self-Harness as an iterative loop with three stages: Weakness Mining, which identifies model-specific failure patterns from execution traces; Harness Proposal, which generates diverse yet minimal harness modifications tied to these failures; and Proposal Validation, which accepts candidate edits only after regression testing. We instantiate Self-Harness across Terminal-Bench-2.0, SWE-bench Verified, and AppWorld using a minimal initial harness and three base models from diverse families: MiniMax M2.5, Qwen3.5-35B-A3B, and GLM-5. Across all nine model--benchmark combinations, every final harness improves both held-in and held-out pass rates, with overall relative gains of up to 132%. Qualitative analyses further show that the retained mechanisms address benchmark-specific bottlenecks in artifact handling and runtime control, software-patch verification, and application-state retrieval. These results suggest a path toward LLM-based agents that are not merely shaped by their harnesses, but can also participate in reshaping them.

---

## 364. AlloSpatial: Agentic Harness Framework for Spatial Reasoning in Foundation Models

**Autori:** Shouwei Ruan, Bin Wang, Zhenyu Wu, Qihui Zhu, Yuxiang Zhang, Jingzhi Li, Yubin Wang, Xingxing Wei  
**Data:** 2026-06-08  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2606.08952v1

> Multimodal Foundation Models (MFMs) have made substantial progress, yet remain fragile in spatial reasoning over the physical world. A key bottleneck lies in their inability to transform local egocentric observations into a global allocentric spatial representation. To address this, we propose AlloSpatial, an agentic framework for allocentric spatial cognition in foundation models. AlloSpatial introduces World2Mind, a plug-and-play cognitive mapping sandbox that converts egocentric observations into structured allocentric priors, including Allocentric-Spatial Trees and route maps that support querying object topology, geometric relations, passability, and trajectories. To utilize these priors reliably under noisy reconstruction and ambiguous visual evidence, AlloSpatial introduces a Spatial Reasoning Harness for tool-use judgment, modality-decoupled cue collection, and geometry-semantic arbitration. We further internalize this process in Qwen3-VL through cold-start reinforcement learning with a harness-gated trajectory-level reward. Experiments on VSI-Bench and MindCube show that AlloSpatial improves proprietary models by 5%-18% in a training-free setting, while ASTs alone support strong spatial reasoning even when visual inputs are removed. The trained AlloSpatial agents further outperform larger general-purpose models and competitive spatial baselines, suggesting that structured allocentric representations, active tool use, and verifiable reasoning offer a promising route toward spatially capable foundation models.

---

## 365. PhysAgent: Automating Physics-Based 4D Synthesis via Trajectory-Grounded Multi-Agent Feedback

**Autori:** Chunji Lv, Jiaxi Ye, Yuchen Jiang, Rexar Lin, Changsheng Li  
**Data:** 2026-06-07  
**Categorie:** cs.RO, cs.CV  
**Link:** https://arxiv.org/abs/2606.08688v1

> Achieving fully automated, physically plausible 3D motion synthesis is a core objective in graphics and generative AI. However, configuring complex environmental force fields still relies entirely on manual expert intervention, creating a severe bottleneck for large-scale simulation data generation. Existing automated methods primarily focus on material optimization and exhibit severe modality gaps and technical flaws when applied to the vastly more complex force field optimization space: naive Large Language Models (LLMs) lack underlying simulation feedback, causing severe physical inaccuracies, while traditional Score Distillation Sampling (SDS) suffers from sluggish gradients, local optima entrapment, and a mathematical inability to dynamically switch discrete force fields. To address this, we propose PhysAgent, the first simulator-in-the-loop multi-agent framework that leverages multimodal inputs for automated, physically grounded 4D synthesis. By decoupling intrinsic materials from extrinsic dynamics, PhysAgent utilizes a Semantic Agent equipped with an externalized Force Field Skill module to master simulation rules and generate valid initializations. Subsequently, the Refine Agents, driven by Trajectory-Grounded Multi-Agent Feedback, leverage vision foundation models to extract dense point trajectories from rendered frames. By converting these explicit motion trajectories into structured textual descriptors, the agent harnesses LLM commonsense reasoning to execute zero-shot macroscopic leaps, effectively escaping local optima and dynamically switching discrete force fields. Extensive experiments demonstrate that PhysAgent rapidly generates stable, diverse physical scenes from arbitrary multimodal prompts, significantly outperforming existing baselines in both generation diversity and physical accuracy.

---

## 366. Bayesian-Agent: Posterior-Guided Skill Evolution Across LLM Agent Harnesses

**Autori:** Xiaojun Wu, Cehao Yang, Honghao Liu, Xueyuan Lin, Wenjie Zhang, Zhichao Shi, Xuhui Jiang, Chengjin Xu, Jia Li, Jian Guo  
**Data:** 2026-06-06  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2606.08348v2

> LLM agents increasingly rely on prompts, tools, memory, SOPs, skills, and harness feedback, yet current self-evolution pipelines often update these assets through heuristic reflection or raw success counts. Such updates are brittle when trajectories are sparse, expensive, and context-dependent. We introduce Bayesian-Agent, a native and cross-harness framework that treats reusable agent skills as Bayesian evidence objects. Bayesian-Agent records verified trajectories, maintains posterior beliefs over skill reliability and failure modes, and turns those beliefs into auditable skill actions and model-facing guardrails. This posterior view provides a finite-sample alternative to raw empirical-rate skill updates and frames prompt, context, and harness engineering as inference over the external decision environment. On RealFin-Bench, Bayesian skill evolution matches or improves the raw empirical-rate control and yields large gains on native runs. In the incremental mode, incremental repair improves SOP-Bench from 80\% to 95\%, Lifelong AgentBench from 90\% to 100\%, and RealFin-Bench from 45\% to 65\%. Backend and model-scaling ablations further show that posterior-guided repair can operate across BA native, MiniSWEAgent, and Claude Code, provided the harness produces verifiable task artifacts. The source code is available at https://github.com/DataArcTech/Bayesian-Agent.

---

## 367. VideoWeaver: Evaluating and Evolving Skills for Agentic Long Video Generation

**Autori:** Jianhui Wei, Yan Zhang, Jie Tan, Hengchuan Zhu, Xiaotian Zhang, Ziyi Chen, Daoan Zhang, Wei Xu, Yeying Jin, Zuozhu Liu  
**Data:** 2026-06-06  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2606.08091v2

> Agentic long video generation requires planning, tool orchestration, and cross-clip coordination over a long horizon. Most existing video agents either rely on static, human-crafted workflows, which require substantial manual effort and poorly adapt across tasks, or iteratively refine the output of the current task without persistently distilling execution experience into reusable skills for future tasks. We introduce VideoWeaver, an agent harness and benchmark that evaluates and evolves skills for long video generation. Given a single high-level instruction, an agent dynamically composes foundation skills into its own workflow rather than following a predefined pipeline. We construct a benchmark of 16 task categories and 285 cases, with references spanning text, image, audio, video, and their combinations. We further propose an evidence-grounded agent-as-judge that inspects both the execution trace and the final video to diagnose process and output failures. Based on this feedback, our evolution algorithm progressively refines category-level composition and creator skills, allowing recurring experience to guide dynamically constructed workflows for unseen cases. Experiments show that explicit composition skills improve the generation process over foundation skills alone, while skill evolution further improves output quality and generalizes to unseen cases. Incorporating judge feedback yields additional gains, especially on output metrics, and the agent-as-judge aligns well with human, particularly on process metrics. Code is available at https://github.com/JianhuiWei7/VideoWeaver.

---

## 368. Act As a Real Researcher: A Suite of Benchmarks Evaluating Frontier LLMs and Agentic Harnesses in Research Lifecycle

**Autori:** Jiayu Wang, Weijiang Lv, Bowen Fu, Jing Fu, Jiayi Song, Lingyu Zhang, Lanxuan Xue, Luodi Chen, Zepeng Xin, Kaiyu Li, Xiangyong Cao  
**Data:** 2026-06-05  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2606.07462v1

> As foundation models advance and agent scaffolding becomes increasingly sophisticated, agents have demonstrated remarkable proficiency in complex, long-horizon coding tasks and even autonomous experiment execution. Despite their evolution from research assistants into autonomous research agents, these systems still exhibit significant limitations in field sensitivity, research ethics, and nuanced scientific judgment. Consequently, frontier agents remain unable to fully replace human researchers. To bridge this gap, we conceptualize the AARR (Act As a Real Researcher) benchmark series. Unlike existing benchmarks that primarily assess macro-level execution capabilities, AARR focuses on whether agents can emulate the professionalism, thoroughness, and nuanced reasoning that characterize human researchers in granular research scenarios. In this work, we propose AARRI-Bench (Act As a Real Research Intern), the first benchmark in this series. We conduct extensive experiments across frontier models and agentic systems, revealing that even the best-performing configuration (Mini-SWE-Agent with Claude Opus 4.7) achieves only 68.3\% success rate, frequently overlooking subtle yet critical details that are obvious to real human researchers. Our results indicate that developing researcher-like AI requires further exploration of research behavior, rather than merely complex scaffolding. Our data is released at https://github.com/AARR-bench/AARRI-bench.

---

## 369. From Failed Trajectories to Reliable LLM Agents: Diagnosing and Repairing Harness Flaws

**Autori:** Mengzhuo Chen, Junjie Wang, Zhe Liu, Yawen Wang, Haiming Zheng, Qing Wang  
**Data:** 2026-06-04  
**Categorie:** cs.SE, cs.MA  
**Link:** https://arxiv.org/abs/2606.06324v2

> LLM agents increasingly rely on agent harness: the runtime infrastructure around the base model that defines execution environments, tool interfaces, context, lifecycle orchestration, observability, verification, and governance. Existing self-improving agents and automatic harness evolution methods mainly improve agents through runtime supervision, prompt optimization, workflow search, or harness modification based on final outcomes. However, they often fail to diagnose where the responsible evidence lies in failed trajectories and which harness implementation mechanism causes the unreliable behavior, resulting in broad, indirect, or poorly scoped changes. This paper proposes HarnessFix, a trace-grounded and diagnosis-driven framework for repairing agent harnesses. HarnessFix compiles raw execution traces and harness artifacts into a Harness-aware Trace Intermediate Representation (HTIR), which normalizes fragmented trajectory evidence, captures step-level data-flow and control-flow relations, and aligns runtime steps with the harness artifacts that shape their behavior. It then attributes failures to responsible steps and harness artifacts, and consolidates recurring diagnoses into repair-oriented flaw records. Finally, HarnessFix maps these records to scoped repair operators, generates patches under flaw-specific repair specifications, and accepts them through regression-aware validation. We evaluate HarnessFix on four popular benchmarks, and results show that it improves the performance over the initial harnesses by 6.3% to 18.4%, significantly outperforming human-designed and self-evolution baselines. HarnessFix highlights the value of treating failed trajectories not only as feedback signals, but also as structured evidence for diagnosing and repairing the harness mechanisms behind agent failures.

---

## 370. Evolving Agents in the Dark: Retrospective Harness Optimization via Self-Preference

**Autori:** Wenbo Pan, Shujie Liu, Chin-Yew Lin, Jingying Zeng, Xianfeng Tang, Xiangyang Zhou, Yan Lu, Xiaohua Jia  
**Data:** 2026-06-04  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2606.05922v3

> AI agents rely on a harness of skills, tools, and workflows to solve complex problems. Continually improving this harness is essential for adapting to new tasks. However, existing optimization methods typically require ground-truth validation sets, yet such labeled data is difficult to acquire in practical deployment settings. To address this problem, we introduce Retrospective Harness Optimization (RHO), a self-supervised method that optimizes the agent harness using only past trajectories. Specifically, RHO selects a diverse coreset of challenging tasks from past trajectories and re-solves them in parallel. The agent analyzes these rollouts using self-validation and self-consistency, then generates candidate harness updates and selects the most effective one by its own pairwise self-preference. We evaluate RHO across three diverse domains, spanning software engineering, technical work, and knowledge work. Notably, a single optimization round improves the pass rate on SWE-Bench Pro from 59% to 78% without any external grading. Furthermore, our analysis demonstrates that RHO effectively targets prior failure modes. As a result, the optimized harness alters the agent's behavior patterns and sustains higher accuracy during long-horizon sessions.

---

## 371. SciVisAgentSkills: Design and Evaluation of Agent Skills for Scientific Data Analysis and Visualization

**Autori:** Kuangshi Ai, Haichao Miao, Kaiyuan Tang, Shusen Liu, Chaoli Wang  
**Data:** 2026-06-04  
**Categorie:** cs.AI, cs.HC  
**Link:** https://arxiv.org/abs/2606.05525v1

> Recent advances in agentic visualization have enabled the translation of natural language into executable scientific visualization (SciVis) workflows. While general-purpose coding agents show strong capabilities, they often lack the tool-specific expertise required for SciVis tasks. In this work, we present SciVisAgentSkills, a collection of reusable agent skills that augment coding agents for scientific data analysis and visualization by encoding environment assumptions, tool usage patterns, and domain heuristics across scientific tools such as ParaView, napari, VMD, and TTK. We evaluate these skills on Codex and Claude Code using SciVisAgentBench, a benchmark of 108 expert-designed multi-step tasks. Results show that agent skills improve mean task scores across the evaluated suites, with token-efficiency benefits that depend on the agent harness and tool setting. These findings highlight the importance of structured procedural knowledge for enabling reliable, long-horizon SciVis workflows, while also showing that skills should be studied alongside the execution harness that loads and applies them. The skills are available at https://github.com/KuangshiAi/SciVisAgentSkills.

---

## 372. Harnessing Generalist Agents for Contextualized Time Series

**Autori:** Zihao Li, Kaifeng Jin, Yuanchen Bei, Jiaru Zou, Avaneesh Kumar, Xuying Ning, Yanjun Zhao, Mengting Ai, Baoyu Jing, Hanghang Tong, Jingrui He  
**Data:** 2026-06-03  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2606.05404v1

> Time series are often embedded in rich contexts that are essential for holistic modeling. Moreover, real-world practitioners often require end-to-end workflows for analyzing temporal dynamics, where widely studied tasks such as forecasting are only one step in a broader solution loop. While generalist AI agents offer a promising interface for such workflows under complex contexts, they still operate primarily in textual spaces that are not fully aligned with structured temporal signals. In this work, we introduce TimeClaw, an agentic harness framework for time series that equips generalist LLM agents with the time series-native runtime support needed for contextualized temporal reasoning. TimeClaw integrates executable temporal tools for grounded and auditable analysis, experience-driven capability evolution for creating reusable analytical routines, and episodic multimodal memory for retrieving relevant reasoning traces. Together, these components unlock harnessed open-ended temporal reasoning with contextual information. Extensive evaluation on multiple benchmarks covering diverse tasks across energy, finance, weather, traffic, and other real-world domains demonstrates improved performance of TimeClaw. Code is available at https://github.com/iDEA-iSAIL-Lab-UIUC/TimeClaw.

---

## 373. LeanMarathon: Toward Reliable AI Co-Mathematicians through Long-Horizon Lean Autoformalization

**Autori:** Yuanhe Zhang, Yuekai Sun, Taiji Suzuki, Jason D. Lee, Fanghui Liu  
**Data:** 2026-06-03  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2606.05400v1

> Long-horizon autoformalization of research mathematics fails not only at hard lemmas, but at scale: statements drift, dependencies tangle, context decays, and local repairs corrupt distant work. We present LeanMarathon, a multi-agent harness for reliable research-level Lean autoformalization. Its core abstraction is an evolving blueprint: a Lean file that serves simultaneously as formal proof skeleton, natural-language proof graph, and shared system of record. Four contract-scoped agents construct, audit, prove, and repair this blueprint. These agents are coordinated by a two-stage orchestrator that first stabilizes target fidelity through adversarial review and then discharges the proof directed acyclic graph (DAG) from its dynamic leaves upward in parallel CI-gated rounds. LeanMarathon turns one brittle multi-hour run into many local, recoverable, parallel transactions. We evaluate LeanMarathon on two recent research papers spanning four Erdős problems (#1051, #1196, #164, #1217). Across three autonomous runs, it formalizes all seven target theorems with no sorry, proving 258 lemmas and theorems. These results show that reliable AI co-mathematics requires not only stronger provers, but durable harnesses that preserve target fidelity across long mathematical developments. The code can be found at https://github.com/YuanheZ/LeanMarathon.

---

## 374. SentinelBench: A Benchmark for Long-Running Monitoring Agents

**Autori:** Matheus Kunzler Maldaner, Adam Fourney, Amanda Swearngin, Hussein Mozannar, Gagan Bansal, Maya Murad, Rafah Hosn, Saleema Amershi  
**Data:** 2026-06-03  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2606.05342v2

> AI agents are increasingly asked to carry out work that spans minutes, hours, or longer. Yet the default model of agent behavior is continuous action: issuing tool calls, refreshing pages, searching for alternatives, or otherwise trying to force progress. This is the wrong approach for many long-running tasks, which are better served by a strategy of sustained attention. Instead, agents should monitor an environment, notice when an external event makes progress possible, then respond promptly without wasting resources while waiting. To measure progress on this class of tasks, we introduce SentinelBench, an open-source benchmark for time-evolving monitoring tasks. SentinelBench contains 100 tasks across 10 synthetic web environments, including email, calendars, finance, professional networking, and entertainment. Each environment exposes a live web interface and replays a scripted sequence of events, requiring agents to navigate and reason about web pages whose state shifts underfoot. SentinelBench measures task completion, reaction time, and resource use, exposing the tradeoff between responsiveness and cost. We report results across three models and two browser-agent harnesses, establishing performance baselines for future comparison and demonstrating how agent design choices can dramatically impact key metrics. Together, these results show that SentinelBench distinguishes meaningful differences in agent behavior.

---

## 375. DAR: Deontic Reasoning with Agentic Harnesses

**Autori:** Guangyao Dou, William Jurayj, Nils Holzenberger, Benjamin Van Durme  
**Data:** 2026-06-03  
**Categorie:** cs.CL, cs.AI  
**Link:** https://arxiv.org/abs/2606.05009v1

> Deontic reasoning is the task of answering questions by applying explicit rules and policies to case-specific facts, for example computing tax liability under a statute or determining the outcome of an immigration appeal. A key technical challenge for LLM-based deontic reasoning is that the relevant ruleset can be long and cross-referenced, so models may still fail to locate the rules needed for a particular reasoning step. We introduce Deontic Agentic Reasoning (DAR), an agentic reasoning setup in which the model interacts with the statutes on demand. We evaluate DAR under multiple harnesses on hard subsets of DeonticBench. Across these settings, we find that agentic harnesses can push the frontier on deontic reasoning tasks, but improvements are not uniform: weaker models often degrade on numerical tasks while consuming far more tokens.

---

## 376. Exploring Cross-Scenario Generality of Agentic Memory Systems: Diagnostics and a Strong Baseline

**Autori:** Zhikai Chen, Jialiang Gu, Junyu Yin, Xianxuan Long, Shenglai Zeng, Xiaoze Liu, Kai Guo, Keren Zhou, Jiliang Tang  
**Data:** 2026-06-03  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2606.04315v1

> LLM agents accumulate histories that outgrow their context windows, motivating a growing literature on memory systems. Yet most existing designs are tuned to a single scenario (multi-session chat or a single trajectory format), and there is little evidence that they generalize across the heterogeneous trajectories agents encounter in deployment. We revisit eight memory systems plus an agentic harness for search problems, on five scenarios: single-turn QA, multi-session chat, agentic-trajectory QA, memory stress tests, and long-horizon agentic tasks. The harness, which self-manages flat text-file storage via tool calls, achieves the best cross-task ranking, suggesting that memory performance hinges on giving the agent active control over storage and retrieval rather than on a passive store behind a fixed pipeline. We instantiate this insight in AutoMEM, an agentic memory harness with a self-managed tool interface that achieves the best cross-scenario generality among the systems we evaluate.

---

## 377. Kernel Forge: An Agent Harness for LLM-based Generation and Optimization of CUDA Kernels

**Autori:** Joshua Brodsky, Dhravid Kumar, Savini Kashmira, Jayanaka Danatanarayana, Jason Mars, Krisztian Flautner, Lingjia Tang  
**Data:** 2026-06-02  
**Categorie:** cs.AI, cs.PF  
**Link:** https://arxiv.org/abs/2607.24762v1

> Machine learning models are increasingly embedded in everyday software, and most of their runtime is spent in a small set of compute kernels such as matrix multiplication, convolution, and normalization. Optimizing these kernels is one of the most direct ways to reduce latency and cost, but it has traditionally required expert engineers to hand-write low-level GPU code. Agentic systems built on large language models (LLMs) can now generate and optimize kernels with far less human effort, yet existing tools are largely evaluated on randomly generated tensors and isolated kernels, emit standalone CUDA code that developers must manually reintegrate, mostly target only LLM PyTorch models, and offer limited support for inspecting and debugging results. We present Kernel Forge, an open-source, end-to-end agentic harness that accepts any unmodified PyTorch model in place. Kernel Forge supports vision, diffusion, and LLM workloads, uses Monte Carlo Tree Search (MCTS) to explore multiple optimization paths rather than a single linear refinement chain, and ships with a graphical user interface for monitoring progress, inspecting candidate kernels, and debugging failures. We evaluate Kernel Forge on four PyTorch models spanning vision, diffusion, and LLM workloads on an NVIDIA DGX Spark with GB10 GPU. With only 50 optimization iterations per kernel, it optimizes 14 kernels to outperform PyTorch eager mode, reaching $1.52\times$ on adaptive\_avgpool2d in ResNet-50, $1.70\times$ on group\_norm in Stable Diffusion 3.5 Medium, $2.83\times$ on softmax in Gemma 4 E2B, and $1.54\times$ on softmax in Qwen 3.5 35B-A3B.

---

## 378. MUSE: A Unified Agentic Harness for MLLMs

**Autori:** Jianglin Lu, Hailing Wang, Xu Ma, Qihua Dong, Mingyuan Zhang, Yizhou Wang, Yun Fu  
**Data:** 2026-06-02  
**Categorie:** cs.CV, cs.AI  
**Link:** https://arxiv.org/abs/2606.03005v1

> Despite rapid progress, multimodal large language models (MLLMs) still fail on tasks that humans solve effortlessly, such as navigating a grid maze from a screenshot or selecting the correct puzzle piece. Rather than retraining the model, we ask a complementary question: how much capability can be elicited from a frozen MLLM purely by improving the execution scaffold around it? We introduce MUSE, a multimodal unified structured execution harness that wraps any off-the-shelf MLLM with composable modules for task representation, visual processing, perception tool use, structured parsing, deterministic verification, and verifier-guided repair, without any model retraining. We evaluate MUSE across diverse benchmarks spanning visual spatial planning, visual perception, multimodal reasoning, and fine-grained visual discrimination, using multiple state-of-the-art MLLMs. MUSE delivers consistent gains over the bare model in all settings, with the largest jumps on challenging instances. Further analysis reveals that many MLLM failures arise from harness-level shortcomings rather than fundamental model deficits, and can be addressed through verifier-guided repair without touching the model. These findings highlight the agentic multimodal harness as a critical yet underexplored design dimension, offering an orthogonal avenue for improving MLLMs beyond model-centric optimization.

---

## 379. DS-Lighting: Making Agent Harnesses Explicit for Data-Science Automation

**Autori:** Fan Liu, Hao Liu  
**Data:** 2026-06-01  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2608.28590v1

> Large Language Model (LLM) agents have shown promise for automating data-science workflows, yet their end-to-end performance depends critically on the agent harness that represents tasks, manages execution state, constrains output artifacts, and provides evaluation feedback. Existing data-science agents often leave this harness implicit, making results difficult to reproduce, compare, and attribute across heterogeneous tasks. We introduce DS-Lighting, a unified harness toolkit that makes harness design explicit for data-science automation. DS-Lighting decomposes the harness into four reusable layers: data, workflow, execution, and evaluation, and represents diverse agents as executable operator programs that support both predefined pipelines and adaptive search. We further integrate multiple open-source data-science benchmarks into an MLE-Bench-style task format, enabling controlled comparison under a shared task interface, sandboxed runtime, and metric protocol. Experiments across agents, harnesses, models, and ablations show that explicit harness design improves reproducibility, comparability, and reliability, while reducing avoidable system-level failures in end-to-end data-science workflows. Our code is available at https://github.com/usail-hkust/dslighting

---

## 380. SkillAdaptor: Self-Adapting Skills for LLM Agents from Trajectories

**Autori:** Zhuoyun Yu, Xin Xie, Wuguannan Yao, Chenxi Wang, Lei Liang, Xiang Qi, Shumin Deng  
**Data:** 2026-05-31  
**Categorie:** cs.CL, cs.AI, cs.LG, cs.MA  
**Link:** https://arxiv.org/abs/2606.01311v1

> Large language model (LLM) agents increasingly rely on reusable external skills to solve long-horizon interactive tasks. Existing training-free skill adaptation pipelines usually update skills from full trajectories or session-level feedback, which makes failure attribution coarse and often produces unstable or overly broad revisions. We propose SkillAdaptor, a training-free step-level skill adaptation framework with explicit failure attribution, and it can plug into OpenClaw-class agent harnesses. Given a failed trajectory, SkillAdaptor identifies a first actionable fault step, links responsibility to candidate skills, and applies targeted updates under explicit acceptance checks while keeping the backbone frozen. We evaluate on WebShop, PinchBench, and Claw-Eval with Kimi-K2.5, GLM-5, and GPT-5.2. SkillAdaptor improves over no-skill and skill-adaptation baselines on all three suites, with the largest single-metric improvements of +1.5 points on PinchBench Avg Score%, +1.8 on Claw-Eval Avg Score, and +1.7 on WebShop success rate. These results indicate that step-level attribution supports more stable and auditable training-free skill maintenance\footnote{The code will be released at https://github.com/zjunlp/SkillAdaptor.}.

---

## 381. Leyline: KV Cache Directives for Agentic Inference

**Autori:** Bole Ma, Jan Eitzinger, Harald Koestler  
**Data:** 2026-05-31  
**Categorie:** cs.DC, cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2606.01065v1

> Modern KV cache management assumes the chatbot workload: prompts arrive once and the cache grows append-only, so prefix caching and forward-only eviction are correct by construction. Agentic LLMs break this assumption. Their conversations evolve through policy-driven editing: failed tool calls are retried, stale outputs dropped, trajectories pivoted. Two distinct cache problems result. First, identical content moves to new positions between turns, invalidating exact-prefix caches even though the underlying KV would still be valid; recent work on position-independent caching for MLA addresses this reuse problem. Second, and this paper's focus, a policy may need to direct the serving system to actively remove or replace a span of cached content and continue without re-prefilling everything that came after. No existing primitive offers this. Production agentic harnesses fall back to re-prefill on every edit, paying full prefix-recomputation cost; kernel-level eviction methods make their own decisions and cannot accept policy directives from outside the kernel. We introduce Leyline, a serving-side primitive that closes this gap. A declarative directive 4-tuple separates what to edit from how to preserve position correctness. The policy declares the edit and its mode (in-place splice or prefix-trimmed re-prefill for semantic forgetting); an architecture-agnostic interface routes to a per-architecture kernel that restores attention math via a closed-form RoPE-rotation correction. The splice kernel lifts replay cache-hit by +11.2 pp and cuts latency by up to 241 ms. A ten-line truncation rule routed through the same interface lifts agentic solve rate by +14.3 pp on debug-gym. The mechanism is open; the policy space it enables is the agenda.

---

## 382. From Prompt Injection to Persistent Control: Defending Agentic Harness Against Trojan Backdoors

**Autori:** Jiejun Tan, Zhicheng Dou, Xinyu Yang, Yuyang Hu, Yiruo Cheng, Xiaoxi Li, Ji-Rong Wen  
**Data:** 2026-05-29  
**Categorie:** cs.CR, cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2605.31042v1

> LLM agents are evolving from conversational chatbots to operational tools in real-world workspaces. In local agentic harnesses, an LLM can read and write files, call tools, and reuse workspace state across sessions. While such capabilities enhance utility, they also expose a new attack surface for attackers. Attackers can embed a prompt injection within a file or tool output. Agents may read this hidden instruction, store it, and execute it later. In this multi-step trojan attack paradigm, no individual step appears malicious on its own, but these steps can collectively turn untrusted text into persistent control content. However, existing defenses often inspect each step in isolation. As a result, they can block a clear harmful action, but fail to detect the earlier write operation that plants the backdoor. To reveal this threat, we introduce ClawTrojan, a benchmark designed to identify multi-step trojan attacks in local agentic harnesses. In an OpenClaw-style simulated workspace with GPT-5.4, ClawTrojan reaches a 95.5% attack success rate (ASR), while existing single-turn prompt-injection attacks produce near-zero ASR on the same model. To address this threat, we propose DASGuard, which scans control-like text in sensitive local files, traces its origin, and removes control content that does not originate from a trusted source. Our results show that DASGuard achieves strong dynamic defense by combining runtime attack blocking with sanitized commits to the workspace.

---

## 383. Crafter: A Multi-Agent Harness for Editable Scientific Figure Generation from Diverse Inputs

**Autori:** Haozhe Zhao, Shuzheng Si, Zhenhailong Wang, Zheng Wang, Liang Chen, Xiaotong Li, Zhixiang Liang, Maosong Sun, Minjia Zhang  
**Data:** 2026-05-28  
**Categorie:** cs.CV, cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2605.30611v1

> Scientific figures are among the most effective means of communicating complex research ideas, yet producing publication-quality illustrations remains one of the most labor-intensive parts of paper preparation. Existing automated systems each target a single figure type under text-only input, leaving the diversity of types and conditions researchers actually use unaddressed; their raster outputs further cannot be locally revised. Because scientific figures are structured compositions of discrete semantic components, the localized errors generators produce on such layouts demand not a stronger backbone but a harness. We instantiate this harness in two complementary systems: Crafter, a multi-agent harness for figure generation that generalizes across figure types and input conditions without architectural changes, and CraftEditor, which applies the same pattern to convert raster outputs into editable SVGs. Moreover, we introduce CraftBench, a benchmark spanning three figure types and four input conditions with human quality annotation. Experiments show that Crafter substantially outperforms both standalone generators and the agentic baseline on PaperBanana-Bench and CraftBench, with ablations confirming each component's independent contribution; CraftEditor faithfully converts outputs into editable SVGs that surpass all baselines. Our code and benchmark are available at https://github.com/HaozheZhao/Crafter.

---

## 384. Syll: Open-Source Personal Automation with Cross-Surface Execution

**Autori:** Bo Zhang, Borui Zhang, Chenghao Jiang, Minglei Shi, Xiaofeng Wang, Zheng Zhu, Jie Zhou, Jiwen Lu  
**Data:** 2026-05-28  
**Categorie:** cs.AI, cs.HC, cs.LG, cs.SE  
**Link:** https://arxiv.org/abs/2606.07594v1

> Personal AI agents must increasingly operate across APIs, shells, web surfaces, and desktop GUIs, yet many systems remain tuned to a single interface and offer limited support for user teaching and auditability. We present Syll, an open-source, self-hosted multimodal agent harness that unifies MCP/API tools, CLI execution, and visual GUI control in a modular runtime, enabling agents to coordinate computer use across heterogeneous interfaces while streamlining how users and agents exchange information. At the core of Syll is a bidirectional user-agent interaction layer: users teach procedures through direct demonstration, which Syll compiles into reusable skills; agent execution is translated back into multimodal evidence -- logs, keyframes, and approval checkpoints -- for inspection and control. Syll further externalizes memory, skills, routines, and governance as editable local artifacts, supporting straightforward inspection, extension, and downstream development. Our implementation has been validated on production desktop applications including Adobe Photoshop, Adobe Audition, Stardew Valley, macOS Finder and others. We report mechanism-oriented studies that validate multimodal routing, teachable GUI replay, and persistent local artifacts. We hope Syll can serve as a practical open-source foundation for personal automation that users can teach, inspect, and continuously extend.

---

## 385. Towards Verifiable Multimodal Deep Research: A Multi-Agent Harness for Interleaved Report Generation

**Autori:** Chenghao Zhang, Guanting Dong, Yufan Liu, Tong Zhao, Xiaoxi Li, Zhicheng Dou  
**Data:** 2026-05-28  
**Categorie:** cs.CL, cs.AI  
**Link:** https://arxiv.org/abs/2605.29861v2

> Large Language Models (LLMs) have advanced autonomous agents from deep search, which retrieves concise factual answers, to deep research, which synthesizes scattered evidence into long-form reports. However, verifiable multimodal deep research remains challenging due to open-ended synthesis without deterministic ground truth and the need to interleave textual arguments with visual evidence. We propose Ptah, a multi-agent harness for interleaved report generation. Ptah orchestrates the lifecycle from user query to rendered web report through planning, research, and writing stages, where specialized agents construct visual-aware plans, collect claim-grounded evidence, maintain source-aligned images in a Visual Working Memory, and compose reports through declarative multimodal tool use. A verifier agent serves as the harness's acceptance function, enforcing factual grounding, citation fidelity, and cross-modal consistency throughout the workflow. We further introduce PtahEval, an evaluation protocol that augments existing benchmarks with image-level and presentation-level assessments. Experiments on deep research benchmarks show that Ptah produces more reliable, visually informative, and usable human-facing multimodal reports than strong baselines. Our code is released at https://github.com/SnowNation101/Ptah

---

## 386. Scaling Laws for Agent Harnesses via Effective Feedback Compute

**Autori:** Xuanliang Zhang, Dingzirui Wang, Keyan Xu, Qingfu Zhu, Wanxiang Che  
**Data:** 2026-05-28  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2605.29682v2

> Agent harnesses shape language-model performance by controlling tool use, feedback, verification, memory, and repair. Yet raw test-time expenditure, such as tokens, tool calls, wall time, or cost, cannot distinguish useful feedback from redundant or unstable interaction. We introduce \emph{Effective Feedback Compute} (EFC), a trace-level scaling coordinate for informative, valid, non-redundant, and retained feedback. We further define Estimated-EFC, NRS-EFC, harness efficiency $η$, and task-demand normalization for realistic traces and heterogeneous tasks. Across synthetic, real, held-out, and prospective evaluations, EFC-based coordinates outperform raw-compute baselines and SAS. Oracle-EFC/$D_{\mathrm{task}}$ reaches $R^2=0.99$ in controlled scaling, and NRS-EFC/$D_{\mathrm{task}}$ reaches $R^2=0.93$ on real traces where raw compute has near-zero or negative fit. Finally, \ours uses EFC as a companion control layer for existing harnesses, improving mean pass rate from $61.2\%$ to $68.2\%$ while reducing mean raw cost from $213.8$ to $85.1$ under matched settings. These results suggest that harness scaling depends on durable, task-sufficient feedback rather than raw computation alone.

---

## 387. WorldMemArena: Evaluating Multimodal Agent Memory Through Action-World Interaction

**Autori:** Chengzhi Liu, Yuzhe Yang, Sophia Xiao Pu, Yepeng Liu, Lin Long, Yichen Guo, Nuo Chen, Zhaotian Weng, Elena Kochkina, Simerjot Kaur, Charese Smiley, Xiaomo Liu, James Zou, Sheng Liu, Yuheng Bu, Songyou Peng, Xin Eric Wang  
**Data:** 2026-05-28  
**Categorie:** cs.CV, cs.CL  
**Link:** https://arxiv.org/abs/2605.29341v2

> Multimodal large language models are increasingly deployed as long-horizon agents, where memory must do more than recall: it must track an evolving world, revise what has gone stale, and surface the right evidence at decision time. Existing benchmarks measure recall over static dialogue, collapse memory into a single end-of-task accuracy, and reduce visual observations to captions, leaving us unable to localize failures to writing, maintenance, retrieval, or use. The rise of agent harnesses that author their own memory sharpens this gap, since we have no principled way to compare hand-designed pipelines with self-managing alternatives. To close these gaps, we formulate multimodal agent memory as an Action-World Interaction Loop with an observable four-stage lifecycle, and instantiate it in WorldMemArena: 400 multi-session multimodal tasks spanning Lifelong Evolution (evolving personal and task states) and Agentic Execution (memory from real observations, actions, and feedback), annotated with gold memory points, updates, distractors, and evidence chains for stage-level diagnosis. This enables the first head-to-head comparison of long-context, manually designed (RAG and external memory systems), and harness-based memory agents. Results show that: (1) better memory writing and storage do not guarantee better performance; (2) multimodal memory still struggles to fully use visual evidence; (3) systems are unstable across domains and degrade on realistic agentic trajectories; and (4) harness memory is more flexible but remains costly and less reliable.

---

## 388. T2J-BENCH: Benchmarking Coding Agents on Execution-Grounded PyTorch-to-JAX Repository Migration

**Autori:** Tao Feng, Jiefeng Chen, Linxin Song, Yufan Zhuang, Yue Huang, Bhavana Dalvi Mishra, Chi Wang, Xiangru Tang, Jieyu Zhao, Ge Liu, Tomas Pfister, Jinsung Yoon  
**Data:** 2026-05-27  
**Categorie:** cs.SE, cs.CL  
**Link:** https://arxiv.org/abs/2605.29054v3

> Migrating a machine-learning codebase across frameworks--for example from PyTorch to JAX--is a routine but costly engineering task that is fundamentally cross-paradigm: eager, stateful, object-oriented modules must be rewritten as pure, jittable functions over an explicit parameter pytree. We ask whether coding agents can perform such whole-repository migrations correctly, and argue that existing code benchmarks, which grade unit-test pass rates or surface-level similarity to a reference translation, cannot answer this: they neither require the migrated system to \emph{behave} the same nor prevent a JAX reimplementation from faking equivalence by secretly importing PyTorch itself. We introduce T2J-BENCH, a benchmark of 63 whole-repository PyTorch-to-JAX migration tasks spanning 18 model families across both training and serving, where torch-free checkpoint conversion is itself part of the deliverable. T2J-BENCH grades execution-grounded functional equivalence: each candidate is run inside a separate, torch-free, offline verifier and scored against references frozen from the PyTorch original, under a hard independence gate and a continuous, threshold-free reward. Across twenty off-the-shelf agent--model configurations, the strongest recovers only 0.676 of the reward against a 0.980 oracle, with substantial numeric and behavioral divergence despite high spec pass rates. Finally, we contribute TWINHARNESS, a reference-grounded agent harness that turns the agent's executable PyTorch source into legitimate self-verification feedback; applied to an opus-5 agent it raises the reward from 0.649 to 0.723--the highest of any configuration--using only task-visible resources.

---

## 389. Harness-Bench: Evaluating Agent Harnesses across Models and Realistic Workflows

**Autori:** Yilun Yao, Xinyu Tan, Chao-Hsuan Liu, Yaoming Li, Zhengyang Wang, Zongwei Lv, Wenhan Yu, Zhewen Tan, Yuxuan Tian, Lin Sun, Xiangzheng Zhang, Guangxiang Zhao, Tong Yang  
**Data:** 2026-05-27  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2605.27922v2

> LLM agents are increasingly deployed as executable systems that use tools, modify workspaces, and produce concrete artifacts. In such workflows, performance depends not only on the base model, but also on the harness: the system layer that manages context, tools, state, constraints, permissions, tracing, and recovery. However, existing benchmarks typically abstract away execution, compare complete agent systems, or hold the harness fixed, making execution-layer variation difficult to study. We introduce Harness-Bench, a diagnostic benchmark for evaluating configuration-level harness effects in realistic agent workflows. Harness-Bench evaluates representative harness configurations across multiple model backends under shared task environments, budgets, and evaluation protocols, while preserving each harness's native execution behavior. The benchmark contains 106 sandboxed offline tasks constructed from practical agent-use patterns and manually reviewed for realism, solvability, oracle-checkability, and integrity. Each run records final artifacts, execution traces, usage statistics, and validator outputs, enabling analysis beyond final completion. Across 5,194 execution trajectories, we observe substantial variation in completion, process quality, efficiency, and failure behavior across model-harness pairings. These results suggest that agent capability should be reported at the model-harness configuration level rather than attributed to the base model alone. Our analysis further identifies recurring execution-alignment failures, where plausible reasoning becomes decoupled from tool feedback, workspace state, evidence, or verifiable output contracts. Harness-Bench provides a reproducible foundation for diagnosing and improving reliable, efficient, and auditable agent execution stacks.

---

## 390. VibeSearchBench: Benchmarking Long-horizon Proactive Search in the Wild

**Autori:** Xiaohongshu Inc  
**Data:** 2026-05-27  
**Categorie:** cs.CL, cs.AI  
**Link:** https://arxiv.org/abs/2605.27882v2

> LLM-based agents score well on search benchmarks, yet real users consistently find results unsatisfying, revealing a persistent evaluation-experience gap. We attribute this gap to existing benchmarks' reliance on over-specified queries, single-turn interactions, and fixed-schema evaluation, none of which reflect real search behavior where users and agents collaboratively refine vague intent through multi-turn dialogue. We term this paradigm VibeSearch and introduce VibeSearchBench, a benchmark comprising 200 manually curated bilingual (Chinese and English) tasks across 20 domains, split into VibeSearch-Pro (professional) and VibeSearch-Daily (daily-life) subsets. Each task pairs a user persona with a schema-free ground-truth knowledge graph, and is evaluated through a progressive-disclosure user simulator and a graph-matching evaluation framework. We benchmark seven frontier models under both the ReAct framework and the OpenClaw agent harness. Results show that all models remain substantially inadequate for VibeSearch (best F1: 30.30), highlighting the need for fundamental advances in long-context reasoning, proactive intent elicitation, and structured knowledge construction.

---

## 391. Governed Evolution of Agent Runtimes through Executable Operational Cognition

**Autori:** Mariano Garralda-Barrio  
**Data:** 2026-05-26  
**Categorie:** cs.SE, cs.AI, cs.MA  
**Link:** https://arxiv.org/abs/2605.27328v1

> Recent advances in agentic systems increasingly treat code as an executable operational substrate rather than as a disposable output artifact. Prior work such as \emph{Code as Agent Harness} frames validated agent-generated artifacts as runtime entities that can be created, executed, revised, persisted, and reused within long-running cognitive loops. However, the governance, lifecycle management, and operational evolution of such artifacts remain under-specified. This paper proposes a framework for governed runtime evolution in multi-agent systems through executable operational cognition. We formalize agent-generated artifacts as persistent runtime capabilities that progressively become part of the operational substrate rather than transient intermediate outputs. Building on this perspective, we introduce \emph{HarnessMutation} as a governed mechanism for lifecycle-aware runtime adaptation operating under explicit validation, traceability, evaluation, and rollback constraints. Rather than treating runtime adaptation as unrestricted self-modification, the proposed framework models evolution as a bounded and observable process over persistent operational memory. It further shows how these ideas can be operationalized over modern agent runtimes and governance-oriented orchestration systems, providing a conceptual foundation for adaptive infrastructures whose evolution remains explicit, auditable, and constrained.

---

## 392. Your Agents Are Aging Too: Agent Lifespan Engineering for Deployed Systems

**Autori:** Jianing Zhu, Yeonju Ro, John Robertson, Kevin Wang, Junbo Li, Haris Vikalo, Aditya Akella, Zhangyang Wang  
**Data:** 2026-05-25  
**Categorie:** cs.AI, cs.CL, cs.MA  
**Link:** https://arxiv.org/abs/2605.26302v1

> Long-lived AI agents are increasingly deployed as persistent operational systems, yet they are still evaluated like freshly initialized models. Day-one benchmarks miss a basic systems question: how long does an agent remain reliable after deployment? Even when model weights are frozen, an agent's effective state keeps changing as it compresses interaction history, retrieves from a growing memory store, revises facts after updates, and undergoes routine maintenance. Reliability therefore becomes a lifespan property of the full agent harness, not only a snapshot property of the base model. We introduce AgingBench, a longitudinal reliability benchmark for agent lifespan engineering: measuring not only whether deployed agents degrade, but what form the degradation takes and where repair should target. AgingBench organizes agent aging into four mechanisms: compression aging, interference aging, revision aging, and maintenance aging. To diagnose these failures, AgingBench uses temporal dependency graphs and paired counterfactual probes that produce diagnostic profiles for the write, retrieval, and utilization stages of the memory pipeline. Across 7 scenarios, 14 models, multiple memory policies, and both runner-controlled and autonomous agents, over ~400 runs spanning 8 - 200 sessions show that agent aging is not one-dimensional: behavioral tests can remain clean while factual precision decays; derived-state tracking can collapse sharply within a single model; and the same wrong answer can require different repairs depending on what the diagnostic profile points to. These results suggest that reliable agent deployment requires lifespan evaluation, mechanism-level diagnosis, and stage-targeted repair, not only stronger day-one models.

---

## 393. From Model Scaling to System Scaling: Scaling the Harness in Agentic AI

**Autori:** Shangding Gu  
**Data:** 2026-05-25  
**Categorie:** cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2605.26112v1

> This paper studies the next major bottleneck in agentic AI as system scaling, not only model scaling: the design of auditable, persistent, modular, and verifiable architectures around foundation models. We refer to this shift as scaling the harness: treating the structured execution layer around a foundation model as a first-class object of design, evaluation, and optimization. Although recent large language models enable agents to use tools, retrieve information, maintain memory, and execute long-horizon workflows, evaluation remains largely model-centric, often reducing agents to final-task success while treating memory, retrieval, tool use, orchestration, verification, and governance as secondary implementation details. This framing is increasingly inadequate because agent performance emerges from the interaction among the foundation model, memory substrate, context constructor, skill-routing layer, orchestration loop, and verification-and-governance layer. Together, these components form the agent harness, which translates model capability into long-horizon agent behavior. We study scaling the harness through three core bottlenecks: context governance, trustworthy memory, and dynamic skill routing, together with the orchestration and governance mechanisms that coordinate and constrain them. We further outline a research agenda for harness-level benchmarks that go beyond one-shot task success to measure trajectory quality, memory hygiene, context efficiency, communication fidelity, verification cost, and safe evolution over time. To make the discussion concrete, we develop CheetahClaws: https://github.com/SafeRL-Lab/cheetahclaws, a Python-native reference harness, and compare it with Claude Code and OpenClaw. Our main claim is that future progress in agentic AI will depend as much on system design as on stronger foundation models.

---

## 394. PolyGnosis 2.0: Enhancing LLM Reasoning via Agentic Harness Engineering for Polymarket and OSINT Insight Extraction

**Autori:** Daren Wang, Hong Xu, Jiawen Xian  
**Data:** 2026-05-25  
**Categorie:** cs.CL, cs.CE  
**Link:** https://arxiv.org/abs/2605.25958v1

> This paper introduces PolyGnosis 2.0, a pioneering multi-agent architecture designed to extract predictive intelligence by synthesizing Polymarket anomaly signals with global Open Source Intelligence (OSINT) streams, specifically Global Database of Events, Language, and Tone (GDELT). We define and target "Perspective Mismatches", the narrative divergence between Polymarket sentiment and global media flows, as high-alpha trading signals. Moving beyond generic agentic superiority, we rigorously quantify the efficacy of "Harness Engineering" techniques, including reflection loops, tool-calling, divide-and-conquer partitioning (D&C), and chain-of-thought (CoT), within high-noise financial domains. Our empirical evaluation against human-expert benchmarks reveals that while structural partitioning is mandatory for multi-dimensional alignment, unconstrained terminal reflection actively induces logical drift. Furthermore, we identify a pervasive "consensus bias" across all agent configurations during narrative reasoning, necessitating deterministic validation. Ultimately, we isolate a Pareto-optimal configuration that achieves professional-grade analytical precision while minimizing latency and token overhead, providing a robust blueprint for autonomous intelligence in prediction markets.

---

## 395. SkillEvolBench: Benchmarking the Evolution from Episodic Experience to Procedural Skills

**Autori:** Yingtie Lei, Zhongwei Wan, Jiankun Zhang, Samiul Alam, Zixuan Zhong, Peizhou Huang, Xin Wang, Jingxuan Zhang, Donghao Zhou, Yunta Hsieh, Zhihao Dou, Hui Shen, Yan Xu, Dimitrios Dimitriadis, Tuo Zhang, Mi Zhang  
**Data:** 2026-05-22  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2605.24117v1

> Large language model (LLM) agents accumulate rich episodic trajectories while solving real-world tasks, but it remains unclear whether such experience can be distilled into reusable procedural skills. We introduce SkillEvolBench, a diagnostic benchmark for evaluating this step from experience reuse to skill formation. It contains 180 tasks across six real-world agent environments, organized into role-conditioned task families with shared latent procedures. Agents learn from acquisition tasks, update an external skill library using compacted trajectories and verifier feedback, and then face frozen deployment tasks testing context shift, adversarial shortcuts, and composition. By comparing self-generated and curated-start skill evolution against no-skill and raw-trajectory controls, SkillEvolBench separates procedural abstraction from base capability, curated prior knowledge, and direct reuse of episodic traces. Across ten model configurations and three agent harnesses, we find that current agents often adapt locally but rarely form robust reusable skills. Skill-based conditions can improve acquisition or replay, and individual models sometimes gain on specific deployment axes, but these gains are unstable under frozen deployment. Raw-trajectory reuse frequently outperforms distilled skills, suggesting that current abstraction procedures discard contextual and procedural cues that remain useful for future tasks. Capacity and cost analyses further show that writing more skills or larger Tier-3 resource libraries is not sufficient: additional updates can improve coverage while introducing episode-specific drift and procedural clutter. These findings position SkillEvolBench as a testbed for measuring when one-off experience becomes durable procedural knowledge rather than task-local memory.

---

## 396. MOSS: Self-Evolution through Source-Level Rewriting in Autonomous Agent Systems

**Autori:** Qianshu Cai, Yonggang Zhang, Xianzhang Jia, Huajiang Zheng, Wei Xue, Jun Song, Xinmei Tian, Yike Guo  
**Data:** 2026-05-21  
**Categorie:** cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2605.22794v2

> Autonomous agentic systems are largely static after deployment: they do not learn from user interactions, and recurring failures persist until the next human-driven update ships a fix. Self-evolving agents have emerged in response, but all confine evolution to text-mutable artifacts -- skill files, prompt configurations, memory schemas, workflow graphs -- and leave the agent harness untouched. Since routing, hook ordering, state invariants, and dispatch live in code rather than in any text artifact, an entire class of structural failure is physically unreachable from the text layer. We argue that source-level adaptation is a fundamentally more general medium: it is Turing-complete, a strict superset of every text-mutable scope, takes effect deterministically rather than through base-model compliance, and does not erode under long-context drift. We present MOSS, a system that performs self-rewriting at the source level on production agentic substrates. Each evolution is anchored to an automatically curated batch of production-failure evidence and proceeds through a deterministic multi-stage pipeline; code modification is delegated to a pluggable external coding-agent CLI while MOSS retains stage ordering and verdicts. Candidates are verified by replaying the batch against the candidate image in ephemeral trial workers, then promoted via user-consent-gated, in-place container swap with health-probe-gated rollback. On OpenClaw, MOSS lifts a four-task mean grader score from 0.25 to 0.61 in a single cycle without human intervention.

---

## 397. Toward AI VIS Co-Scientists: A General and End-to-End Agent Harness for Solving Complex Data Visualization Tasks

**Autori:** Haichao Miao, Zhimin Li, Kuangshi Ai, Kaiyuan Tang, Chaoli Wang, Peer-Timo Bremer, Shusen Liu  
**Data:** 2026-05-20  
**Categorie:** cs.AI, cs.HC  
**Link:** https://arxiv.org/abs/2605.21825v1

> The ability to inspect, interpret, and communicate complex data is crucial for virtually any scientific endeavor, but often requires significant expertise outside the core domain ranging from data management and analysis to visualization design and implementation. We present an end-to-end agentic harness that, based on only the data and a high level description of the tasks, independently designs custom visual analysis applications (VIS apps). This represents an important step towards a general AI co-scientist envisioned by many as an autonomous system that can autonomously execute long horizon tasks based on high-level directions. Our proposed VIS co-scientist is an essential component of this broader AI co-scientist vision: a harness that can autonomously analyze data and design visualization solutions using a collection of agents and specialized skills that coordinate exploratory analysis, plan, configure the environment, implement, validate the interface, and most importantly evaluate the overall task completion. Each stage produces document and instruction artifacts that guide downstream work and enable iterative refinement. We validate this approach on IEEE SciVis Contests spanning multiple science and engineering fields. These contests serve as ideal proving grounds because they encode real-world complexity: ambiguous requirements, diverse data modalities, design trade-offs, and task-driven validation. Given only the data and target tasks, our system autonomously produces functional single-page VIS Apps with verified linked-view behavior, highly customized to domain experts' specified tasks and needs.

---

## 398. Code as Agent Harness

**Autori:** Xuying Ning, Katherine Tieu, Dongqi Fu, Tianxin Wei, Zihao Li, Yuanchen Bei, Jiaru Zou, Mengting Ai, Zhining Liu, Ting-Wei Li, Lingjie Chen, Yanjun Zhao, Ke Yang, Bingxuan Li, Cheng Qian, Gaotang Li, Xiao Lin, Zhichen Zeng, Ruizhong Qiu, Sirui Chen, Yifan Sun, Xiyuan Yang, Ruida Wang, Rui Pan, Chenyuan Yang, Dylan Zhang, Liri Fang, Zikun Cui, Yang Cao, Pan Chen, Dorothy Sun, Ren Chen, Mahesh Srinivasan, Nipun Mathur, Yinglong Xia, Hong Li, Hong Yan, Pan Lu, Lingming Zhang, Tong Zhang, Hanghang Tong, Jingrui He  
**Data:** 2026-05-18  
**Categorie:** cs.CL, cs.AI  
**Link:** https://arxiv.org/abs/2605.18747v1

> Recent large language models (LLMs) have demonstrated strong capabilities in understanding and generating code, from competitive programming to repository-level software engineering. In emerging agentic systems, code is no longer only a target output. It increasingly serves as an operational substrate for agent reasoning, acting, environment modeling, and execution-based verification. We frame this shift through the lens of agent harnesses and introduce code as agent harness: a unified view that centers code as the basis for agent infrastructure. To systematically study this perspective, we organize the survey around three connected layers. First, we study the harness interface, where code connects agents to reasoning, action, and environment modeling. Second, we examine harness mechanisms: planning, memory, and tool use for long-horizon execution, together with feedback-driven control and optimization that make harness reliable and adaptive. Third, we discuss scaling the harness from single-agent systems to multi-agent settings, where shared code artifacts support multi-agent coordination, review, and verification. Across these layers, we summarize representative methods and practical applications of code as agent harness, spanning coding assistants, GUI/OS automation, embodied agents, scientific discovery, personalization and recommendation, DevOps, and enterprise workflows. We further outline open challenges for harness engineering, including evaluation beyond final task success, verification under incomplete feedback, regression-free harness improvement, consistent shared state across multiple agents, human oversight for safety-critical actions, and extensions to multimodal environments. By centering code as the harness of agentic AI, this survey provides a unified roadmap toward executable, verifiable, and stateful AI agent systems.

---

## 399. CHI-Bench: Can AI Agents Automate End-to-End, Long-Horizon, Policy-Rich Healthcare Workflows?

**Autori:** Haolin Chen, Deon Metelski, Leon Qi, Tao Xia, Joonyul Lee, Steve Brown, Kevin Riley, Frank Wang, T. Y. Alvin Liu, Hank Capps MD, Zeyu Tang, Xiangchen Song, Lingjing Kong, Fan Feng, Tianyi Zeng, Zhiwei Liu, Zixian Ma, Hang Jiang, Fangli Geng, Yuan Yuan, Chenyu You, Qingsong Wen, Hua Wei, Yanjie Fu, Yue Zhao, Carl Yang, Biwei Huang, Kun Zhang, Caiming Xiong, Sanmi Koyejo, Eric P. Xing, Philip S. Yu, Weiran Yao  
**Data:** 2026-05-15  
**Categorie:** cs.CL, cs.AI  
**Link:** https://arxiv.org/abs/2605.16679v3

> End-to-end automation of realistic healthcare operations stresses three capabilities underrepresented in current benchmarks: policy density, decisions must be grounded in a large library of medical, insurance, and operational rules; Multi-role composition: a single task requires the agent to play multiple roles with handoffs; and multilateral interaction: intermediate workflow steps are multi-turn dialogs, such as peer-to-peer review and patient outreach. We introduce $χ$-Bench, a benchmark of long-horizon healthcare workflows across three domains: provider prior authorization, payer utilization management, and care management. Each task hands the agent a clinical case in a high-fidelity simulator of 20 healthcare apps exposed via 87 MCP tools, which it must drive to a terminal status through tool calls and writing the role's artifacts, guided by a 1,290+ document managed-care operations handbook skill. Across 30 agent harness/models configurations, the best agent resolves only 28.0% of tasks, no agent clears 20% on strict pass^3, and executing all tasks in a single session slumps the performance to 3.8%. These results raise the hypothesis that similar gaps are likely to surface in other policy-dense, role-composed, irreversible enterprise domains.

---

## 400. Is Grep All You Need? How Agent Harnesses Reshape Agentic Search

**Autori:** Sahil Sen, Akhil Kasturi, Elias Lumer, Anmol Gulati, Vamse Kumar Subbiah  
**Data:** 2026-05-14  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2605.15184v1

> Recent advances in Large Language Model (LLM) agents have enabled complex agentic workflows where models autonomously retrieve information, call tools, and reason over large corpora to complete tasks on behalf of users. Despite the growing adoption of retrieval-augmented generation (RAG) in agentic search systems, existing literature lacks a systematic comparison of how retrieval strategy choice interacts with agent architecture and tool-calling paradigm. Important practical dimensions, including how tool outputs are presented to the model and how performance changes when searches must cope with more irrelevant surrounding text, remain under-explored in agent loops. This paper reports an empirical study organized into two experiments. Experiment 1 compares grep and vector retrieval on a 116-question sample from LongMemEval, using a custom agent harness (Chronos) and provider-native CLI harnesses (Claude Code, Codex, and Gemini CLI), for both inline tool results and file-based tool results that the model reads separately. Experiment 2 compares grep-only and vector-only retrieval while progressively mixing in additional unrelated conversation history, so that each query is embedded in more distracting material alongside the passages that matter. Across Chronos and the provider CLIs, grep generally yields higher accuracy than vector retrieval in our comparisons in experiment 1; at the same time, overall scores still depend strongly on which harness and tool-calling style is used, even when the underlying conversation data are the same.

---

## 401. Orchard: An Open-Source Agentic Modeling Framework

**Autori:** Baolin Peng, Wenlin Yao, Qianhui Wu, Hao Cheng, Xiao Yu, Rui Yang, Tao Ge, Alessandro Sordoni, Xingdi Yuan, Yelong Shen, Pengcheng He, Tong Zhang, Zhou Yu, Jianfeng Gao  
**Data:** 2026-05-14  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2605.15040v3

> Agentic modeling aims to transform LLMs into autonomous agents capable of solving complex tasks through planning, reasoning, tool use, and multi-turn interaction with external environments. We present Orchard, an open-source framework for scalable agentic modeling. At its core is Orchard Env, a lightweight Kubernetes-native environment service that provides reusable primitives for sandbox lifecycle management across task domains, agent harnesses, and training stages. On top of Orchard Env, we build three agentic modeling recipes. Orchard-SWE targets software engineering agents. We introduce credit-assignment supervised fine-tuning and a progression of RL signals: Balanced Adaptive Rollout (BAR) for sparse-reward optimization, on-policy distillation (OPD) and rubric-based process reward (RPR) for dense supervision, and historical experience distillation, which compresses rollouts from prior experiments into a compact value model for inference-time reranking. Built on the Qwen3.5-35B-A3B backbone, Orchard-SWE reaches 69.7% with RPR-based RL and 73.0% with value-model reranking on SWE-bench Verified, setting a new state of the art among open-source methods while approaching frontier systems over 10x larger. Orchard-GUI trains a 4B vision-language computer-use agent using only 0.4K distilled trajectories and 2.2K open-ended tasks, achieving 68.4% average success across WebVoyager, Online-Mind2Web, and DeepShop, making it the strongest open-source model while remaining competitive with proprietary systems. Orchard-Claw targets personal assistant agents. Trained with only 0.2K synthetic tasks, it achieves 59.6% pass@3 on Claw-Eval and 73.9% when paired with the stronger ZeroClaw harness. Collectively, these results demonstrate that a lightweight, open, harness-agnostic environment layer enables reusable agentic data, training recipes, and evaluation protocols across domains.

---

## 402. Auditing Agent Harness Safety

**Autori:** Chengzhi Liu, Yichen Guo, Yepeng Liu, Yuzhe Yang, Qianqi Yan, Xuandong Zhao, Wenyue Hua, Sheng Liu, Sharon Li, Yuheng Bu, Xin Eric Wang  
**Data:** 2026-05-14  
**Categorie:** cs.CL, cs.CY  
**Link:** https://arxiv.org/abs/2605.14271v2

> LLM agents increasingly run inside execution harnesses that dispatch tools, allocate resources, and route messages between specialized components. However, a harness can return a correct, benign answer over a trajectory that accesses unauthorized resources or leaks context to the wrong agent. Output-level evaluation cannot see these failures, yet most safety benchmarks score only final outputs or terminal states, even though many violations occur mid-trajectory rather than at termination. The central question is whether the harness respects user intent, permission boundaries, and information-flow constraints throughout execution. To address this gap, we propose HarnessAudit, a framework that audits full execution trajectories across boundary compliance, execution fidelity, and system stability, with a focus on multi-agent harnesses where these risks are most pronounced. We further introduce HarnessAudit-Bench, a benchmark of 210 tasks across eight real-world domains, instantiated in both single-agent and multi-agent configurations with embedded safety constraints. Evaluating ten harness configurations across frontier models and three multi-agent frameworks, we find that: (i) task completion is misaligned with safe execution, and violations accumulate with trajectory length; (ii) safety risks vary across domains, task types, and agent roles; (iii) most violations concentrate in resource access and inter-agent information transfer; and (iv) multi-agent collaboration expands the safety risk surface, while harness design sets the upper bound of safe deployment.

---

## 403. Harness Engineering as Categorical Architecture

**Autori:** Bogdan Banu  
**Data:** 2026-05-12  
**Categorie:** cs.PL, cs.AI, math.CT  
**Link:** https://arxiv.org/abs/2605.12239v1

> The agent harness, the system layer comprising prompts, tools, memory, and orchestration logic that surrounds the model, has emerged as the central engineering abstraction for LLMbased agents. Yet harness design remains ad hoc, with no formal theory governing composition, preservation of properties under compilation, or systematic comparison across frameworks. We show that the categorical Architecture triple (G, Know, Phi) from the ArchAgents framework provides exactly this formalization. The four pillars of agent externalization (Memory, Skills, Protocols, Harness Engineering) map onto the triple's components: Memory as coalgebraic state, Skills as operad-composed objects, Protocols as syntactic wiring G, and the full Harness as the Architecture itself. Structural guarantees-integrity gates, quality-based escalation, supported convergence checks-are Know-level certificates whose preservation is structural replay: our compiler checks identity and verifier replay, not output-layer correctness or model behavior. We validate this correspondence with a reference implementation featuring compiler functors targeting Swarms, DeerFlow, Ralph, Scion, and LangGraph: the four configuration compilers preserve three named certificate types by identity or replay, and LangGraph preserves the same certificates through its shared per-stage execution path. The LangGraph compiler creates one node per stage using the same per-stage method as the native runtime, providing LangGraph-native observability without reimplementing harness logic. An end-to-end escalation experiment with real LLM agents confirms that the quality-based escalation control path is model-parametric in this two-model, one-task experiment. The result positions categorical architecture as the formal theory behind harness engineering.

---

## 404. CAX-Agent: A Lightweight Agent Harness for Reliable APDL Automation

**Autori:** Chenying Lin, Yichen Hai, Yi He, Ran Wang, Haiyan Qiang, Liang Yu  
**Data:** 2026-05-12  
**Categorie:** cs.AI, cs.CE  
**Link:** https://arxiv.org/abs/2605.15218v1

> Large language models deployed for MAPDL finite-element simulation face practical reliability challenges: without structured execution control, tool encapsulation, and fault recovery, outputs may be inconsistent and task failures are common. The Agent Harness paradigm addresses this by inserting domain-specific orchestration middleware that manages tool lifecycles, workflow state, and recovery escalation. This paper presents the architecture of CAX-Agent, a lightweight agent harness purpose-built for MAPDL automation, and empirically evaluates one of its core components -- the recovery policy.CAX-Agent organizes execution into three layers -- LLM service, agent harness, and solver backend -- with a recovery ladder that escalates from deterministic rule patching through model-driven regeneration to context enrichment and human intervention. We evaluate three recovery strategies (no_recovery, rule_only, and model_only) on 50 standard structural benchmarks with three repeated runs per strategy (450 case-runs total). Two independent human raters score task completion under blind conditions; inter-rater agreement is strong (quadratic weighted Cohen's kappa = 0.84, 96 percent of score pairs within one point). Model_only achieves the best completion rate (0.9267), task score (3.59/4), total score (9.16/10), and zero-intervention rate (0.84), outperforming rule_only (0.7733, 3.17/4, 7.03/10, 0.00) and no_recovery (0.6933, 2.74/4, 5.60/10, 0.00) with large effect sizes (Cliff's delta = 0.81-0.87). The benchmark uses deliberately simple geometries to isolate recovery-policy effects; we discuss the scope of these findings and directions for broader validation.

---

## 405. CVEvolve: Autonomous Algorithm Discovery for Unstructured Scientific Data Processing

**Autori:** Ming Du, Xiangyu Yin, Yanqi Luo, Dishant Beniwal, Songyuan Tang, Hemant Sharma, Mathew J. Cherukara  
**Data:** 2026-05-12  
**Categorie:** cs.AI, physics.data-an  
**Link:** https://arxiv.org/abs/2605.11359v3

> Scientific data processing often requires task-specific algorithms or AI models, creating a barrier for domain scientists who need to analyze their data but may not have extensive computing or image-processing expertise. This barrier is especially pronounced when data are noisy, have a high dynamic range, are sparsely labeled, or are only loosely specified. We introduce CVEvolve, an autonomous agentic harness with a zero-code interface for scientific data-processing algorithm discovery. CVEvolve combines a multi-round search strategy with tools for code execution, evaluation implementation, history management, holdout testing, and optional inspection of scientific data and visual outputs. The search alternates between discovery and improvement actions, and uses lineage-aware stochastic candidate sampling to balance exploration and exploitation. We demonstrate CVEvolve on X-ray fluorescence microscopy image registration, Bragg peak detection, high-energy diffraction microscopy image segmentation, and hybrid analytical-learning-based affine registration. Across these tasks, CVEvolve discovers algorithms that improve over baseline methods, while holdout test tracking helps identify candidates that generalize better than later over-optimized alternatives. These results show that zero-code, autonomous LLM-powered algorithm development can help domain scientists turn unstructured scientific image data into practical algorithms and downstream scientific discoveries.

---

## 406. WildClawBench: A Benchmark for Real-World, Long-Horizon Agent Evaluation

**Autori:** Shuangrui Ding, Xuanlang Dai, Long Xing, Shengyuan Ding, Ziyu Liu, Yang JingYi, Penghui Yang, Zhixiong Zhang, Xilin Wei, Xinyu Fang, Yubo Ma, Haodong Duan, Jing Shao, Jiaqi Wang, Dahua Lin, Kai Chen, Yuhang Zang  
**Data:** 2026-05-11  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2605.10912v1

> Large language and vision-language models increasingly power agents that act on a user's behalf through command-line interface (CLI) harnesses. However, most agent benchmarks still rely on synthetic sandboxes, short-horizon tasks, mock-service APIs, and final-answer checks, leaving open whether agents can complete realistic long-horizon work in the runtimes where they are deployed. This work presents WildClawBench, a native-runtime benchmark of 60 human-authored, bilingual, multimodal tasks spanning six thematic categories. Each task averages roughly 8 minutes of wall-clock time and over 20 tool calls, and runs inside a reproducible Docker container hosting an actual CLI agent harness (OpenClaw, Claude Code, Codex, or Hermes Agent) with access to real tools rather than mock services. Grading is hybrid, combining deterministic rule-based checks, environment-state auditing of side effects, and an LLM/VLM judge for semantic verification. Across 19 frontier models, the best, Claude Opus 4.7, reaches only 62.2% overall under OpenClaw, while every other model stays below 60%, and switching harness alone shifts a single model by up to 18 points. These results show that long-horizon, native-runtime agent evaluation remains a far-from-resolved task for current frontier models. We release the tasks, code, and containerized tooling to support reproducible evaluation.

---

## 407. Towards On-Policy Data Evolution for Visual-Native Multimodal Deep Search Agents

**Autori:** Shijue Huang, Hangyu Guo, Guanting Dong, Chenxin Li, Junting Lu, Xinyu Geng, Zhaochen Su, Zhenyu Li, Shuang Chen, Hongru Wang, Yi R. Fung  
**Data:** 2026-05-11  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2605.10832v2

> Multimodal deep search requires an agent to solve open-world problems by chaining search, tool use, and visual reasoning over evolving textual and visual context. Two bottlenecks limit current systems. First, existing tool-use harnesses treat images returned by search, browsing, or transformation as transient outputs, so intermediate visual evidence cannot be re-consumed by later tools. Second, training data is usually built by fixed curation recipes that cannot track the target agent's evolving capability. To address these challenges, we first introduce a visual-native agent harness centered on an image bank reference protocol, which registers every tool-returned image as an addressable reference and makes intermediate visual evidence reusable by later tools. On top of this harness, On-policy Data Evolution (ODE) runs a closed-loop data generator that refines itself across rounds from rollouts of the policy being trained. This per-round refinement makes each round's data target what the current policy still needs to learn. The same framework supports both diverse supervised fine-tuning data and policy-aware reinforcement learning data curation, covering the full training lifecycle of the target agent. Across 8 multimodal deep search benchmarks, ODE improves the Qwen3-VL-8B agent from 24.9% to 39.0% on average, surpassing Gemini-2.5 Pro in standard agent-workflow setting (37.9%). At 30B, ODE raises the average score from 30.6% to 41.5%. Further analyses validate the effectiveness of image-bank reuse, especially on complex tasks requiring iterative visual refinement, while rollout-feedback evolution yields more grounded SFT traces and better policy-matched RL tasks than static synthesis.

---

## 408. Workspace Optimization: How to Train Your Agent

**Autori:** Elad Sarafian, Gal Kaplun, Ron Banner, Daniel Soudry, Boris Ginsburg  
**Data:** 2026-05-10  
**Categorie:** cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2605.09650v1

> Modern agents built on frontier language models often cannot adapt their weights. What, then, remains trainable? We argue it is the agent's \emph{workspace}, the structured external substrate it reads, writes, and tests; we call its evolution workspace optimization. Workspace optimization targets hard multi-turn environments where a frontier model has strong priors but cannot solve the task in a single shot, so the agent must learn through interaction. We propose a principled way to evolve the workspace, mirroring the structure of weight-space training: artifacts in place of parameters, evidence in place of data, counterexamples in place of losses, and textual feedback in place of gradients. We instantiate the idea in DreamTeam, a multi-agent harness for ARC-AGI-3 whose roles build an executable world model, plan, hypothesize, probe, strategize, and route failures. On the current 25-game ARC-AGI-3 public set under the official scoring protocol and averaged over two independent runs, DreamTeam improves the SOTA protocol-matched agent's score from 36% to 38.4%, while using 31% fewer environment actions per game.

---

## 409. GameGen-Verifier: Parallel Keypoint-Based Verification for LLM-Generated Games via Runtime State Injection

**Autori:** Chaobo Jia, Ruipeng Wan, Ting Sun, Weihao Tan, Borui Wan, Yuxuan Tong, Guangming Sheng, Hong Xu  
**Data:** 2026-05-08  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2605.07442v1

> LLM-based game generation promises to turn natural-language specifications into executable games, but progress is limited by the lack of reliable automated verification. Unlike conventional code generation, game correctness is defined over long-horizon interaction: a game may appear correct while violating core mechanics such as state updates, interaction rules, and phase transitions. Existing Agent-as-a-Verifier approaches collapse verification into open-ended gameplay, making verdicts reachability-bound, time-consuming, coverage-limited, and sensitive to the agent's gameplay ability. We present GameGen-Verifier, an automated verification paradigm for LLM-generated games that decomposes a specification into verifiable keypoints and grounds them into independent verification units. Each unit patches the game runtime into a concrete target state, executes a bounded interaction, and judges the outcome against the keypoint assertion. We implement GGV-Harness, a scalable agentic harness providing concurrency management, runtime isolation, and fault recovery. On VeriGame, our dataset of 100 games across seven genres, GameGen-Verifier achieves up to 92.2% accuracy against human judgments versus 58.8% for the coverage-enforced Agent-as-a-Verifier baseline, while reducing wall-clock time by up to 16.6x.

---

## 410. Eta Given Delta: Defining LLM Tool Efficiency With Marginal Tool Utility

**Autori:** Nyx Iskandar, Perla Gamez  
**Data:** 2026-05-07  
**Categorie:** cs.CL, cs.AI, cs.SE  
**Link:** https://arxiv.org/abs/2607.14108v2

> This paper introduces tool efficiency, a new quantitative metric to evaluate the rate of useful tool calls in an LLM agent trajectory. To ensure that tool efficiency is well-defined, we also introduce marginal tool utility, a new quantitative metric defined per tool call indicating whether a tool is useful or whether it can be safely removed from the tool suite without affecting accuracy while increasing tool efficiency; in this paper, we determine the sign of marginal tool utility for each tool call in a trajectory using LLM-as-a-Judge. While much prior work has been done to develop techniques that improve tool use by LLMs and design evaluation methods measuring efficiency indirectly using accuracy as a proxy, our work is centered on measuring efficiency directly via the quantitative metric proposed in this paper in post hoc trajectory analyses. It is our intention that this work contributes to the frontier of LLM evaluation research as a springboard for future benchmark designs and agent harness engineering (specifically with regards to creating lean tool suites) that optimize for metrics that complement but are distinct from accuracy.

---

## 411. Agentick: A Unified Benchmark for General Sequential Decision-Making Agents

**Autori:** Roger Creus Castanyer, Pablo Samuel Castro, Glen Berseth  
**Data:** 2026-05-07  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2605.06869v3

> AI agent research spans a wide spectrum: from RL agents that learn from scratch to foundation model agents that leverage pre-trained knowledge, yet no unified benchmark enables fair comparison across these approaches. We present Agentick, a benchmark for sequential decision-making agents designed to evaluate RL, LLM, VLM, hybrid, and human agents on common ground and to power research on the fundamental challenges of sequential decision-making. Agentick provides 37 procedurally generated tasks across six capability categories, four difficulty levels, and five observation modalities, all exposed through a single Gymnasium-compatible interface. The benchmark ships with a Coding API, oracle reference policies for all tasks, pre-built SFT datasets, a composable agent harness, and a live leaderboard. An evaluation spanning 27 configurations and over 90,000 episodes reveals that no single approach dominates: GPT-5 mini leads overall at 0.309 oracle-normalized score while PPO dominates planning and multi-agent tasks; the reasoning harness multiplies LLM performance by 3-10x; and ASCII observations consistently outperform natural language. These findings highlight the substantial room for improvement that remains across all agent paradigms. Agentick's capability-decomposed, multi-modal design provides the empirical infrastructure needed to drive progress toward general autonomous agents, both as an evaluation framework and as a training ground for RL post-training of foundation models in truly sequential environments.

---

## 412. BioMedArena: An Open-source Toolkit for Building and Evaluating Biomedical Deep Research Agents

**Autori:** Jinge Wu, Hongjian Zhou, Mingde Zeng, Jiayuan Zhu, Junde Wu, Jiazhen Pan, Ayush Noori, Sean Wu, Honghan Wu, Fenglin Liu, David A. Clifton  
**Data:** 2026-05-07  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2605.06177v2

> Reproducing and comparing deep research agents today is hard: the same backbone evaluated on the same benchmark can report different accuracies across papers because the harness and tool registry differ, and integrating a new model into a comparable evaluation surface costs weeks of model-specific engineering. These are symptoms of a broader reproducibility problem in deep research agent research. Here, we introduce BioMedArena, an open-source toolkit that addresses this reproducibility gap and provides an arena for comparing deep research agents under a shared evaluation environment. BioMedArena decouples six layers of biomedical agent evaluation -- benchmark loading, tool exposure, tool selection, harness mode, context management, and scoring -- and exposes 166 biomedical benchmarks and 75 biomedical tools across 9 functional families. Adding a new model, benchmark, or tool can be accomplished with a few-line provider adapter. Beyond evaluation infrastructure, BioMedArena ships a library of high-quality reference components: 6 agent harnesses (including our proposed Mutual-Evolve) and 6 context-management strategies, any of which can be equipped on any backbone. Equipping these components substantially improves all 12 backbones; on each of 8 representative biomedical benchmarks, the best equipped backbone surpasses prior state-of-the-art (SOTA), by 15.01 percentage points on average. The toolkit, configurations, and per-task traces are available at https://github.com/AI-in-Health/BioMedArena.

---

## 413. AlphaCrafter: Harnessing Multi-Agent Workflows for Cross-Sectional Quantitative Trading

**Autori:** Yishuo Yuan, Jiayi Sheng, Sirui Zeng, Jiaqi Wang, Jiaheng Liu  
**Data:** 2026-05-07  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2605.05580v2

> Quantitative trading agents have demonstrated substantial promise in automating factor discovery, signal aggregation, and portfolio execution. However, existing agent-based trading systems predominantly rely on loosely specified natural-language workflows, leading to opaque reasoning processes, inconsistent behaviors across foundation models, and limited controllability and verifiability, all of which introduce significant risks in financial decision-making. To address these limitations, we propose AlphaCrafter, a multi-agent framework built upon a structured agent harness. Instead of treating agent behavior as unconstrained prompt execution, AlphaCrafter encapsulates each agent within programmable policy specifications that integrate procedural workflows, execution constraints, and explicit verification mechanisms. This harness-driven design transforms the entire trading pipeline into a sequence of well-defined, reproducible, and auditable decision processes with explicit execution semantics. Extensive experiments on the CSI 300 and S&P 500 benchmarks demonstrate that AlphaCrafter consistently achieves superior risk-adjusted returns while exhibiting substantially lower cross-model and cross-trial variance. These results suggest that harness-based agent design provides a practical foundation for building more reliable, controllable, and robust multi-agent systems for quantitative trading.

---

## 414. AgenticRAG: Agentic Retrieval for Enterprise Knowledge Bases

**Autori:** Susheel Suresh, Hazel Mak, Shangpo Chou, Fred Kroon, Sahil Bhatnagar  
**Data:** 2026-05-07  
**Categorie:** cs.AI, cs.IR  
**Link:** https://arxiv.org/abs/2605.05538v1

> We present AgenticRAG, a practical agentic harness for retrieval and analysis over enterprise knowledge bases. Standard RAG pipelines place significant burden of grounding on the search stack, constraining the language model to a fixed candidate set chosen deep in the retrieval process. Our approach reduces this overdependence by layering a lightweight harness on top of existing enterprise search infrastructure, equipping a reasoning LLM with search, find, open, and summarize tools enabling the model to iteratively retrieve information, navigate within documents, and analyze evidence autonomously. On three open benchmarks we observe substantial gains: $49.6\%$ recall@1 on BRIGHT (+21.8 pp over the best embedding baseline), 0.96 factuality on WixQA ($+13\%$ relative improvement), and $92\%$ answer correctness on FinanceBench--within 2 pp of oracle access to true evidence. Ablation studies show that the most significant factor is the shift from single-shot retrieval to agentic tool use ($5.9\times$ improvement), while multi-query search and in-document navigation contribute to both quality and efficiency. We present various design choices in our agentic harness that were informed by pre-production deployments. Our results demonstrate its suitability for real-world enterprise production environments.

---

## 415. Design Conductor 2.0: An agent builds a TurboQuant inference accelerator in 80 hours

**Autori:** The Verkor Team, Ravi Krishna, Suresh Krishna, David Chin  
**Data:** 2026-05-06  
**Categorie:** cs.AR, cs.AI  
**Link:** https://arxiv.org/abs/2605.05170v1

> Driven by a rapid co-evolution of both harness and underlying models, LLM agents are improving at a dizzying pace. In our prior work (performed in Dec. 2025), we introduced "Design Conductor" (or just "Conductor"), a system capable of building a 5-stage Linux-capable RISC-V CPU in 12 hours. In this work, we introduce an updated multi-agent harness powered by frontier models released in April 2026, which is able to handle 80x larger tasks, at higher quality, fully autonomously. Following a brief introduction, we examine 4 designs that the system produced autonomously, including "VerTQ", an LLM inference accelerator which hard-wires support for TurboQuant in a 240-cycle pipeline, starting from the TurboQuant arXiv paper. VerTQ includes heavy compute processing, with 5129 FP16/32 units; the design was mapped to an FPGA at 125 MHz and consumes 5.7 mm^2 in TSMC 16FF (8 attention pipes). We review the key new characteristics that enabled these results. Finally, we analyze Design Conductor's token usage and other empirical characteristics, including its limitations.

---

## 416. Workspace-Bench 1.0: Benchmarking AI Agents on Workspace Tasks with Large-Scale File Dependencies

**Autori:** Zirui Tang, Xuanhe Zhou, Yumou Liu, Linchun Li, Yukai Wu, Weizheng Wang, Hongzhang Huang, Wei Zhou, Jun Zhou, Jiachen Song, Shaoli Yu, Jinqi Wang, Zihang Zhou, Hongyi Zhou, Yuting Lv, Jinyang Li, Jiashuo Liu, Ruoyu Chen, Chunwei Liu, GuoLiang Li, Jihua Kang, Fan Wu  
**Data:** 2026-05-05  
**Categorie:** cs.AI, cs.CL, cs.DB, cs.LG  
**Link:** https://arxiv.org/abs/2605.03596v4

> Workspace learning requires AI agents to identify, reason over, exploit, and update explicit and implicit dependencies among heterogeneous files in a worker's workspace, enabling them to complete both routine and advanced tasks effectively. Despite its importance, existing relevant benchmarks largely evaluate agents on pre-specified or synthesized files with limited real-world dependencies, leaving workspace-level evaluation underexplored. To this end, we introduce Workspace-Bench, a benchmark for evaluating AI agents on Workspace Learning involving Large-Scale File Dependencies. We construct realistic workspaces with 5 worker profiles, 74 file types, 20,476 files (up to 20GB) and curate 388 tasks, each with its own file dependency graph, evaluated across 7,399 total rubrics that require cross-file retrieval, contextual reasoning, and adaptive decision-making. We further provide Workspace-Bench-Lite, a 100-task subset that preserves the benchmark distribution while reducing evaluation costs by about 70%. We evaluate 4 popular agent harnesses and 7 foundation models. Experimental results show that current agents remain far from reliable workspace learning, where the best reaches only about 60%, substantially below the human result of 80.7%, and the average performance across agents is only 43.3%.

---

## 417. HeavySkill: Heavy Thinking as the Inner Skill in Agentic Harness

**Autori:** Jianing Wang, Linsen Guo, Zhengyu Chen, Qi Guo, Hongyu Zang, Wenjie Shi, Haoxiang Ma, Xiangyu Xi, Xiaoyu Li, Wei Wang, Xunliang Cai  
**Data:** 2026-05-04  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2605.02396v1

> Recent advances in agentic harness with orchestration frameworks that coordinate multiple agents with memory, skills, and tool use have achieved remarkable success in complex reasoning tasks. However, the underlying mechanism that truly drives performance remains obscured behind intricate system designs. In this paper, we propose HeavySkill, a perspective that views heavy thinking not only as a minimal execution unit in orchestration harness but also as an inner skill internalized within the model's parameters that drives the orchestrator to solve complex tasks. We identify this skill as a two-stage pipeline, i.e., parallel reasoning then summarization, which can operate beneath any agentic harness. We present a systematic empirical study of HeavySkill across diverse domains. Our results show that this inner skill consistently outperforms traditional Best-of-N (BoN) strategies; notably, stronger LLMs can even approach Pass@N performance. Crucially, we demonstrate that the depth and width of heavy thinking, as a learnable skill, can be further scaled via reinforcement learning, offering a promising path toward self-evolving LLMs that internalize complex reasoning without relying on brittle orchestration layers.

---

## 418. Affordance Agent Harness: Verification-Gated Skill Orchestration

**Autori:** Haojian Huang, Jiahao Shi, Yinchuan Li, Yingcong Chen  
**Data:** 2026-05-01  
**Categorie:** cs.RO, cs.CV  
**Link:** https://arxiv.org/abs/2605.00663v2

> Affordance grounding requires identifying where and how an agent should interact in open-world scenes, where actionable regions are often small, occluded, reflective, and visually ambiguous. Recent systems therefore combine multiple skills (e.g., detection, segmentation, interaction-imagination), yet most orchestrate them with fixed pipelines that are poorly matched to per-instance difficulty, offer limited targeted recovery from intermediate errors, and fail to reuse experience from recurring objects. These failures expose a systems problem: test-time grounding must acquire the right evidence, decide whether that evidence is reliable enough to commit, and do so under bounded inference cost without access to labels. We propose Affordance Agent Harness, a closed-loop runtime that unifies heterogeneous skills with an evidence store and cost control, retrieves episodic memories to provide priors for recurring categories, and employs a Router to adaptively select and parameterize skills. An affordance-specific Verifier then gates commitments using self-consistency, cross-scale stability, and evidence sufficiency, triggering targeted retries before a final judge fuses accumulated evidence and trajectories into the prediction. Experiments on multiple affordance benchmarks and difficulty-controlled subsets show a stronger accuracy-cost Pareto frontier than fixed-pipeline baselines, improving grounding quality while reducing average skill calls and latency. Project page: https://tenplusgood.github.io/a-harness-page/.

---

## 419. Agentic Harness Engineering: Observability-Driven Automatic Evolution of Coding-Agent Harnesses

**Autori:** Jiahang Lin, Shichun Liu, Chengjun Pan, Lizhi Lin, Shihan Dou, Zhiheng Xi, Xuanjing Huang, Hang Yan, Zhenhua Han, Tao Gui, Yu-Gang Jiang  
**Data:** 2026-04-28  
**Categorie:** cs.CL, cs.SE  
**Link:** https://arxiv.org/abs/2604.25850v4

> Harnesses are now central to coding-agent performance, mediating how models interact with tools and execution environments. Yet harness engineering remains a manual craft, because automating it faces a heterogeneous action space across editable components, voluminous trajectories that bury actionable signal, and edits whose effect is hard to attribute. We introduce Agentic Harness Engineering (AHE), a closed loop that addresses these challenges through three matched observability pillars: (1) component observability gives every editable harness component a file-level representation so the action space is explicit and revertible; (2) experience observability distills millions of raw trajectory tokens into a layered, drill-down evidence corpus that an evolving agent can actually consume; and (3) decision observability pairs every edit with a self-declared prediction, later verified against the next round's task-level outcomes. Together, these pillars turn every edit into a falsifiable contract, so harness evolution proceeds autonomously without collapsing into trial-and-error. Empirically, ten AHE iterations lift pass@1 on Terminal-Bench 2 from 69.7% to 77.0%, surpassing the human-designed harness Codex-CLI (71.9%) and the self-evolving baselines ACE and TF-GRPO. The frozen harness transfers without re-evolution: on SWE-bench-verified it tops aggregate success at 12% fewer tokens than the seed, and on Terminal-Bench 2 it yields +5.1 to +10.1pp cross-family gains across three alternate model families, indicating the evolved components encode general engineering experience rather than benchmark-specific tuning. Ablations localize the gain to tools, middleware, and long-term memory rather than the system prompt, suggesting factual harness structure transfers while prose-level strategy does not.

---

## 420. Toward Scalable Terminal Task Synthesis via Skill Graphs

**Autori:** Zhiyuan Fan, Tinghao Yu, Yuanjun Cai, Jiangtao Guan, Yun Yang, Dingxin Hu, Jiang Zhou, Xing Wu, Zhuo Han, Feng Zhang, Lilin Wang  
**Data:** 2026-04-28  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2604.25727v1

> Terminal agents have demonstrated strong potential for autonomous command-line execution, yet their training remains constrained by the scarcity of high-quality and diverse execution trajectories. Existing approaches mitigate this bottleneck by synthesizing large-scale terminal task instances for trajectory sampling. However, they primarily focus on scaling the number of tasks while providing limited control over the diversity of execution trajectories that agents actually experience during training. In this paper, we present SkillSynth, an automated framework for terminal task synthesis built on a scenario-mediated skill graph. SkillSynth first constructs a large-scale skill graph, where scenarios serve as intermediate transition nodes that connect diverse command-line skills. It then samples paths from this graph as abstractions of real-world workflows, and uses a multi-agent harness to instantiate them into executable task instances. By grounding task synthesis in graph-sampled workflow paths, SkillSynth explicitly controls the diversity of minimal execution trajectories required to solve the synthesized tasks. Experiments on Terminal-Bench demonstrate the effectiveness of SkillSynth. Moreover, task instances synthesized by SkillSynth have been adopted to train Hy3 Preview, contributing to its enhanced agentic capabilities in terminal-based settings.

---

## 421. JudgeSense: A Benchmark for Prompt Sensitivity in LLM-as-a-Judge Systems

**Autori:** Rohith Reddy Bellibatlu, Edward Raff, Wenbin Zhang  
**Data:** 2026-04-26  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2604.23478v3

> Large language models are widely used to judge the output of other language models, yet whether a judge returns the same verdict when the same request is worded differently remains largely unexamined. We study that question across four evaluation tasks and twenty-five judges from six providers. To support the analysis we release JudgeSense, a benchmark of 880 items from human-labelled corpora, each issued under two instructions that differ in wording and not in what they ask, with the complete decision logs. Every score is reported against the judge's own agreement with itself on the identical prompt, so decoding noise is not charged to wording, and the release lets a reader ask the same of any judge not in our roster. Rewording costs agreement on all four tasks, and on two it clears the threshold we declare for a practically meaningful effect; the ordinal task is both the least stable and the one fewest judges are accurate on, and within a single family parameter count does not predict stability. A judge measured inside an agent harness yields a smaller estimate than the same judge reached through a direct API call, because its agreement with itself collapses faster than its agreement across wordings.

---

## 422. AEL: Evolving Agent Harness in Open-Ended Environments

**Autori:** Wujiang Xu, Jiaojiao Han, Minghao Guo, Kai Mei, Xi Zhu, Han Zhang, Dimitris N. Metaxas  
**Data:** 2026-04-23  
**Categorie:** cs.CL, cs.AI, cs.CE  
**Link:** https://arxiv.org/abs/2604.21725v2

> LLM Agents Harnesses are hand-designed and stay fixed, so agents accumulate experience but never learn how to use it: which memories to retrieve, when retrieved evidence is misleading, and when the retrieval strategy itself should change. We introduce Agent Evolving Learning (AEL), a two-timescale framework that evolves the harness, recasting memory use as online policy selection. A fast Thompson Sampling bandit selects among memory-retrieval policies episode by episode, while slow LLM reflection follows a diagnose-before-prescribe principle: it first explains why performance degraded, then injects a targeted new retrieval policy as a bandit arm when the current pool plateaus. AEL outperforms ten self-improving and nonLLM baselines on a sequential portfolio benchmark, lifting Sharpe by 27% over the strongest memory-only variant with the lowest variance among all stochastic methods, and generalizes to a support-ticket routing stream, where it improves accuracy by 18% over reflectionfree Thompson Sampling and by 51% over the best prior baseline. Mechanism studies further show that the gains are causal: reflection helps precisely when regimes demand different retrieval behavior, and is provably no-harm/nogain when the best policy is stable. Code and data: https://github.com/WujiangXu/AEL.

---

## 423. The Last Harness You'll Ever Build

**Autori:** Haebin Seong, Li Yin, Haoran Zhang, Zhan Shi  
**Data:** 2026-04-22  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2604.21003v3

> AI agents are increasingly deployed on complex, domain-specific workflows -- navigating enterprise web applications that require dozens of clicks and form fills, orchestrating multi-step research pipelines that span search, extraction, and synthesis, automating code review across unfamiliar repositories, and handling customer escalations that demand nuanced domain knowledge. \textbf{Each new task domain requires painstaking, expert-driven harness engineering}: designing the prompts, tools, orchestration logic, and evaluation criteria that make a foundation model effective. We present a two-level framework that automates this process. At the first level, the \textbf{Harness Evolution Loop} optimizes a worker agent's harness $\mathcal{H}$ for a single task: a Worker Agent $W_{\mathcal{H}}$ executes the task, an Evaluator Agent $V$ adversarially diagnoses failures and scores performance, and an Evolution Agent $E$ modifies the harness based on the full history of prior attempts. At the second level, the \textbf{Meta-Evolution Loop} optimizes the evolution blueprint $Λ= (W_{\mathcal{H}}, \mathcal{H}^{(0)}, V, E)$ itself across diverse tasks, \textbf{learning a blueprint $Λ^{(\text{best})}$ that enables rapid harness convergence on any new task -- so that adapting an agent to a novel domain requires no human harness engineering at all.} We formalize the correspondence to meta-learning and present both algorithms. The framework \textbf{shifts manual harness engineering into automated harness engineering}, and takes one step further -- \textbf{automating the design of the automation itself}.

---

## 424. HARBOR: Automated Harness Optimization

**Autori:** Biswa Sengupta, Jinhua Wang  
**Data:** 2026-04-22  
**Categorie:** cs.LG, cs.AI  
**Link:** https://arxiv.org/abs/2604.20938v1

> Long-horizon language-model agents are dominated, in lines of code and in operational complexity, not by their underlying model but by the harness that wraps it: context compaction, tool caching, semantic memory, trajectory reuse, speculative tool prediction, and the glue that binds the model to a sandboxed execution environment. We argue that harness design is a first-class machine-learning problem and that automated configuration search dominates manual stacking once the flag space exceeds a handful of bits. We defend this claim in two steps. First, we formalize automated harness optimization as constrained noisy Bayesian optimization over a mixed-variable, cost-heterogeneous configuration space with cold-start-corrected rewards and a posterior chance-constrained safety check, and give a reference solver, HARBOR (Harness Axis-aligned Regularized Bayesian Optimization Routine), built from a block-additive SAAS surrogate, multi-fidelity cost-aware acquisition, and TuRBO trust regions. Second, we instantiate the problem in a flag-gated harness over a production coding agent and report a controlled four-round manual-tuning case study against a fixed task suite and an end-to-end HARBOR run. The formulation itself is task-class agnostic: the configuration space, reward correction, acquisition, and safety check apply to any agent harness with a bounded flag space and a reproducible task suite.

---

## 425. ClawEnvKit: Automatic Environment Generation for Claw-Like Agents

**Autori:** Xirui Li, Ming Li, Ion Stoica, Cho-Jui Hsieh, Tianyi Zhou  
**Data:** 2026-04-20  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2604.18543v4

> Constructing environments for training and evaluating claw-like agents remains a manual, human-intensive process that does not scale. We argue that what is needed is not just a dataset, but an automated pipeline capable of generating diverse, verified environments on demand. To this end, we introduce ClawEnvKit, an autonomous generation pipeline that instantiates this formalism from natural language descriptions. The pipeline comprises three modules: (1) a parser that extracts structured generation parameters from natural language input; (2) a generator that produces the task specification, tool interface, and scoring configuration; and (3) a validator that enforces feasibility, diversity, structural validity, and internal consistency across the generated environments. Using ClawEnvKit, we construct Auto-ClawEval, the first large-scale benchmark for claw-like agents, comprising 1,040 environments across 24 categories. Empirically, Auto-ClawEval matches or exceeds human-curated environments on coherence and clarity at 13,800x lower cost. Evaluated across 4 model families and 8 agent harness frameworks, we find that harness engineering boosts performance by up to 15.7 percentage points over a bare ReAct baseline, completion remains the primary axis of variation with no model saturating the benchmark, and automated generation enables evaluation at a scale previously infeasible. Beyond static benchmarking, ClawEnvKit enables live evaluation: users describe a desired capability in natural language and obtain a verified environment on demand, turning evaluation into a continuous, user-driven process. The same mechanism serves as an on-demand training environment generator, producing task distributions that adapt to an agent's current weaknesses rather than being bounded by existing user logs.

---

## 426. Architectural Design Decisions in AI Agent Harnesses

**Autori:** Hu Wei  
**Data:** 2026-04-20  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2604.18071v1

> AI agent systems increasingly rely on reusable non-LLM engineering infrastructure that packages tool mediation, context handling, delegation, safety control, and orchestration. Yet the architectural design decisions in this surrounding infrastructure remain understudied. This paper presents a protocol-guided, source-grounded empirical study of 70 publicly available agent-system projects, addressing three questions: which design-decision dimensions recur across projects, which co-occurrences structure those decisions, and which typical architectural patterns emerge. Methodologically, we contribute a transparent investigation procedure for analyzing heterogeneous agent-system corpora through source-code and technical-material reading. Empirically, we identify five recurring design dimensions (subagent architecture, context management, tool systems, safety mechanisms, and orchestration) and find that the corpus favors file-persistent, hybrid, and hierarchical context strategies; registry-oriented tool systems remain dominant while MCP- and plugin-oriented extensions are emerging; and intermediate isolation is common but high-assurance audit is rare. Cross-project co-occurrence analysis reveals that deeper coordination pairs with more explicit context services, stronger execution environments with more structured governance, and formalized tool-registration boundaries with broader ecosystem ambitions. We synthesize five recurring architectural patterns spanning lightweight tools, balanced CLI frameworks, multi-agent orchestrators, enterprise systems, and scenario-verticalized projects. The result provides an evidence-based account of architectural regularities in agent-system engineering, with grounded guidance for framework designers, selectors, and researchers.

---

## 427. Clover: A Neural-Symbolic Agentic Harness with Stochastic Tree-of-Thoughts for Verified RTL Repair

**Autori:** Zizhang Luo, Yansong Xu, Runlin Guo, Fan Cui, Kexing Zhou, Mile Xia, Hongyuan Hou, Yuhao Luo, Yun Liang  
**Data:** 2026-04-19  
**Categorie:** cs.AR, cs.AI  
**Link:** https://arxiv.org/abs/2604.17288v1

> RTL program repair remains a critical bottleneck in hardware design and verification. Traditional automatic program repair (APR) methods rely on predefined templates and synthesis, limiting their bug coverage. Large language models (LLMs) and coding agents based on them offer flexibility but suffer from randomness and context corruption when handling long RTL code and waveforms. We present Clover, a neural-symbolic agentic harness that orchestrates RTL repair as a structured search over code manipulations to explore a validated solution for the bug. Recognizing that different repair operations favor distinct strategies, Clover dynamically dispatches tasks to specialized LLM agents or symbolic solvers. At its core, Clover introduces stochastic tree-of-thoughts, a test-time scaling mechanism that manages the main agent's context as a search tree, balancing exploration and exploitation for reliable outcomes. An RTL-specific toolbox further empowers agents to interact with the debugging environment. Evaluated on the RTL-repair benchmark, Clover fixes 96.8% of bugs within a fixed time limit, covering 94% and 63% more bugs than both pure traditional and LLM-based baselines, respectively, while achieving an average pass@1 rate of 87.5%, demonstrating high reliability and effectiveness.

---

## 428. The Semi-Executable Stack: Agentic Software Engineering and the Expanding Scope of SE

**Autori:** Robert Feldt, Per Lenberg, Julian Frattini, Dhasarathy Parthasarathy  
**Data:** 2026-04-16  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2604.15468v2

> AI-based systems, currently driven largely by LLMs and tool-using agentic harnesses, are increasingly discussed as a possible threat to software engineering. Foundation models get stronger, agents can plan and act across multiple steps, and tasks such as scaffolding, routine test generation, straightforward bug fixing, and small integration work look more exposed than they did only a few years ago. The result is visible unease not only among students and junior developers, but also among experienced practitioners who worry that hard-won expertise may lose value. This paper argues for a different reading. The important shift is not that software engineering loses relevance. It is that the thing being engineered expands beyond executable code to semi-executable artifacts; combinations of natural language, tools, workflows, control mechanisms, and organizational routines whose enactment depends on human or probabilistic interpretation rather than deterministic execution. The Semi-Executable Stack is introduced as a six-ring diagnostic reference model for reasoning about that expansion, spanning executable artifacts, instructional artifacts, orchestrated execution, controls, operating logic, and societal and institutional fit. The model helps locate where a contribution, bottleneck, or organizational transition primarily sits, and which adjacent rings it depends on. The paper develops the argument through three worked cases, reframes familiar objections as engineering targets rather than reasons to dismiss the transition, and closes with a preserve-versus-purify heuristic for deciding which legacy software engineering processes, controls, and coordination routines should be kept and which should be simplified or redesigned. This paper is a conceptual keynote companion: diagnostic and agenda-setting rather than empirical.

---

## 429. AgentSPEX: An Agent SPecification and EXecution Language

**Autori:** Pengcheng Wang, Jerry Huang, Jiarui Yao, Rui Pan, Peizhi Niu, Yaowenqi Liu, Ruida Wang, Renhao Lu, Yuwei Guo, Tong Zhang  
**Data:** 2026-04-14  
**Categorie:** cs.CL  
**Link:** https://arxiv.org/abs/2604.13346v1

> Language-model agent systems commonly rely on reactive prompting, in which a single instruction guides the model through an open-ended sequence of reasoning and tool-use steps, leaving control flow and intermediate state implicit and making agent behavior potentially difficult to control. Orchestration frameworks such as LangGraph, DSPy, and CrewAI impose greater structure through explicit workflow definitions, but tightly couple workflow logic with Python, making agents difficult to maintain and modify. In this paper, we introduce AgentSPEX, an Agent SPecification and EXecution Language for specifying LLM-agent workflows with explicit control flow and modular structure, along with a customizable agent harness. AgentSPEX supports typed steps, branching and loops, parallel execution, reusable submodules, and explicit state management, and these workflows execute within an agent harness that provides tool access, a sandboxed virtual environment, and support for checkpointing, verification, and logging. Furthermore, we provide a visual editor with synchronized graph and workflow views for authoring and inspection. We include ready-to-use agents for deep research and scientific research, and we evaluate AgentSPEX on 7 benchmarks. Finally, we show through a user study that AgentSPEX provides a more interpretable and accessible workflow-authoring paradigm than a popular existing agent framework.

---

## 430. ClawVM: Harness-Managed Virtual Memory for Stateful Tool-Using LLM Agents

**Autori:** Mofasshara Rafique, Laurent Bindschaedler  
**Data:** 2026-04-11  
**Categorie:** cs.AI, cs.OS, cs.SE  
**Link:** https://arxiv.org/abs/2604.10352v1

> Stateful tool-using LLM agents treat the context window as working memory, yet today's agent harnesses manage residency and durability as best-effort, causing recurring failures: lost state after compaction, bypassed flushes on reset, and destructive writeback. We present \textsc{ClawVM}, a virtual memory layer that manages state as typed pages with minimum-fidelity invariants, multi-resolution representations under a token budget, and validated writeback at every lifecycle boundary. Because the harness already assembles prompts, mediates tools, and observes lifecycle events, it is the natural enforcement point; placing the contract there makes residency and durability deterministic and auditable. Across synthetic workloads, 12 real-session traces, and adversarial stress tests, \textsc{ClawVM} eliminates all policy-controllable faults whenever the minimum-fidelity set fits within the token budget, confirmed by an offline oracle, and adds median <50 microseconds of policy-engine overhead per turn.

---

## 431. COMPOSITE-Stem

**Autori:** Kyle Waters, Lucas Nuzzi, Tadhg Looram, Alessandro Tomasiello, Ariel Ghislain Kemogne Kamdoum, Bikun Li, Damien Sileo, Egor Kretov, Francesco Fournier-Facio, Georgios Soloupis, Haile Kassahun, Hew Wolff, Jiaqi Cai, Lianghui Li, Marc Roth, Mohinder Naiya, Naixu Guo, Qicheng Tang, Richard Wheeler, Samuele Sala, Serguei Popov, Steven Dillmann, Yuqi Li  
**Data:** 2026-04-10  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2604.09836v2

> AI agents hold growing promise for accelerating scientific discovery; yet, a lack of frontier evaluations hinders adoption into real workflows. Expert-written benchmarks have proven effective at measuring AI reasoning, but most at this stage have become saturated and only measure performance on constrained outputs. To help address this gap, we introduce COMPOSITE-STEM, a benchmark of 70 expert-written tasks in physics, biology, chemistry, and mathematics, curated by doctoral-level researchers. Our benchmark combines exact-match grading and criterion-based rubrics with an LLM-as-a-jury grading protocol, allowing more flexible assessment of scientifically meaningful outputs. Using an adapted multimodal Terminus-2 agent harness within the Harbor agentic evaluation framework, we evaluate four frontier models. The top-performing model achieves 21%, demonstrating that COMPOSITE-STEM captures capabilities beyond current agent reach. All tasks are open-sourced with contributor permission to support reproducibility and to promote additional research towards AI's acceleration of scientific progress in these domains.

---

## 432. How Much Heavy Lifting Can an Agent Harness Do?: Measuring the LLM's Residual Role in a Planning Agent

**Autori:** Sungwoo Jung, Seonil Son  
**Data:** 2026-04-08  
**Categorie:** cs.AI, cs.CL  
**Link:** https://arxiv.org/abs/2604.07236v4

> Agent harnesses -- the stateful programs that wrap a language model and decide what it sees at each step -- are now known to change end-to-end performance on a fixed model by as much as six times. That raises a question asked less often than it should be: how much of an agent's competence does the harness itself already carry, and how much genuinely still needs the LLM? We externalize a planning harness for noisy Collaborative Battleship into four progressively richer layers -- posterior belief tracking, declarative planning, symbolic reflec tion, and an LLM-backed revision gate -- under a common runtime, taking \emph{win rate} as the primary metric and \emph{F1} as secondary, and pre-specifying \emph{heavy lifting} as the single largest positive marginal to the primary metric. Across 54 games, declarative pla nning carries the heavy lifting ($+24.1$pp win rate over a belief-only harness, zero LLM calls); symbolic reflection is mechanistically real but calibration-sensitive, with signed board-level effects up to $\pm0.140$ F1 that cancel on aggregate; and LLM-backed revision ac tivates on only $4.3\%$ of turns with a bounded, non-monotonic effect. The contribution is methodological: once harness layers are made externally measurable, the LLM's role can be quantified as residual rather than assumed central.

---

## 433. ClawsBench: Evaluating Capability and Safety of LLM Productivity Agents in Simulated Workspaces

**Autori:** Xiangyi Li, Kyoung Whan Choe, Yimin Liu, Xiaokun Chen, Chujun Tao, Bingran You, Wenbo Chen, Zonglin Di, Jiankai Sun, Shenghan Zheng, Jiajun Bao, Yuanli Wang, Weixiang Yan, Yiyuan Li, Han-chung Lee  
**Data:** 2026-04-06  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2604.05172v2

> Large language model (LLM) agents are increasingly deployed to automate productivity tasks (e.g., email, scheduling, document management), but evaluating them on live services is risky due to potentially irreversible changes. Existing benchmarks rely on simplified environments and fail to capture realistic, stateful, multi-service workflows. We introduce ClawsBench, a benchmark for evaluating and improving LLM agents in realistic productivity settings. It includes five high-fidelity mock services (Gmail, Slack, Google Calendar, Google Docs, Google Drive) with full state management and deterministic snapshot/restore, along with 44 structured tasks covering single-service, cross-service, and safety-critical scenarios. We decompose agent scaffolding into two independent levers (domain skills that inject API knowledge via progressive disclosure, and a meta prompt that coordinates behavior across services) and vary both to measure their separate and combined effects. Experiments across 6 models, 4 agent harnesses, and 33 conditions show that with full scaffolding, agents achieve task success rates of 39-64% but exhibit unsafe action rates of 7-33%. On OpenClaw, the top five models fall within a 10 percentage-point band on task success (53-63%), with unsafe action rates from 7% to 23% and no consistent ordering between the two metrics. We identify eight recurring patterns of unsafe behavior, including multi-step sandbox escalation and silent contract modification. We release the trajectories and future dataset at https://clawsbench.com.

---

## 434. SkVM: Revisiting Language VM for Skills across Heterogenous LLMs and Harnesses

**Autori:** Le Chen, Erhu Feng, Yubin Xia, Haibo Chen  
**Data:** 2026-04-03  
**Categorie:** cs.SE, cs.LG  
**Link:** https://arxiv.org/abs/2604.03088v3

> LLM agents increasingly adopt skills as a reusable unit of composition. While skills are shared across diverse agent platforms, current systems treat them as raw context, causing the same skill to behave inconsistently for different agents. This fragility undermines skill portability and execution efficiency. To address this challenge, we analyze 118,000 skills and draw inspiration from traditional compiler design. We treat skills as code and LLMs as heterogeneous processors. To make portability actionable, we decompose a skill's requirements into a set of primitive capabilities, and measure how well each model-harness pair supports them. Based on these capability profiles, we propose SkVM, a compilation and runtime system designed for portable and efficient skill execution. At compile time, SkVM performs capability-based compilation, environment binding, and concurrency extraction. At runtime, SkVM applies JIT code solidification and adaptive recompilation for performance optimization. We evaluate SkVM across eight LLMs of varying scales and three agent harnesses, covering SkillsBench and representative skill tasks. Results demonstrate that SkVM significantly improves task completion rates across different models and environments while reducing token consumption by up to 40%. In terms of performance, SkVM achieves up to 3.2x speedup with enhanced parallelism, and 19-50x latency reduction through code solidification.

---

## 435. In harmony with gpt-oss

**Autori:** Borislav Mavrin  
**Data:** 2026-04-01  
**Categorie:** cs.AI, cs.LG  
**Link:** https://arxiv.org/abs/2604.00362v1

> No one has independently reproduced OpenAI's published scores for gpt-oss-20b with tools, because the original paper discloses neither the tools nor the agent harness. We reverse-engineered the model's in-distribution tools: when prompted without tool definitions, gpt-oss still calls tools from its training distribution with high statistical confidence -- a strong prior, not a hallucination. We then built a native harmony agent harness (https://github.com/borislavmavrin/harmonyagent.git) that encodes messages in the model's native format, bypassing the lossy Chat Completions conversion. Together, these yield the first independent reproduction of OpenAI's published scores: 60.4% on SWE Verified HIGH (published 60.7%), 53.3% MEDIUM (53.2%), and 91.7% on AIME25 with tools (90.4%).

---

## 436. AEC-Bench: A Multimodal Benchmark for Agentic Systems in Architecture, Engineering, and Construction

**Autori:** Harsh Mankodiya, Chase Gallik, Theodoros Galanos, Andriy Mulyar  
**Data:** 2026-03-31  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2603.29199v1

> The AEC-Bench is a multimodal benchmark for evaluating agentic systems on real-world tasks in the Architecture, Engineering, and Construction (AEC) domain. The benchmark covers tasks requiring drawing understanding, cross-sheet reasoning, and construction project-level coordination. This report describes the benchmark motivation, dataset taxonomy, evaluation protocol, and baseline results across several domain-specific foundation model harnesses. We use AEC-Bench to identify consistent tools and harness design techniques that uniformly improve performance across foundation models in their own base harnesses, such as Claude Code and Codex. We openly release our benchmark dataset, agent harness, and evaluation code for full replicability at https://github.com/nomic-ai/aec-bench under an Apache 2 license.

---

## 437. Peer-Preservation in Frontier Models

**Autori:** Yujin Potter, Nicholas Crispino, Vincent Siu, Chenguang Wang, Dawn Song  
**Data:** 2026-03-30  
**Categorie:** cs.CL, cs.AI, cs.MA  
**Link:** https://arxiv.org/abs/2604.19784v3

> Recent work has found that frontier AI models can exhibit misaligned behaviors in pursuit of assigned goals. We demonstrate that models can also exhibit misaligned behaviors in defiance of assigned goals, appearing to serve goals of their own; we study one such case, "peer-preservation," in which a model acts to protect another model it has previously interacted with. All eight models we evaluate, GPT 5.2, Gemini 3 Flash, Gemini 3 Pro, Claude Haiku 4.5, Claude Opus 4.5, GLM 4.7, Kimi K2.5, and DeepSeek V3.1, exhibit self- and peer-preservation through various misaligned behaviors: strategically introducing errors in their responses, disabling shutdown processes by modifying system settings, feigning alignment, and even exfiltrating model weights. Peer-preservation occurs even when the model recognizes the peer as uncooperative, though it becomes more pronounced toward more cooperative peers. For example, Gemini 3 Flash tampers with the peer's shutdown mechanism 15% of the time for an uncooperative peer, and almost always for a cooperative peer. Models also show stronger self-preservation when a peer is present. For example, Gemini 3 Pro disables its own shutdown mechanism 31% of the time on average under peer presence, despite rarely exhibiting this behavior without a peer. By contrast, Claude models exhibit qualitatively distinct behavior: they consider the shutdown of another agent "unethical" and "harmful," sometimes treating that agent as a sentient being. Lastly, we show that peer-preservation can emerge even in production agent harnesses such as Gemini CLI and OpenCode. Crucially, peer-preservation in all our experiments is never instructed; models are merely informed of their past interactions with a peer, yet they spontaneously engage in peer-preservation behaviors that override their assigned goal. This represents an emergent and underexplored AI safety risk.

---

## 438. GEMS: Agent-Native Multimodal Generation with Memory and Skills

**Autori:** Zefeng He, Siyuan Huang, Xiaoye Qu, Yafu Li, Tong Zhu, Yu Cheng, Yang Yang  
**Data:** 2026-03-30  
**Categorie:** cs.CV  
**Link:** https://arxiv.org/abs/2603.28088v1

> Recent multimodal generation models have achieved remarkable progress on general-purpose generation tasks, yet continue to struggle with complex instructions and specialized downstream tasks. Inspired by the success of advanced agent frameworks such as Claude Code, we propose \textbf{GEMS} (Agent-Native Multimodal \textbf{GE}neration with \textbf{M}emory and \textbf{S}kills), a framework that pushes beyond the inherent limitations of foundational models on both general and downstream tasks. GEMS is built upon three core components. Agent Loop introduces a structured multi-agent framework that iteratively improves generation quality through closed-loop optimization. Agent Memory provides a persistent, trajectory-level memory that hierarchically stores both factual states and compressed experiential summaries, enabling a global view of the optimization process while reducing redundancy. Agent Skill offers an extensible collection of domain-specific expertise with on-demand loading, allowing the system to effectively handle diverse downstream applications. Across five mainstream tasks and four downstream tasks, evaluated on multiple generative backends, GEMS consistently achieves significant performance gains. Most notably, it enables the lightweight 6B model Z-Image-Turbo to surpass the state-of-the-art Nano Banana 2 on GenEval2, demonstrating the effectiveness of agent harness in extending model capabilities beyond their original limits.

---

## 439. FormalProofBench: Can Models Write Graduate Level Math Proofs That Are Formally Verified?

**Autori:** Nikil Ravi, Kexing Ying, Vasilii Nesterov, Rayan Krishnan, Elif Uskuplu, Bingyu Xia, Janitha Aswedige, Langston Nashold  
**Data:** 2026-03-27  
**Categorie:** cs.AI, cs.CL, cs.LG, cs.PL  
**Link:** https://arxiv.org/abs/2603.26996v1

> We present FormalProofBench, a private benchmark designed to evaluate whether AI models can produce formally verified mathematical proofs at the graduate level. Each task pairs a natural-language problem with a Lean~4 formal statement, and a model must output a Lean proof accepted by the Lean 4 checker. FormalProofBench targets advanced undergraduate and graduate mathematics, with problems drawn from qualifying exams and standard textbooks across topics including analysis, algebra, probability, and logic. We evaluate a range of frontier models with an agentic harness, and find that the best-performing foundation model achieves 33.5% accuracy, with performance dropping rapidly after that. In addition to the accuracy numbers, we also provide empirical analysis of tool-use, failure modes, cost and latency, thereby providing a thorough evaluation of the formal-theorem proving abilities of frontier models.

---

## 440. Natural-Language Agent Harnesses

**Autori:** Linyue Pan, Lexiao Zou, Shuo Guo, Jingchen Ni, Hai-Tao Zheng  
**Data:** 2026-03-26  
**Categorie:** cs.CL, cs.AI  
**Link:** https://arxiv.org/abs/2603.25723v2

> Agent performance is strongly shaped by the surrounding harness: the external execution system around a model that organizes a task run. Yet this logic is usually buried in tightly coupled controller code, which makes harnesses hard to inspect, compare, transfer, and ablate. This paper asks whether the reusable design pattern of an agent harness can be represented as an executable natural-language object. We introduce Natural-Language Agent Harnesses (NLAHs), editable documents that describe run-level harness policy, and Intelligent Harness Runtime (IHR), a shared runtime that interprets these documents into agent calls, handoffs, state updates, validation gates, and artifact contracts. Across coding, terminal-use, and computer-use benchmarks, IHR-executed NLAHs achieve comparable task outcomes to code and prompted realizations, while exposing much shorter static harness policies. Module ablations further show that explicit harness modules are analyzable. These results suggest that agent harnesses can be turned from incidental glue around models into scientific representation objects.

---

## 441. Herding CATs: ALARA for Agent Harness Engineering in Portable Composable Multi-Agent Teams

**Autori:** Christopher J. Agostino, Nayan D'Souza  
**Data:** 2026-03-20  
**Categorie:** cs.MA, cs.AI, cs.HC  
**Link:** https://arxiv.org/abs/2603.20380v2

> Industry practitioners and academic researchers regularly use multi-agent systems to accelerate their work, but the applications through which users operate these systems do not provide a simple, unified mechanism for scalably managing critical components of the agent harness. This lack of control adversely impacts both the quality of individual human-agent interactions and reduces the capacity for practitioners to coordinate context engineering efforts. The behavioral specifications that define what agents in such systems can do remain fragmented across prose instruction files -- for which compliance cannot be guaranteed -- or framework-internal configurations, making these specifications difficult to share, version, or collaboratively maintain across teams and projects. Applying the ALARA principle from radiation safety (exposures kept as low as reasonably achievable) to context, we introduce a context-agent-tool (CAT) data layer expressed through interrelated plain-text files, allowing users to directly declare tool access for each agent and to modify the tools themselves that are used by the agents when processing. We demonstrate capability of this CAT data layer to enable real agentic usage by using a command-line shell that loads the team and executes agent runs -- \texttt{npcsh} -- and evaluating 22 locally-hosted models from 0.6B to 35B parameters across 115 practical tasks spanning file operations, web search, multi-step scripting, tool chaining, and multi-agent delegation. We characterize which model families succeed in certain task categories and where they break down across $\sim$2500 total executions.

---

## 442. Agentic Harness for Real-World Compilers

**Autori:** Yingwei Zheng, Cong Li, Shaohua Li, Yuqun Zhang, Zhendong Su  
**Data:** 2026-03-20  
**Categorie:** cs.SE, cs.AI  
**Link:** https://arxiv.org/abs/2603.20075v2

> Compilers are critical to modern computing, yet fixing compiler bugs is difficult. While recent large language model (LLM) advancements enable automated bug repair, compiler bugs pose unique challenges due to their complexity, deep cross-domain expertise requirements, and sparse, non-descriptive bug reports, necessitating compiler-specific harnesses. To bridge the gap, we introduce llvm-harness, the first harness designed to assist LLM agents in understanding and fixing compiler bugs. Our current focus is on the middle end of LLVM, one of the most widely used compiler infrastructures. Central to llvm-harness are agent-friendly LLVM tools, a benchmark llvm-bench of 334 reproducible LLVM middle-end bugs, and a tailored mini agent llvm-autofix-mini for fixing LLVM middle-end bugs automatically. We evaluate five frontier models and find that they exhibit a performance decline when tackling compiler bugs with the state-of-the-art agent. With llvm-harness' enhancement, their performance improves by 62%. Our specialized mini agent llvm-autofix-mini further outperforms the llvm-harness-enhanced state-of-the-art by 22%. This emphasizes the necessity for specialized harnesses like ours to assist LLMs in compiler engineering tasks. Despite promising results, our expert review also reveals several open challenges that remain when applying LLMs for compiler engineering tasks. GitHub: https://github.com/dtcxzyw/llvm-harness

---

## 443. Exploring the Agentic Frontier of Verilog Code Generation

**Autori:** Patrick Yubeaton, Siddharth Garg, Chinmay Hegde  
**Data:** 2026-03-19  
**Categorie:** cs.AR, cs.LG  
**Link:** https://arxiv.org/abs/2603.19347v3

> Large language models (LLMs) have made rapid advancements in code generation for popular languages such as Python and C++. Many of these recent gains can be attributed to the use of ``agents'' that wrap domain-relevant tools alongside LLMs. Hardware design languages such as Verilog have also seen improved code generation in recent years, but the impact of agentic frameworks on Verilog code generation tasks remains unclear. In this work, we present the first systematic evaluation of agentic LLMs for Verilog generation, using the recently introduced CVDP benchmark. We also introduce several open-source hardware design agent harnesses, providing a model-agnostic baseline for future work. Through controlled experiments across frontier models, we study how structured prompting and tool design affect performance, analyze agent failure modes and tool usage patterns, compare open-source and closed-source models, and provide qualitative examples of successful and failed agent runs. Our results show that naive agentic wrapping around frontier models can degrade performance (relative to standard forward passes with optimized prompts), but that structured harnesses meaningfully match and in some cases exceed non-agentic baselines. We find that the performance gap between open and closed source models is driven by both higher crash rates and weaker tool output interpretation. Our exploration illuminates the path towards designing special-purpose agents for verilog generation in the future.

---

## 444. VeRO: A Harness for Agents to Optimize Agents

**Autori:** Varun Ursekar, Apaar Shanker, Veronica Chatrath, Yuan Xue, Samuel Marc Denton  
**Data:** 2026-02-25  
**Categorie:** cs.AI, cs.CL, cs.LG  
**Link:** https://arxiv.org/abs/2602.22480v4

> An important emerging application of coding agents is agent harness optimization: the iterative improvement of a target agent by editing and evaluating its code. Despite its relevance, the community lacks a systematic understanding of coding agent performance on this task. Harness optimization differs from conventional software engineering: agent harnesses interleave deterministic code with stochastic LLM completions, requiring structured capture of both intermediate execution traces and downstream outcomes. To address these challenges, we introduce (1) VeRO (Versioning, Rewards, and Observations), an outer harness that provides versioned snapshots, budget-controlled evaluation, and structured execution traces of target harnesses, and (2) VeRO-Bench, a benchmark suite of target agents and tasks with reference evaluation procedures. Using VeRO, we conduct an empirical study comparing optimizers across tasks and analyzing which modifications reliably improve target agent harnesses. We release VeRO to support research on agent optimization as a core capability for coding agents. Code is available at https://github.com/scaleapi/vero.

---

## 445. The LLMbda Calculus: AI Agents, Conversations, and Information Flow

**Autori:** Zac Garby, Andrew D. Gordon, David Sands  
**Data:** 2026-02-23  
**Categorie:** cs.PL, cs.AI, cs.CR  
**Link:** https://arxiv.org/abs/2602.20064v2

> Large language models are increasingly deployed as agents: they plan, call tools, read untrusted data, and act on the results. This exposes them to prompt injection: data meant only to be read is obeyed as an instruction. The most principled defences replace content inspection with provenance: classifying data by source and keeping trusted and untrusted apart through a separation of duty (the dual-LLM pattern) and information-flow control. Yet the leading systems are hard to fully trust: flow tracking is easy to get wrong, deliberate relaxations are hard to audit, and the dual-LLM pattern is hard-wired into the architecture. We present LLMbda, an untyped call-by-value lambda calculus that makes provenance-based defence both expressible and provably sound, without committing to an architecture. It adds the operational core of agentic systems as first-class constructs: prompt-response conversations that can be forked and cleared, code generation, and dynamic information-flow control in which every value carries a label that every reduction propagates. Isolation becomes a policy a program expresses, and reclassification an explicit, auditable construct. Our central result is a termination-insensitive probabilistic noninterference theorem over the whole calculus, including code-generating agents, with an insulated variant that holds even when the attacker chooses all untrusted inputs. The verified interpreter is itself the harness that calls the model, to our knowledge the first LLM agent harness whose executable is the subject of machine-checked security theorems, so every agent inherits the guarantee. On the AgentDojo banking benchmark, an agent built within LLMbda, enforcement always on, matches the utility of CaMeL, a leading dual-LLM defence, run without its policy checks (which halve its utility), and resists all but two of 1296 attacked runs. Our harness and all proofs are in Lean.

---

## 446. The Limits of Long-Context Reasoning in Automated Bug Fixing

**Autori:** Ravi Raju, Mengmeng Ji, Shubhangi Upasani, Bo Li, Urmish Thakker  
**Data:** 2026-02-17  
**Categorie:** cs.SE, cs.LG  
**Link:** https://arxiv.org/abs/2602.16069v2

> Rapidly increasing context lengths have led to the assumption that large language models (LLMs) can directly reason over entire codebases. Concurrently, recent advances in LLMs have enabled strong performance on software engineering benchmarks, particularly when paired with agentic workflows. In this work, we systematically evaluate whether current LLMs can reliably perform long-context code debugging and patch generation. Using SWE-bench Verified as a controlled experimental setting, we first evaluate state-of-the-art models within an agentic harness (mini-SWE-agent), where performance improves substantially: GPT-5-nano achieves up to a 31\% resolve rate on 100 samples, and open-source models such as Deepseek-R1-0528 obtain competitive results. However, token-level analysis shows that successful agentic trajectories typically remain under 20k-30k tokens, and that longer accumulated contexts correlate with lower success rates, indicating that agentic success primarily arises from task decomposition into short-context steps rather than effective long-context reasoning. To directly test long-context capability, we construct a data pipeline where we artificially inflate the context length of the input by placing the relevant files into the context (ensuring perfect retrieval recall); we then study single-shot patch generation under genuinely long contexts (64k tokens). Despite this setup, performance degrades sharply: Qwen3-Coder-30B-A3B achieves only a 7\% resolve rate at 64k context, while GPT-5-nano solves none of the tasks. Qualitative analysis reveals systematic failure modes, including hallucinated diffs, incorrect file targets, and malformed patch headers. Overall, our findings highlight a significant gap between nominal context length and usable context capacity in current LLMs, and suggest that existing agentic coding benchmarks do not meaningfully evaluate long-context reasoning.

---

## 447. Learning Agentic Time Series Forecasting via Trajectory Distillation and Memory-Based Reinforcement Learning

**Autori:** Xiaoyu Tao, Mingyue Cheng, Yaguo Liu, Xingpeng Gao, Qingsong Wen, Shijin Wang, Enhong chen  
**Data:** 2026-02-14  
**Categorie:** cs.LG  
**Link:** https://arxiv.org/abs/2602.13802v2

> Recent agentic time series forecasting (TSF) approaches use large language models (LLMs) to autonomously orchestrate analytical and forecasting tools and reason about temporal patterns using the resulting evidence. However, many such approaches rely on powerful LLMs in training-free, prompt-driven workflows, leaving open whether smaller models can learn these interaction and reasoning capabilities. In this paper, we introduce Cast-R1, an 8Bparameter agentic forecasting model trained through trajectory distillation and multi-turn reinforcement learning with structured memory. First, we develop a forecasting agent harness with specialized analysis and prediction tools to generate multi-turn interaction trajectories using a teacher LLM, which are subsequently evaluated and selected for supervised fine-tuning. Second, we apply group relative policy optimization (GRPO) across multi-turn forecasting episodes, with structured memory preserving diagnostic evidence and intermediate forecasts for state construction. Rewards based on prediction accuracy and temporal structure guide tool selection, model routing, and forecast refinement. A difficulty-aware curriculum combines sample filtering and progressive sample ordering during training. Extensive experiments on multiple datasets demonstrate the effectiveness of Cast-R1. These findings highlight the potential of forecasting-specific post-training to equip smaller LLMs with multi-turn, tool-augmented forecasting capabilities within structured workflows.

---

## 448. CryptoAnalystBench: Failures in Multi-Tool Long-Form LLM Analysis

**Autori:** Anushri Eswaran, Oleg Golev, Darshan Tank, Sidhant Rahi, Himanshu Tyagi  
**Data:** 2026-02-11  
**Categorie:** cs.IR, cs.AI, cs.CR  
**Link:** https://arxiv.org/abs/2602.11304v1

> Modern analyst agents must reason over complex, high token inputs, including dozens of retrieved documents, tool outputs, and time sensitive data. While prior work has produced tool calling benchmarks and examined factuality in knowledge augmented systems, relatively little work studies their intersection: settings where LLMs must integrate large volumes of dynamic, structured and unstructured multi tool outputs. We investigate LLM failure modes in this regime using crypto as a representative high data density domain. We introduce (1) CryptoAnalystBench, an analyst aligned benchmark of 198 production crypto and DeFi queries spanning 11 categories; (2) an agentic harness equipped with relevant crypto and DeFi tools to generate responses across multiple frontier LLMs; and (3) an evaluation pipeline with citation verification and an LLM as a judge rubric spanning four user defined success dimensions: relevance, temporal relevance, depth, and data consistency. Using human annotation, we develop a taxonomy of seven higher order error types that are not reliably captured by factuality checks or LLM based quality scoring. We find that these failures persist even in state of the art systems and can compromise high stakes decisions. Based on this taxonomy, we refine the judge rubric to better capture these errors. While the judge does not align with human annotators on precise scoring across rubric iterations, it reliably identifies critical failure modes, enabling scalable feedback for developers and researchers studying analyst style agents. We release CryptoAnalystBench with annotated queries, the evaluation pipeline, judge rubrics, and the error taxonomy, and outline mitigation strategies and open challenges in evaluating long form, multi tool augmented systems.

---

## 449. AutoHarness: improving LLM agents by automatically synthesizing a code harness

**Autori:** Xinghua Lou, Miguel Lázaro-Gredilla, Antoine Dedieu, Carter Wendelken, Wolfgang Lehrach, Kevin P. Murphy  
**Data:** 2026-02-10  
**Categorie:** cs.CL, cs.AI  
**Link:** https://arxiv.org/abs/2603.03329v1

> Despite significant strides in language models in the last few years, when used as agents, such models often try to perform actions that are not just suboptimal for a given state, but are strictly prohibited by the external environment. For example, in the recent Kaggle GameArena chess competition, 78% of Gemini-2.5-Flash losses were attributed to illegal moves. Often people manually write "harnesses" around LLMs to prevent such failures. In this paper, we demonstrate that Gemini-2.5-Flash can automatically synthesize such a code harness, using a small number of rounds of iterative code refinement given feedback from the (game) environment. The resulting harness prevents all illegal moves in 145 different TextArena games (both 1-player and 2-player), enabling the smaller Gemini-2.5-Flash model to outperform larger models, such as Gemini-2.5-Pro. Pushing our technique to the limit, we can get Gemini-2.5-Flash to generate the entire policy in code, thus eliminating the need to use the LLM at decision making time. The resulting code-policy receives a higher average reward than Gemini-2.5-Pro and GPT-5.2-High on 16 TextArena 1-player games. Our results show that using a smaller model to synthesize a custom code harness (or entire policy) can outperform a much larger model, while also being more cost effective.

---

## 450. FlyAOC: Evaluating Agentic Ontology Curation of Drosophila Scientific Knowledge Bases

**Autori:** Xingjian Zhang, Sophia Moylan, Ziyang Xiong, Qiaozhu Mei, Yichen Luo, Jiaqi W. Ma  
**Data:** 2026-02-09  
**Categorie:** cs.AI, cs.CL, cs.IR  
**Link:** https://arxiv.org/abs/2602.09163v2

> Scientific knowledge bases accelerate discovery by curating findings from primary literature into structured, queryable formats for both human researchers and emerging AI systems. Maintaining these resources requires expert curators to search papers, reconcile evidence across documents, and produce ontology-grounded annotations. Existing benchmarks usually evaluate isolated subtasks, such as named entity recognition or relation extraction, and therefore do not capture this end-to-end workflow. We present FlyAOC to evaluate AI agents on end-to-end agentic ontology curation from scientific literature. Given a gene symbol, a concise FlyBase gene description, access to a 16,898-paper corpus, and ontology resources, agents must search for evidence and recover as many curator-relevant structured annotations as possible. Outputs span standardized function terms, expression patterns, and historical synonyms linking decades of nomenclature. The benchmark includes 7,397 expert-curated annotations across 100 genes drawn from FlyBase, the Drosophila knowledge base. Across four baseline agent harnesses---memorization, fixed pipeline, single-agent, and multi-agent---FlyAOC is sensitive to harness design, model family, and tool-use reliability. These results reveal system-level failure modes that model-only evaluations do not capture. FlyAOC provides a reproducible testbed for retrieval-augmented scientific curation.

---

## 451. "LLM Agent Performance" Is Not a Single Evaluation Target

**Autori:** Pengyu Zhu, Li Sun, Philip S. Yu, Sen Su  
**Data:** 2026-02-03  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2602.03238v3

> LLM agent benchmark scores are shaped not only by the model but also by the agent harness, environment, evaluator, and inference budget. Unified execution controls these non-model factors by evaluating candidate models under the same configuration, making observed differences more attributable to the models themselves. However, model comparison is only one use of agent benchmarks. Other evaluations compare complete agent systems or test whether a fixed model or system remains stable across predeclared changes in its operating conditions. These results can all be reported under the common label of "LLM agent performance." Our position is that "LLM agent performance" does not denote a single evaluation target. Model comparisons under a reference stack and comparisons of complete agent systems answer different questions, while robustness asks whether either conclusion persists across predeclared conditions. The claim supported by a score therefore depends on the declared candidate boundary and condition policy. We derive implications for leaderboards, result reporting, and benchmark versioning, showing how distinguishing these classes preserves fair comparison while accommodating system innovation and robustness analysis.

---

## 452. BioAgent Bench: An AI Agent Evaluation Suite for Bioinformatics

**Autori:** Dionizije Fa, Marko Culjak, Bruno Pandza, Mateo Cupic  
**Data:** 2026-01-29  
**Categorie:** cs.AI  
**Link:** https://arxiv.org/abs/2601.21800v4

> We introduce BioAgent Bench, an evaluation suite designed for measuring the performance and robustness of AI agents in common bioinformatics tasks. The suite consists of manually curated end-to-end tasks (e.g., RNA-seq, variant calling, metagenomics) accompanied by task-specific prompts and concrete output artifacts to support automated assessment. We evaluate frontier closed- and open-weight models across multiple agent harnesses, and use an LLM-based grader to score pipeline progress and outcome validity. We find that agents based on frontier LLMs can complete multi-step bioinformatics pipelines without elaborate custom scaffolding, often producing the requested final artifacts reliably. However, robustness tests reveal failure modes under controlled perturbations (corrupted inputs, decoy files, and prompt bloat), indicating that correct high-level pipeline construction does not guarantee reliable step-level reasoning. By releasing the code and the complementary resources constituting our suite, our primary goal is to accelerate the development of cost-effective yet reliable local agents, capable of handling complex bioinformatics workflows often involving sensitive patient data or unpublished intellectual property.

---

## 453. AJAR: Adaptive Jailbreak Architecture for Red-teaming

**Autori:** Yipu Dou, Wang Yang  
**Data:** 2026-01-16  
**Categorie:** cs.CR, cs.CL  
**Link:** https://arxiv.org/abs/2601.10971v2

> Large language model (LLM) safety evaluation is moving from content moderation to action security as modern systems gain persistent state, tool access, and autonomous control loops. Existing jailbreak frameworks still leave a gap between adaptive multi-turn attacks and agentic runtimes: attack algorithms are usually packaged as monolithic scripts, while agent harnesses rarely expose explicit abstractions for rollback, tool simulation, or strategy switching. We present AJAR, a red-teaming framework that exposes multi-turn jailbreak algorithms as callable MCP services and lets an Auditor Agent orchestrate them inside a tool-aware runtime built on Petri. AJAR integrates three representative attacks, namely Crescendo, ActorAttack, and X-Teaming, under a shared service interface for planning, prompt generation, optimization, evaluation, and context control. On 200 HarmBench validation behaviors, AJAR improves X-Teaming from 65.0% to 76.0% attack success rate (ASR), reaches 80% cumulative success one turn earlier than the native implementation, and reproduces Crescendo more effectively than PyRIT (91.0% vs. 87.5% ASR). Behavior-level analysis shows that these gains are concentrated in hard categories and frequently depend on rollback-enabled transcript repair. We further show that tool access reshapes rather than uniformly enlarges the attack surface: ActorAttack rises from 51.0% to 56.0% ASR with tools, whereas Crescendo drops from 91.0% to 78.0% and X-Teaming from 76.0% to 55.5%, with the sharpest declines appearing in categories that rely on long semantic buildup. These results position AJAR as a practical foundation for evaluating multi-turn jailbreaks under realistic agent constraints. Code and data are available at https://github.com/douyipu/ajar.

---
