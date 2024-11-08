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

# Fine tuning single task

- Like summarization or translate
- Catastrophic forgetting: The fine tunning was too spefically to a task, so he cannot performs too well in others tasks
  - Prompt have to made more generalistic
  - Fine tuning on multiple tasks
  - Consider Parameter Efficient Fine-tuning 
