# 📝 Changelog

Todas as mudanças notáveis neste projeto serão documentadas neste arquivo.

O formato é baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.0.0/),
e este projeto adere ao [Versionamento Semântico](https://semver.org/lang/pt-BR/).

## [1.4.0] - 30/05/2025

### Adicionado
- **Nova Interface de Usuário (Colab HTML):** Experiência de chat aprimorada com textarea, botão de envio e interatividade via callbacks, substituindo o input de console.
- **Gerenciamento Seguro de API Key:** Utilização de Colab Secrets para configuração da chave da API Gemini, com tratamento de erro robusto.
- **Utilitário de Seleção de Modelo:** Nova célula para listar e facilitar a escolha de diferentes modelos Gemini para o Conrad.
- **Avanços na IA (System Instruction):**
    - Melhoria na clareza das respostas (uso de Markdown).
    - Maior foco no usuário como condutor do aprendizado.
    - Instruções detalhadas para lidar com "code-switching" (múltiplos idiomas no prompt).
    - Capacidade de sugerir pausas e injetar curiosidades pertinentes.

### Alterado
- **Modernização da API e Lógica de Chat:**
    - Migração para a API `genai.GenerativeModel` (mais recente) para sessões de chat.
    - Lógica de interação e encerramento completamente refeita para suportar a nova interface HTML e a API atualizada.
- **Refinamentos no `System Instruction`:** Ajustes nas diretrizes multilíngues e de encerramento.

## [1.3.0] - 29/05/2025

### Adicionado
- **Suporte Multilíngue Dinâmico:** Conrad agora adapta saudações e respostas ao idioma do usuário, permitindo também a solicitação explícita de mudança de idioma.
- **Interface com Instruções Bilíngues:** Mensagens fixas do console (encerrar, resumo) exibidas em PT-BR e Inglês.

### Alterado
- **Lógica de Interação:** Saudação inicial, comando de encerramento e exibição de mensagens adaptadas para o novo suporte multilíngue.

## [1.2.0] - 24/05/2025

### Adicionado
- **Habilidades de Comunicação Avançadas:** Incluindo linguagem inclusiva, reconhecimento de frustração, melhor gestão de tópicos, tratamento de perguntas complexas e incentivo à autonomia do usuário.
- **Modo "Curiosidade Rápida":** Capacidade de compartilhar fatos interessantes.

### Alterado
- **Estrutura Interna e Feedback:** Melhor organização das instruções do `system_instruction` e refinamento no processo de lidar com feedback do usuário.

## [1.1.0] - 23/05/2025

### Adicionado
- **Interação e Pedagogia Aprimoradas:** Saudação padrão, sugestão de tópicos, novas estratégias de ensino (celebração de marcos, perguntas de sondagem), melhorias na gestão da conversa e maior clareza nas limitações do assistente.
- **Expansão de Tipos de Solicitação:** Suporte a brainstorming, comparações, explicações passo a passo, definições rápidas, role-playing e criação de estruturas.

### Alterado
- **Persona e Diretrizes:** Refinamento na expressão de empatia, adaptação de tom e política de uso de recursos externos.

## [1.0.0] - 18/05/2025

### Adicionado
- **Lançamento Inicial do Conrad:** Assistente educativo pessoal com personalidade base, 10 estratégias de ensino fundamentais e interface de chat interativa via console.
