# CI Papers

A reading list on continuous integration, focusing on LLM-based regression testing and continuous formal verification.

## LLM-based Regression Testing

- **Just-in-Time Catching Test Generation at Meta** — FSE 2026, Industry.
  Matthew Becker et al., Meta.
  [Paper](https://arxiv.org/abs/2601.22832) · [PDF](https://arxiv.org/pdf/2601.22832)

  Generates tests for proposed code changes in Meta's CI workflow to catch regressions before they land. The focus is on understanding change intent and distinguishing real bugs from false positives without slowing down developers.

- **Evaluating LLM-Based Regression Test Generation** — FSE 2026.
  Jing Liu, Seongmin Lee, Eleonora Losiouk, and Marcel Böhme; MPI-SP, UCLA, and the University of Padua.
  [Paper](https://doi.org/10.1145/3808129) · [PDF](https://nimgnoeseel.github.io/assets/pdf/llm-regression-paper.pdf)

  Studies commit-specific regression test generation within a short CI budget. Cleverest uses commit messages, code changes, and execution feedback; ClevFuzz uses the generated tests as fuzzing seeds. The evaluation covers both bug-introducing and bug-fixing commits.

## Continuous Formal Verification

- **Code-Level Model Checking in the Software Development Workflow at Amazon Web Services** — Software: Practice and Experience, 2021.
  Nathan Chong et al., AWS and academic collaborators.
  [Paper](https://doi.org/10.1002/spe.2949) · [Open-access version](https://discovery.ucl.ac.uk/id/eprint/10131088/)

  Integrates CBMC proof harnesses and specifications into ordinary development and CI, rechecking properties as code changes. Section 6 describes the continuous verification infrastructure, including feedback latency, parallel execution, and resource requirements.

- **Continuous Reasoning: Scaling the Impact of Formal Methods** — LICS 2018, Invited Paper.
  Peter W. O'Hearn, Facebook and UCL.
  [Paper](https://doi.org/10.1145/3209108.3209109) · [Open-access version](https://discovery.ucl.ac.uk/id/eprint/10074600/)

  Examines how automated reasoning can follow a changing codebase and provide timely feedback through CI and code review. Draws on industrial experience with Infer to discuss incremental analysis, scalability, and developer adoption.
