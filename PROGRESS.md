# Progress

## Compromise NMT

![Architecture of Compromise_NMT](./image/compromise_NMT.png)

### With sinkhorn divergence loss

![Architecture of Compromise_NMT_OT](./image/compromise_NMT_with_ot.png)

| Model | BLEU En-De | BLEU En-En |
| -------- | -------- | -------- |
| Baseline     | 18.8     | -     |
| Compromise_NMT     | 18.7     | 57.1     |
| Compromise_NMT_OT | 23.7 | 77.5 |

**Lesson learned**: 
- Encoder does know how to translate back to it original language
- OT improves the scores significantly

*Potential*: Could use this for paraphrasing.

## BanaBERT

### Text classification

**Dataset**: Bana text classification

| Model | Train Accuracy | Test Accuracy | Validation Accuracy |
| ----- | -------------- | ------------- | ------------------- |
| [GRU](https://github.com/TokisakiKurumi2001/rnn_text_classification) | 91% | 68% | 78% |
| [BanaBERT](https://github.com/TokisakiKurumi2001/banabert_cls) | 85% | 85% | 85% |
| BanaBERT-pretrained + OT + CL | 85% | 85% | 85% |
| BanaBERT + OT + CL | 85% | 85% | 85% |
