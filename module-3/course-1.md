# Fine-tuning LLMs with instruction

- At a high level:
  - Use the new examples to update the weights of LLM
- Steps:
  - Prepare the training data
  - Model
  - LLM completion -> Result
  - Validate: Comparate with a test label
  - Loss: Cross-entropy
- Sample prompt instruction templates
  - Classification
  - Text generation
  - Text summarization

## Fine tuning single task

- Like summarization or translate
- Catastrophic forgetting: The fine tunning was too spefically to a task, so he cannot performs too well in others tasks
  - Prompt have to made more generalistic
  - Fine tuning on multiple tasks
  - Consider Parameter Efficient Fine-tuning 

## Multi-task, instruction fine-tuning

- Avoiding the issue of forgetting others tasks
- Flan family models: Fine-tuned LAnguage Net
  - Specific set of instrutctions used to perform instruction fine-tuning
  - Flant-T5: Fine-tuned version of pre-trained T5 
  - SAMSum: Dialogue open dataset

## Model evaluation

- Metrics:
  - Accuracy
  - ROUGE: texto summarization. Compares a summary to one or more reference summaries
    - Recall, Precision, F1, clipping
  - BLEU: text translation. Compares to human-generated translations
 
## Benchmarks

- Datasets and metrics to benchmark LLM models
- GLUE
- SuperGLUE
- MMLU: Massive Multatask Language Understanding
- HELM: Holsit Evaluation of Language Models
- 
