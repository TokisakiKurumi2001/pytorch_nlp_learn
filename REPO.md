# Useful repositories

Further work can rely on these repositories to save time and effort

## Multiple evaluation metrics

Use for evaluating the paraphrase generation task.

Metrics include
- BERTScore
- ParaScore
- BERT-iBLEU
- SacreBLEU
- TER

[multi_eval](https://github.com/TokisakiKurumi2001/multi_eval)

## Learning rate scheduler with PL

Use to experiment the learning rate scheduler

[lrs](https://github.com/TokisakiKurumi2001/LRS)

## DeepSpeed Full Training

This repo not only fine-tunes the LLM with deepspeed (Zero-3) but also provides some estimation on the resources needed.

```text
For 1.5B, use zero3.json is enough. GPU: 4, RAM: 128GB, CPU: 20 cores
For 7B, use zero3_offload.json to transfer both optimizer and model's parameter to CPU. GPU: 4, RAM: 256GB, CPU: 64 cores
```

[ds3](https://github.com/TokisakiKurumi2001/ds3)

## Helpful HF codes

Store helpful codes for working with HF

[hf_helper](https://github.com/TokisakiKurumi2001/hf_helper)

## Importance scoring for layer, channel and weight of model

[importance](https://github.com/TokisakiKurumi2001/importance)

## Language model evaluation

A working LM-Eval Framework.

[lm_eval](https://github.com/TokisakiKurumi2001/lm_eval)

## Record pip's dependency while using conda

[record_pip](https://github.com/TokisakiKurumi2001/record_pip)

Edit the `~/.bashrc`
```bash
alias rpip="python path/to/record.py"
```

## Llama factory based repo

Fine-tuning LoRA or Full, Deepspeed tp DDP. The Llama factory has many features that supports training with litte modifications, just changing the data path or creating custom trainer.

[base_llm_factory](https://github.com/TokisakiKurumi2001/base-llm-factory)

<details>
  <summary>Inventories</summary>
  
  - [OREO](https://github.com/TokisakiKurumi2001/oreo_llm_factory)
  - [GKD & GRPO](https://github.com/TokisakiKurumi2001/grpo_llm_factory)
  - [MeZO](https://github.com/TokisakiKurumi2001/mezo_llm_factory)

</details>

## LLM-as-a-judge inference on clouds

Perform LLM-as-a-Judge on the cloud using the HF-Inference.

Support different features:
1. Extend the main class to perform customed generation.
2. Register new prompts

[lite_llm_judges](https://github.com/TokisakiKurumi2001/judges)

## Test-time compute

Computation shifted from training to testing.

Using verifier/score/reward model to credit each token generated and choose the best answer based on scores.

[gen_verify](https://github.com/TokisakiKurumi2001/gen_verify)

## Agent learning

- [HF Agent](https://github.com/TokisakiKurumi2001/AgentHF)
