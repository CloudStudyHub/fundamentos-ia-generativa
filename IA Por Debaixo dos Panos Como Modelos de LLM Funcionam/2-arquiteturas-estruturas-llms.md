# Curso: Arquiteturas e Estruturas de LLMs

## 01. Introdução às Arquiteturas e Estruturas de LLMs

Neste módulo, somos apresentados ao universo das arquiteturas que dão forma aos Modelos de Linguagem de Grande Escala (LLMs). O instrutor **Matheus Galliani**, desenvolvedor Full Stack na GIO, conduz a jornada explicando de forma clara como funcionam os componentes internos que tornam esses modelos tão poderosos.

Os principais tópicos abordados incluem:  
* O que é um Transformer e por que ele revolucionou o campo da IA.  
* O papel das **camadas de atenção** na interpretação de contextos complexos.  
* Diferenças entre modelos tradicionais e arquiteturas modernas.  
* Importância de compreender o funcionamento interno dos modelos para otimização e desenvolvimento de aplicações.

Ao final, compreendemos por que entender as arquiteturas de LLMs é o primeiro passo para sair do papel de usuário e se tornar criador de soluções baseadas em IA.

## 02. Evolução das Arquiteturas de Modelos de Linguagem

Neste módulo, o foco é compreender a evolução das arquiteturas — desde os **modelos tradicionais** até a chegada dos **Transformers**, que marcaram uma revolução na Inteligência Artificial.

O conteúdo percorre:  
* **Modelos N-Gram**, que contam sequências de palavras e trabalham apenas com contextos curtos.  
* **Modelos Lineares** (Naive Bayes, Regressão, SVM), voltados para classificação, mas com limitações em compreensão de linguagem natural.  
* **Redes Neurais Recorrentes (RNNs)** e seus sucessores **LSTM** e **GRU**, que trouxeram a noção de memória e dependência sequencial.  
* A chegada dos **Transformers**, que substituíram o processamento sequencial por um mecanismo **paralelo e contextual**, através da operação de **self-attention**.

A explicação detalha como os Transformers resolvem limitações antigas, como o desvanecimento do gradiente, lentidão e falta de contexto global, e como essa arquitetura deu origem aos **LLMs modernos** como GPT, Claude, Llama, Gemini e PaLM.

O projeto prático ("Hands-On") explora esses conceitos em experimentos comparando N-Grams, RNNs e Transformers.

## 03. Funcionamento das Camadas de Atenção

Este módulo aprofunda o entendimento sobre o coração dos Transformers: as **camadas de atenção**.

A aula explica de forma intuitiva como o modelo decide **para onde olhar** em uma sequência de texto, priorizando as partes mais relevantes de acordo com o contexto.  
O exemplo clássico “A gata subiu na árvore porque ela estava com medo” mostra como o modelo atribui mais peso à palavra *gata* ao interpretar *ela*.

Principais conceitos apresentados:  
* **Query, Key e Value:** vetores que representam o que se busca, o que se oferece e o valor carregado de cada palavra.  
* **Cálculo de pesos de atenção**, que determina a relevância de cada token na sequência.  
* **Multi-Head Attention**, onde múltiplas cabeças processam relações diferentes simultaneamente.  
* **Vantagens das camadas de atenção:** processamento paralelo, contexto global, escalabilidade e desempenho superior em tarefas de NLP.

O projeto prático propõe visualizar pesos de atenção, testar ambiguidade e comparar modelos com e sem mecanismos de atenção.

## 04. Estrutura Interna dos LLMs

Neste módulo, o aluno abre a “caixa preta” dos modelos de linguagem para entender o que acontece **dentro de um LLM**.

A estrutura é explicada passo a passo:  
1. **Embeddings (ou Entities):** convertem palavras e tokens em vetores numéricos, representando significados e relações semânticas.  
2. **Camadas de Atenção:** identificam as partes mais relevantes do texto.  
3. **Feed Forward:** processa localmente cada token, refinando e organizando as informações.  
4. **Camadas de Normalização:** mantêm a estabilidade do treinamento.  
5. **Mecanismo de Saída (Softmax):** transforma os vetores finais em probabilidades de palavras, gerando o texto final.

O módulo reforça como o empilhamento dessas camadas, dezenas ou até centenas, gera respostas coerentes, contextuais e humanas.  
Compreender essa estrutura é essencial para ajustar modelos, reduzir erros e desenvolver novas aplicações em IA.

O Hands-On inclui testes práticos com embeddings, normalização, mecanismos de saída e análise de probabilidades de palavras.

## 05. Tendências e Inovações em Arquiteturas de LLMs

O módulo final aborda as **tendências atuais e futuras** que estão moldando o avanço das arquiteturas de LLMs.

Entre as principais inovações estão:  
* **Eficiência Computacional:** busca por modelos menores, rápidos e sustentáveis.  
* **Mixture of Experts (MoE):** modelos que ativam apenas os “neurônios especialistas” necessários, como o Mixtral e o Switch Transformer.  
* **Modelos Multimodais:** integração de texto, imagem, áudio e vídeo (ex: Gemini, GPT-4o, Claude 3).  
* **Modelos Especializados:** voltados para domínios específicos, como medicina e finanças.  
* **Modelos Locais:** execução offline em notebooks, celulares ou IoTs (ex: Llama 3).  
* **Embate Open Source vs Proprietários:** equilíbrio entre acessibilidade, inovação e segurança.

O módulo encerra destacando que acompanhar essas tendências é essencial para quem quer se manter relevante no mercado de IA, e que o futuro caminha para modelos **menores, mais autônomos, multimodais e sustentáveis**.

O Hands-On final propõe experimentos comparando arquiteturas, testando modelos locais, multimodais e o desempenho de sistemas open source versus proprietários.

## Conclusão

O curso **Arquiteturas e Estruturas de LLMs** oferece uma visão completa, teórica e prática, sobre como os grandes modelos de linguagem são construídos, evoluem e impactam o mundo real.  
Ao final, o aluno é capaz de:  
* Identificar as principais arquiteturas de LLMs.  
* Compreender o funcionamento das camadas internas.  
* Reconhecer o papel das inovações recentes e suas implicações.  
* Aplicar na prática conceitos de atenção, embeddings e arquitetura.
