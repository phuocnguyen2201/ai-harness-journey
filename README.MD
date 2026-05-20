# AI Harness — Personal Learning Journey

This repository captures my personal learning journey building and experimenting with "AI harness" techniques — tools, patterns, and projects that help me reliably develop, evaluate, and deploy AI systems.

## About

- **Owner:** Personal learning and experiments
- **Focus:** Practical experiments with model harnessing, evaluation pipelines, prompt engineering, and production-readiness practices.

## Learning Goals

- Understand prompt engineering and instruction tuning
- Build simple evaluation harnesses and metrics
- Automate model benchmarking and comparison
- Explore safe deployment patterns and monitoring

## Milestones & Progress

- [x] Initial repo and notes
- [ ] Implement basic evaluation harness
- [ ] Add example projects and notebooks
- [ ] Create CI checks for model performance

## Resources

- Papers, blog posts, and notebooks collected during experiments
- Small scripts and examples to reproduce results

## How to Use

Add notes, experiments, and small runnable examples here. Keep each experiment self-contained with a README and usage instructions.

---

If you'd like, I can add a starter example, notebook, or a simple benchmarking script next.

## Inspired by Learn Harness Engineering

This repository is inspired by the "Learn Harness Engineering" course from Walking Labs. See the full course for lectures, projects, and copy-ready templates: https://walkinglabs.github.io/learn-harness-engineering/en/

Key concepts adapted from the course:

- A harness is a closed-loop system that makes model outputs actionable and verifiable.
- Core workflow: initialize, run tasks, collect runtime feedback, verify with tests, and cleanup/handoff.
- Design primitives: explicit rules/boundaries, feature lists, initialization phase, and in-harness observability.
- Emphasis on end-to-end verification, preventing premature agent "victory", and maintaining session continuity.

Recommended next steps from the course: follow the lectures for theory, complete hands-on projects, and reuse the provided templates (AGENTS.md, feature_list.json) in experiments.

