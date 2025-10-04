# Introdução à Engenharia de Prompts

## 1. Conceito e Importância

**Prompt:** mensagem ou comando dado a um modelo de IA para gerar uma resposta.  
**Engenharia de Prompts:** habilidade de formular prompts de forma eficaz para obter respostas precisas e úteis.

### Importância
- Prompts claros e detalhados geram respostas mais precisas e relevantes.  
- Pode ser aplicada em contextos profissionais e pessoais, como escrever e-mails, resumir documentos e gerar ideias criativas.

### Exemplo
- **Prompt vago:**  
  "Escreva um e-mail para um cliente." → resultado genérico.  

- **Prompt detalhado:**  
  "Escreva um e-mail formal para um cliente interessado no notebook Oblivion Core, destacando processador Intel Core i9, RAM 32GB, SSD 512GB, display 16”, teclado RGB, refrigeração avançada e oferecendo 10% de desconto com código promocional. Tom profissional e amigável."  
  → resultado preciso e útil.

---

## 2. Pré-requisitos para o Curso

- Noções básicas de **Processamento de Linguagem Natural (PLN):** interação entre máquinas e linguagem humana.  
- Conhecimento de **Modelos de Linguagem de Grande Escala (LLMs):** modelos treinados com grandes volumes de dados para gerar e compreender textos.  
- **Ferramentas que serão utilizadas:** ChatGPT e Microsoft Co-Pilot.

---

## 3. Estrutura do Curso

### Parte 1: Visão Geral da Engenharia de Prompts
- Como os modelos de linguagem entendem prompts.  
- Conceito de tokens.  
- Janela de contexto: como o modelo lembra informações de prompts anteriores.  
- Elementos essenciais de um bom prompt, exemplificado com criação de histórias para RPG de mesa.

### Parte 2: Aplicações Práticas
- Uso de prompts no dia a dia: pessoal e profissional.  
- Exemplos de prompts aplicáveis em tarefas cotidianas.

### Parte 3: Avançando na Engenharia de Prompts
- Técnicas para aperfeiçoar e refinar prompts.  
- Cuidados na aplicação de prompts para evitar resultados indesejados ou incoerentes.

---

## Visão Geral da Engenharia de Prompts

### 1. Como os Modelos de Linguagem "Entendem" um Prompt
- **Modelos de Linguagem de Grande Escala (LLMs):** treinados com grandes volumes de dados textuais para gerar e compreender linguagem natural.  
- **Arquitetura Transformer:** base dos LLMs, utiliza mecanismos de atenção para processar palavras considerando o contexto de todas as outras no texto, não apenas de forma linear.  
- **Processo simplificado:** o modelo calcula probabilidades para prever o próximo token com base nos padrões aprendidos durante o treinamento, gerando respostas coerentes e contextualmente relevantes.

#### Analogia
**Editor experiente revisando um texto:**
- Lê o texto não apenas palavra por palavra, mas consulta outras partes para entender o contexto completo.  
- Semelhante ao mecanismo de atenção do Transformer, que destaca trechos relevantes para compreender o contexto.

---

### 2. Como os Modelos Processam os Prompts

1. **Tokenização:** o prompt é transformado em uma sequência de tokens (palavras, partes de palavras ou caracteres).  
   Exemplo:  
   "A DIO é a primeira plataforma Open Education brasileira dedicada a tornar o conhecimento em tecnologias exponenciais acessível a todos."  
   → Transformado em 24 tokens (exemplo com GPT-4 / GPT-4 Mini).

2. **Embeddings:** tokens são convertidos em representações vetoriais que capturam seu significado.

3. **Camadas do Transformer:**  
   - Aplicam atenção para compreender o contexto de cada token.  
   - Calculam distribuições de probabilidade para prever o próximo token.

4. **Geração de texto:** o modelo repete o processo até formar a sequência completa da resposta.

---

## Visão Geral da Engenharia de Prompts

### 1. Como os Modelos de Linguagem "Lembram" do que foi Dito

- **Memória entre interações:**  
  Modelos de linguagem não possuem memória persistente por padrão; não lembram de conversas passadas após o término da interação.

- **Janela de contexto:**  
  Dentro de uma interação, o modelo mantém o contexto do que foi dito através de um limite de tokens que pode processar simultaneamente.  
  Quando o limite é atingido, tokens mais antigos são descartados para dar espaço aos novos.

#### Analogia
**Professor escrevendo na lousa:**  
A lousa tem espaço limitado; à medida que mais informações são adicionadas, é necessário apagar o que foi escrito primeiro.  
O modelo funciona de forma semelhante, mantendo o contexto apenas dentro do limite da janela de contexto.

---

### 2. Exemplo de Contexto na Prática

**Interação:**
```
Usuário: Em poucas palavras, o que é Aliança?  
IA: Aliança é uma associação ou acordo entre partes para alcançar objetivos comuns.

Usuário: O que é Azeroth?  
IA: Azeroth é o mundo fictício do universo de World of Warcraft, com várias raças, facções e mitologia.

Usuário: O que é Aliança?  
IA: A Aliança é uma das duas principais facções em World of Warcraft, composta por humanos, elfos, anões, gnomos, draenei e worgen.
```

**Observação:**
- O modelo consegue usar o contexto do prompt anterior dentro da mesma interação.  
- Se a conversa ultrapassar o limite da janela de contexto, informações iniciais podem ser perdidas, exigindo reforço dos pontos importantes.

---

### 3. Personalização (ChatGPT)

É possível armazenar informações entre chats e usar instruções personalizadas para:
- Direcionar respostas conforme preferências do usuário.  
- Melhorar a consistência das respostas em múltiplas interações.

---

## Visão Geral da Engenharia de Prompts

### Elementos Essenciais de um Bom Prompt

#### 1. Instrução Clara
Define a tarefa específica que o modelo deve realizar.  
Deve ser direta, objetiva e sem ambiguidades.  

**Exemplo:**  
Crie uma história inicial para uma campanha de RPG de fantasia, envolvendo um grupo de aventureiros presos em uma cidade amaldiçoada.

---

#### 2. Contexto Adequado
Fornece informações adicionais que ajudam o modelo a gerar respostas mais precisas e relevantes.  

**Exemplo:**  
A cidade foi tomada por uma maldição que impede qualquer um de sair. Os moradores estão desaparecendo misteriosamente, e as sombras parecem ganhar vida.  
Os jogadores são aventureiros que chegaram à cidade pouco antes da maldição começar, em busca de tesouros escondidos.

---

#### 3. Exemplos
Orientam o modelo sobre o formato ou estilo da resposta.  
Mostram como a tarefa deve ser realizada.  

**Exemplo:**  
A história pode começar com os aventureiros sendo atacados por sombras vivas na entrada da cidade, forçando-os a buscar refúgio na taberna local.  
Lá, encontram um velho contador de histórias que fala sobre uma relíquia perdida que pode quebrar a maldição.

---

#### 4. Dados de Entrada
Informações ou elementos específicos que o modelo deve considerar.  
Podem incluir personagens, cenários ou problemas a serem resolvidos.  

**Exemplo:**  
Os aventureiros incluem: um ladino sarcástico, um clérigo com uma conexão misteriosa com as sombras, um bárbaro impulsivo e um mago que busca conhecimento proibido.  
O vilão principal é uma figura encapuzada que manipula a maldição das sombras.

---

#### 5. Formato da Saída
Define como a resposta deve ser estruturada, em termos de comprimento, detalhes ou estilo.  

**Exemplo:**  
A história deve ter de 2 a 3 parágrafos, começando com uma introdução impactante, seguida pelo primeiro desafio e um gancho final que motive os jogadores a explorar a cidade.

---

### Prompt Completo (Exemplo Integrado)

Crie uma história inicial para uma campanha de RPG de fantasia, envolvendo um grupo de aventureiros presos em uma cidade amaldiçoada.

A cidade foi tomada por uma maldição que impede qualquer um de sair. Os moradores estão desaparecendo misteriosamente, e as sombras parecem ganhar vida.  
Os jogadores são aventureiros que chegaram à cidade pouco antes da maldição começar, em busca de tesouros escondidos.

Por exemplo, a história pode começar com os aventureiros sendo atacados por sombras vivas na entrada da cidade, forçando-os a buscar refúgio na taberna local.  
Lá, encontram um velho contador de histórias que fala sobre uma relíquia perdida que pode quebrar a maldição.

Os aventureiros incluem: um ladino sarcástico, um clérigo com uma conexão misteriosa com as sombras, um bárbaro impulsivo e um mago que busca conhecimento proibido.  
O vilão principal é uma figura encapuzada que manipula a maldição das sombras.

A história deve ter de 2 a 3 parágrafos, começando com uma introdução impactante, seguida pelo primeiro desafio e um gancho final que motive os jogadores a explorar a cidade.

---

### Exemplo de Resposta Gerada pelo Modelo

História coesa e detalhada seguindo todas as instruções do prompt, incluindo:
- Introdução envolvente  
- Primeiros desafios e ação  
- Personagens e vilão específicos  
- Gancho narrativo final motivando a exploração
