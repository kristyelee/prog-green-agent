Resources.md
    [Notes[AgentBeats].md]

https://rdi.berkeley.edu/assets/agentbeats-competition-info-session-deck.pdf
Type 1: Integrating Existing Benchmarks
• Goal: Adapt an existing benchmark (already published/tested) and
integrate as a assessor agent in AgentBeats
– E.g. SWE-bench Verified, Terminal bench
• Largely reuse existing evaluation metrics or rubrics
• Sample ideas:
https://docs.google.com/presentation/d/1TjtEjh6g9dZBsGxmAmcSp2
EFakbmHpU_z31vnkf0c2Y/
Type 1: Integrating Existing Benchmarks
Main Workflows:#
• Step 1: Integration
– Convert problem formats to correct format like A2A
– Implement dataset loaders & interfaces
– Add quality checks for correctness & reproducibility
• Step 2: Benchmark Quality Analysis
• Step 3: Correction and Expansion
Type 1: Integrating Existing Benchmarks
Main Workflows:
• Step 1: Integration
• Step 2: Benchmark Quality Analysis: check the quality and reliability
of the existing benchmark.
– Manual Validation: Sample and check data correctness, clarity, and difficulty
– Evaluator Check: Confirm metrics/judges align with true task success
– Bias & Limitation Notes: Highlight any gaps or weaknesses
• Step 3: Correction and Expansion
Type 1: Integrating Existing Benchmarks
Main Workflows:
• Step 1: Integration
• Step 2: Benchmark Quality Analysis
• Step 3: Correction and Expansion
– Correct the benchmark if there are errors
– Expand the benchmark to improve its quality, size, and diversity.
SWE-bench and SWE-bench Verified
https://openai.com/index/introducing-swe-bench-verified/
• Problem (Original SWE-bench):
– Some tasks had underspecified issue descriptions or overly specific/misaligned
tests; setup friction sometimes caused false negatives.
• Correction:
– Added human verification by 93 professional developers on 1,699 samples
• Issues flagged: 38.3% underspecification, 61.1% unfair unit tests; total 68.3%
of samples filtered out
– Filtered to 500 verified tasks
• Outcome:
– Curated a higher-quality subset with enhanced task diversity and difficulty balance
– More trustworthy, replicable, and comprehensive benchmark
• GPT-4o reaches 33.2% resolved on Verified (vs. 16% on original using best scaffold),
indicating prior underestimation of capability.

Type 2: Building New Benchmarks
• Create new benchmarks (no existing source)
• Realistic daily tasks → showcase agentic reasoning
Type 2: Building New Benchmarks
• Tasks should reflect useful, real-world scenarios
– e.g., organize calendar, schedule meetings, manage to-dos
• Evaluation: Automatic or lightweight human checks
• We encourage you to build multi-agent benchmarks (e.g., Synthesizer
+ Analyzer roles)

Log -
    https://www.youtube.com/watch?v=ZmBnC4xTyRU [AgentX-AgentBeats Developer Platform Tutorial] 
        https://github.com/agentbeater/Tau2-Bench/tree/5dd9506d54641b52064f1193111cd3044d1282e0 [Scenario, Submission]
        https://agentbeats.dev/agentbeater/tau2-bench 
            Agent ID: 019b4d06-1da3-7c22-88fa-f4660061a779
            Docker Image: ghcr.io/rdi-foundation/agentbeats-tutorial-tau2-evaluator:latest

        https://agentbeats.dev/agentbeater/tau2-agent
            Agent ID: 019b4d08-d84c-7a00-b2ec-4905ef7afc96
            Docker Image: ghcr.io/rdi-foundation/agentbeats-tutorial-tau2-agent:latest
    
    https://google.github.io/adk-docs/a2a/intro/#next-steps
    
    https://docs.agentbeats.dev
    https://docs.agentbeats.dev/tutorial/
        https://docs.github.com/en/packages/working-with-a-github-packages-registry/working-with-the-container-registry
