# Curso: Aplicações Práticas da Inteligência Artificial

## Parte 3: IA no Cotidiano e Aplicações Práticas

### 3.1 IA no dia a dia
**Chatbots e Assistentes Virtuais:**
- Modelos: ChatGPT (OpenAI), Bing Chat (Microsoft), Google Bard
- Assistentes populares: Siri (Apple), Alexa (Amazon), Google Assistant
- Funções: agendar compromissos, buscar informações, controlar dispositivos inteligentes

**Reconhecimento de fala:**
- Speech-to-Text: converte fala em texto (legendas, transcrição)
- Text-to-Speech: converte texto em fala (síntese de voz)
- Impacto na acessibilidade: pessoas com deficiência auditiva e avatares de línguas de sinais

**Criação de conteúdos educacionais:**
- IAs como suporte ao instrutor, potencializando revisão e elaboração de materiais
- Personalização da experiência de aprendizagem para diferentes perfis de alunos

---

### 3.2 Cases e exemplos reais
- **Curso atual:** uso de IAs para clonagem de voz, avatares virtuais e legendas multilíngues (português, inglês e espanhol)
- **Parceria DIO + iamtheCODE:** curso Green Software focado em formação de mulheres programadoras; conteúdos em múltiplos idiomas e reels multi-idioma
- **Parceria DIO + ICMC/USP:** player de vídeo acessível com legendas, transcrições e avatares de libras (VLibras, Hand Talk)

---

### 3.3 Ferramentas práticas de IA
**Chatbots:**
- ChatGPT, Bing Chat, Google Bard
- Uso de linguagem natural para interagir
- Necessidade de criar conta em alguns casos
- Diferentes respostas dependendo do modelo e contexto do prompt

**Geração de apresentações:**
- Gamma App: criação de slides com IA generativa
- Tradução automática, edição e refinamento humano

**Geração de imagens:**
- Bing Image Creator, Leonardo AI, MidJourney, DALL·E
- Baseadas em Stable Diffusion

**Síntese de voz e avatares virtuais:**
- Eleven Labs, D.I.D., HeyGen
- Clonagem de voz e humanização de avatares para conteúdos educativos

**Prática com chatbots:**
- Exemplos de prompts e refinamento de perguntas para otimizar respostas
- Criação de flashcards, vocabulário multilíngue e conteúdo educacional
- Feedback contínuo melhora a inteligência artificial

---

### 3.4 Bônus: Conhecendo a API da OpenAI (Transcrições)
- Exploração dos **endpoints da OpenAI**: text-to-speech, speech-to-text, geração de imagens, entre outros
- Uso do **Postman** para testes de endpoints
- Configuração de **API Key** para consumo das APIs
- Exemplos práticos:
  - Gerar áudio a partir de texto
  - Transcrever áudio em texto
  - Criar imagens com prompts personalizados (DALL·E)
- Observação: APIs possuem créditos gratuitos limitados e modelo de cobrança definido por serviço

**Mensagem principal:** Toda IA generativa funciona a partir de prompts; a OpenAI oferece documentação robusta e ferramentas que podem ser exploradas para criação de soluções práticas.

---
### 3.5 Geração de Imagens (Bing, Leonardo AI e MidJourney)

**Objetivo:** Explorar ferramentas de IA generativa para criação de imagens a partir de prompts.

**Ferramentas abordadas:**
- **Bing Image Creator**
- **Leonardo AI**
- **MidJourney**

**Como funcionam:**
- Todas trabalham em função de **prompts**, que fornecem as informações necessárias para gerar a imagem.
- A qualidade e o estilo das imagens dependem do prompt e das parametrizações específicas de cada ferramenta.

#### Bing Image Creator
- Interface simples, integrada ao Bing Chat.
- Criação de imagens através de prompts em linguagem natural.
- Limite de créditos mensais disponíveis.
- Exemplo de prompt: *"Liga de heróis programadores que usam a inteligência artificial para salvar o mundo"*
- Gera múltiplas imagens de forma rápida.

#### Leonardo AI
- Requer criação de conta para acesso.
- Interface mais técnica, permite:
  - Seleção de modelos (ex.: Leonardo Diffusion XL)
  - Ajuste do tamanho das imagens
  - Uso de versão beta do modelo
  - Geração de múltiplas imagens simultaneamente
- Possui ferramenta de **refinamento de prompts**, sugerindo versões otimizadas em inglês.
- Limite mensal de créditos, consumo por geração de imagens.
- Pontos fortes: controle detalhado sobre estilo, modelo e parametrizações.

#### MidJourney
- Utiliza **Discord como interface** para criação de imagens.
- Comandos via chat (ex.: `/imagine [prompt]`).
- Permite gerar variações de imagens e fazer **upscale**.
- Interface colaborativa: várias pessoas testam prompts simultaneamente.
- Limite de créditos no período beta; após isso, é necessário plano pago.
- Diferencial: imagens de alta qualidade e realismo.
- Não possui API oficial, diferente do Leonardo AI.

**Dicas gerais:**
- Prompts em português ou inglês funcionam na maioria dos modelos.
- Refinamento de prompts aumenta a assertividade das imagens.
- Controle de créditos e otimização do uso é importante, principalmente em plataformas pagas.
- Cada modelo gera resultados diferentes, então experimentar é essencial.

**Resumo:** A geração de imagens com IAs generativas funciona de maneira semelhante à criação de textos: o usuário define um prompt e o modelo realiza o trabalho pesado, enquanto o usuário atua como **engenheiro de prompts**, ajustando entradas para obter o melhor resultado visual.

### 3.6 Voz e Avatares Virtuais (ElevenLabs, D-ID e HeyGen)

**Objetivo:** Explorar ferramentas de IA generativa para criação de vozes sintéticas e avatares virtuais, incluindo clonagem de voz e produção de vídeos.

**Ferramentas abordadas:**
- **Eleven Labs** – Text-to-Speech (TTS), clonagem de voz.
- **D-ID** – Avatares virtuais, vídeos curtos.
- **HeyGen (Heijin)** – Avatares avançados, clonagem de voz, estúdio de edição e templates.

**Como funcionam:**
- Todas utilizam IA para sintetizar voz a partir de texto e gerar vídeos com avatares.
- Possuem **free tiers** limitadas e planos pagos para maior uso.

#### Eleven Labs
- Foco em **Text-to-Speech** e clonagem de voz.
- Free tier: até 10.000 caracteres por mês (~10 minutos de conteúdo).
- Funcionalidades:
  - Clonagem de voz a partir de pequenos trechos de áudio.
  - Ajustes de tom, cadência e sotaque.
  - Uso de vozes profissionais pré-gravadas.
  - Conversão de texto em fala para vídeos ou outros conteúdos.
- Ideal para gerar áudio de alta qualidade e realismo a partir de texto.

#### D-ID
- Criação de **avatares virtuais** a partir de imagens.
- Free tier: 5 minutos de vídeo por mês.
- Funcionalidades:
  - Seleção de avatares pré-definidos ou geração a partir de fotos.
  - Conversão de texto em fala usando vozes do sistema.
  - Movimentos básicos de boca, cabeça e gestos.
- Limitações: avatar gerado pode apresentar pequenas distorções em expressões ou mãos.

#### HeyGen (Heijin)
- Avatares avançados e estúdio de edição.
- Free tier: cerca de 1 minuto de vídeo gratuito (2 vídeos de 30 segundos cada).
- Funcionalidades:
  - Criação de avatares com maior realismo de movimentos.
  - Clonagem de voz e integração com vozes do Eleven Labs.
  - Templates de edição, branding kit e tradução/lip-sync de vídeos.
  - Necessita gravação de vídeo curto para treinar o avatar (2 minutos) para maior naturalidade.
- Diferenciais:
  - Movimentos mais naturais de boca, cabeça e mãos.
  - Pode traduzir vídeos e realizar lip-sync em diferentes idiomas.
  - Integra múltiplas funcionalidades (TTS, avatars, edição) em uma única plataforma.

**Dicas gerais:**
- Fotos para avatares devem ter boa iluminação, sem sombras e com expressão neutra.
- Refinar prompts e scripts melhora o realismo do avatar.
- Planejar créditos e duração de vídeos é importante nas versões gratuitas.
- Essas ferramentas podem ser integradas ao workflow de criação de conteúdo, educação e acessibilidade.

**Resumo:** O uso de IAs generativas de voz e avatares permite criar conteúdos multimídia com **alta personalização**, combinando Text-to-Speech e vídeos com avatares virtuais. As ferramentas analisadas oferecem diferentes níveis de complexidade, realismo e integração, sendo essenciais para explorar aplicações práticas em diversos contextos.