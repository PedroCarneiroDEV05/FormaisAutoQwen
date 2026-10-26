# FormaisAutoQwen

**Um Small Language Model (SLM) especializado em Linguagens Formais e Autômatos.**

## Sobre o projeto

O FormaisAutoQwen é um projeto acadêmico que tem como objetivo desenvolver um modelo de linguagem pequeno (SLM), baseado na família Qwen, especializado no ensino de Linguagens Formais e Autômatos.

A proposta é adaptar um modelo pré-treinado por meio de fine-tuning supervisionado, utilizando um dataset próprio de perguntas, respostas e resoluções de exercícios da disciplina.

O projeto será desenvolvido de forma incremental, documentando as decisões técnicas, os experimentos realizados e os resultados obtidos.

## Objetivos

- Desenvolver um tutor de Linguagens Formais e Autômatos.
- Construir um dataset próprio, com exemplos revisados e organizados.
- Aplicar fine-tuning para especializar o modelo no domínio escolhido.
- Comparar o desempenho do modelo original com o modelo ajustado.
- Estudar técnicas de quantização para reduzir o consumo de memória.
- Executar e avaliar o modelo localmente.
- Relacionar os experimentos aos conceitos teóricos de redes neurais e aprendizado de máquina.

## Comportamento esperado

O FormaisAutoQwen deverá ser capaz de:

- Explicar conceitos de maneira clara e didática.
- Resolver exercícios passo a passo.
- Justificar as transformações e decisões realizadas durante as resoluções.
- Apresentar exemplos que facilitem a compreensão.
- Reconhecer quando não houver informações suficientes para produzir uma resposta confiável.

O modelo terá como foco o ensino e a resolução de problemas relacionados à disciplina, evitando inventar soluções quando não puder responder com segurança.

## Escopo inicial

Os conteúdos inicialmente previstos são:

- Linguagens formais e expressões regulares.
- Autômatos finitos determinísticos (AFD).
- Autômatos finitos não determinísticos (AFN).
- Gramáticas formais.
- Autômatos com pilha.
- Forma Normal de Chomsky.
- Forma Normal de Greibach.

O escopo poderá ser ampliado conforme o desenvolvimento do projeto.

## Tecnologias previstas

| Tecnologia | Finalidade |
|---|---|
| Python | Implementação dos experimentos |
| Qwen | Modelo de linguagem base |
| Hugging Face Transformers | Carregamento e utilização do modelo |
| Hugging Face TRL | Treinamento supervisionado |
| PEFT / LoRA ou QLoRA | Fine-tuning eficiente |
| Google Colab | Ambiente inicial de experimentação |
| Ollama ou llama.cpp | Execução local, conforme a compatibilidade do modelo |

As ferramentas e configurações definitivas serão escolhidas durante o desenvolvimento.

## Etapas do desenvolvimento

- [x] Definição inicial do projeto.
- [ ] Escolha e teste do modelo-base.
- [ ] Construção e revisão do dataset.
- [ ] Preparação do ambiente de treinamento.
- [ ] Implementação do fine-tuning.
- [ ] Avaliação do modelo original e do modelo ajustado.
- [ ] Estudo e aplicação da quantização.
- [ ] Execução e testes locais.
- [ ] Documentação dos resultados.
- [ ] Preparação da apresentação final.

## Estrutura planejada

```text
FormaisAutoQwen/
├── data/
│   ├── train.jsonl
│   ├── validation.jsonl
│   └── test.jsonl
├── notebooks/
│   ├── 01_baseline.ipynb
│   ├── 02_dataset_analysis.ipynb
│   └── 03_finetuning.ipynb
├── src/
│   ├── train.py
│   ├── evaluate.py
│   └── inference.py
├── results/
├── report/
├── README.md
└── requirements.txt
```

A estrutura é uma proposta inicial e será adaptada conforme as necessidades do projeto.

## Avaliação

A avaliação buscará verificar se o fine-tuning melhora o desempenho do modelo nas tarefas propostas.

Serão considerados critérios como:

- Correção das respostas.
- Clareza das explicações.
- Correção das resoluções de exercícios.
- Capacidade de resolver problemas não utilizados no treinamento.
- Consistência das respostas.
- Reconhecimento de limitações.

Os resultados serão documentados e comparados com os obtidos pelo modelo original.

## Relação com a teoria

Durante o desenvolvimento, serão investigados conceitos relacionados a:

- Pesos e parâmetros treináveis.
- Neurônios e camadas de redes neurais.
- Arquitetura Transformer.
- Funções de ativação.
- Função de perda (*loss*).
- Gradientes e otimização.
- Hiperparâmetros.
- Generalização.
- Quantização e eficiência computacional.

## Status do projeto

**Em desenvolvimento — fase inicial de planejamento.**

Este projeto faz parte de um desafio acadêmico voltado ao estudo prático de modelos de linguagem pequenos e de suas técnicas de adaptação.

Os resultados, experimentos e funcionalidades serão adicionados a este repositório à medida que forem implementados.
