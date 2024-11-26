# Parameter efficient fine-tuning (PEFT)

- Small number os trainable layers
- LLM with most layers frozen
- Sometimes LLMs dont touch in original parameters
  - Addition layers for PEFT
- Tradeoffs:
  - Memory efficiency
  - Parameter efficiency
  - Model performance
  - Traianing speed
  - Inference costs
- Methods
  - Selective
  - Reparametereization -> LOra
  - Additive

## LoRA

- Low Rank Adapation of Large Language Models
- Fine tunning re-parameterization
  - Freeze most of the original LLM weithgts
  - 2 rank decomposition matrices
  - Reduce the trainable parameters
- Compare between base odel ROUGE, Full fine-tune ROUGE and LORa fine tunning
- Choose the LoRA rank

  ## Prompt tunning with soft prompts

  - Prompt tuning =! prompt engineering
  - News treinable tokens
