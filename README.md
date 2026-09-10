# CI Papers

A reading list on continuous integration, focusing on regression testing and continuous formal verification.

## LLM-based Regression Testing

- **[Just-in-Time Catching Test Generation at Meta](https://arxiv.org/pdf/2601.22832)** — FSE 2026, Industry.
  Matthew Becker et al., Meta.

  Generates tests for proposed code changes in Meta's CI workflow to catch regressions before they land. The focus is on understanding change intent and distinguishing real bugs from false positives without slowing down developers.

- **[Evaluating LLM-Based Regression Test Generation](https://nimgnoeseel.github.io/assets/pdf/llm-regression-paper.pdf)** — FSE 2026.
  Jing Liu, Seongmin Lee, Eleonora Losiouk, and Marcel Böhme; MPI-SP, UCLA, and the University of Padua.

  Studies commit-specific regression test generation within a short CI budget. Cleverest uses commit messages, code changes, and execution feedback; ClevFuzz uses the generated tests as fuzzing seeds. The evaluation covers both bug-introducing and bug-fixing commits.

## Code and Configuration Changes

- **[Test Selection for Unified Regression Testing](https://tianyin.github.io/pub/urts.pdf)** — ICSE 2023.
  Shuai Wang, Xinyu Lian, Darko Marinov, and Tianyin Xu; UIUC.

  Selects regression tests for code changes, production configuration changes, and their combination in CI/CD. uRTS tracks code and configuration dependencies across revisions and configurations to reduce end-to-end testing time while preserving the safety guarantees of existing regression test selection techniques.

## Continuous Formal Verification

- **[Code-Level Model Checking in the Software Development Workflow at Amazon Web Services](https://cdn.amazon.science/4d/b0/504a2bbf4f3db18d98e37b8580df/code-level-model-checking-in-the-software-development-workflow-at-amazon-web-services.pdf)** — Software: Practice and Experience, 2021.
  Nathan Chong et al., AWS and academic collaborators.

  Integrates CBMC proof harnesses and specifications into ordinary development and CI, rechecking properties as code changes. Section 6 describes the continuous verification infrastructure, including feedback latency, parallel execution, and resource requirements.

- **[Continuous Reasoning: Scaling the Impact of Formal Methods](https://discovery.ucl.ac.uk/id/eprint/10074600/7/O%27Hearn_Continuous%20reasoning.%20Scaling%20the%20impact%20of%20formal%20methods_VoR.pdf)** — LICS 2018, Invited Paper.
  Peter W. O'Hearn, Facebook and UCL.

  Examines how automated reasoning can follow a changing codebase and provide timely feedback through CI and code review. Draws on industrial experience with Infer to discuss incremental analysis, scalability, and developer adoption.
