# Pré-treinamento do LLM e leis de escalonamento

- Diferença entre foundation models e treinar seu próprio modelo
- Cada modelo pode ser melhor para cada situação
- Pré-treinamento
    - Dados não estruturados
    - Aprendizagem dos padrões dos textos
    - Loss function
    - Tokens
    - Data quality filter: exclusão de textos, artigos, etc
- Sequence to sequence models: encoder-decoder LLM
  - T5
  - Span corruption
  - Sentinel token
- COmputational challenges
    - CUDA out of memory
    - Quantization: reduce data types -> INT32 to INT16/8
        - Sign
        - Exponent
        - Fraction
        - Armazena com menor precisão
        - BFLOAT16 é uma boa ideia
