# LLM training digest

**End-to-end LLM fine-tuning process: from dataset to evaluation and cost analysis**

This repository publishes PDF digests on **applied fine-tuning of small LLMs**: choosing a base model and training mode, training data and validation, infrastructure, metrics, risks, and how quality, time, and cost of a run fit together.

## TL;DR

- **Structured training pipeline** — explicit stages from dataset checks through GPU provisioning, monitored training, artifact retrieval, inference deployment, to post-training evaluation.
- **Dataset-driven behavior shaping** — data format, preparation, and balance define what the model reinforces; train, trainer-eval, and holdout sets stay separated to avoid misleading metrics.
- **Evaluation as a decision gate** — quality is judged on a dedicated holdout run via inference, not only on `eval_loss` inside training.
- **Cost & time breakdown** — wall-clock and spend include validation, provisioning, training, artifacts, inference, evaluation, and rerun risk—not just GPU training hours.
- **Reproducibility** — tracking, checkpoints/adapters, and a clear run lifecycle keep experiments comparable and debuggable.

## Pipeline overview

High-level stage flow (same idea as in the digest, §4 *Training flow*):

<p align="center">
  <img src="assets/pipeline_stage_flow_vertical.svg" width="400" alt="Pipeline stage flow: Dataset Validator, GPU Deployer, Training Monitor, Model Retriever, Inference Deployer, Model Evaluator" />
</p>

## Files

| File | Language |
|------|----------|
| [Дайджест по обучению небольших ЛЛМ.pdf](./Дайджест%20по%20обучению%20небольших%20ЛЛМ.pdf) | Russian |
| [Digest on training small LLMs.pdf](./Digest%20on%20training%20small%20LLMs.pdf) | English |

Both PDFs are the same research: a technical engineering narrative (not a code walkthrough). Diagram source: D2 `pipeline_stage_flow_vertical` used in the document.

## Author

**Golikov Daniil**

- GitHub: [@DanilGolikov](https://github.com/DanilGolikov)
- X: [@DaniilGolikoff](https://x.com/DaniilGolikoff)
- Telegram: [@daniil_golikoff](https://t.me/daniil_golikoff)
- Email: [daniil.golikoff@gmail.com](mailto:daniil.golikoff@gmail.com)

## License

Content is provided for reference and education. If you reuse or cite the material, please attribute the author.
