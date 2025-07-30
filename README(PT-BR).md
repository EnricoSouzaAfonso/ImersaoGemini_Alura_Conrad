<p align="center">
  <img src="Conrad_Logo.jpg" alt="Logo do Conrad" width="700"/>
</p>

# Conrad - Seu Assistente Pessoal de Aprendizado com IA

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/) [![Google Gemini](https://img.shields.io/badge/Google-Gemini%20API-purple.svg)](https://ai.google.dev/) [![Google Colab](https://img.shields.io/badge/Google%20Colab-notebook-orange.svg)](https://colab.research.google.com/)

**Conrad é um chatbot inteligente projetado para ser um companheiro de aprendizado, utilizando o poder da API Gemini do Google para fornecer explicações claras, engajadoras e personalizadas sobre uma vasta gama de tópicos.**

---

## 📋 Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Funcionalidades Principais](#funcionalidades-principais)
- [Como Começar](#como-começar-a-usar-o-conrad)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Personalização Avançada](#personalização-avançada)
- [Histórico de Versões](#histórico-de-versões)
- [Contribuição](#contribuição)
- [Desenvolvido por](#desenvolvido-por)
- [Licença](#licença)

---

##  Sobre o Projeto

Conrad nasceu da ideia de tornar o aprendizado mais acessível, interativo e adaptado às necessidades individuais. Sua missão não é apenas fornecer respostas, mas guiar os usuários em um processo de descoberta, utilizando uma abordagem socrática e construtivista para ajudar a construir um entendimento profundo sobre qualquer assunto.

Seja você um estudante curioso, um profissional buscando novos conhecimentos ou alguém que simplesmente ama aprender, Conrad está aqui para ajudar a explorar desde conceitos básicos do dia a dia até teorias complexas como a Equação de Drake.

---

##  Funcionalidades Principais

- **Interface de Chat Interativa no Colab:** Uma experiência de chat rica e amigável criada com `ipywidgets`, estilizada com CSS e aprimorada com JavaScript, tudo dentro de um notebook.
- **Pedagogia Socrática:** O Conrad se esforça para fazer perguntas e usar analogias para guiar o raciocínio, em vez de apenas fornecer respostas diretas.
- **Suporte Multilíngue Dinâmico:** Detecta o idioma do usuário e adapta suas respostas para manter uma conversa fluida e natural.
- **Geração de Código Avançada:**
    - Blocos de código com **realce de sintaxe** automático para centenas de linguagens.
    - Botões para **Copiar** e **Baixar** cada trecho de código.
    - Indicador visual da linguagem de programação detectada.
- **Personalização do Modelo de IA:** Inclui uma célula utilitária para listar os modelos Gemini disponíveis e permite a fácil substituição do modelo padrão.
- **Gerenciamento de Contexto Visível:** Um contador de tokens informa o usuário sobre o uso da janela de contexto da conversa, ajudando a gerenciar sessões de aprendizado mais longas.
- **Persona Empática e Paciente:** Projetado para reconhecer a frustração do usuário, validar seus sentimentos e proativamente sugerir novas estratégias de aprendizado.

---

##  Como Começar a usar o Conrad

Siga estes passos para ter sua própria instância do Conrad rodando em minutos.

1.  **Obtenha sua API Key do Google Gemini:**
    - Acesse o [Google AI Studio](https://aistudio.google.com/).
    - Clique em "**Get API key**" e crie uma nova chave.
    - **Copie e guarde esta chave**, você precisará dela no passo 3.

2.  **Abra o Projeto no Google Colab:**
    - Clique no botão abaixo para abrir o notebook diretamente no Google Colab.
      [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/EnricoSouzaAfonso/ImersaoGemini_Alura_Conrad/blob/main/Conrad.ipynb)

3.  **Configure a API Key:**
    - No Google Colab que você abriu, clique no ícone de **chave (Secrets)** na barra lateral esquerda.
    - Crie um novo "secret" com o nome `GOOGLE_API_KEY`.
    - No campo "Value", cole a sua API Key que você obteve no passo 1.
    - Certifique-se de que a opção "Acesso do notebook" está ativada.

4.  **Execute as Células:**
    - **Célula 1 (`!pip install`):** Execute-a primeiro para instalar todas as dependências necessárias.
    - **Célula 2 (Configuração Inicial):** Execute-a para importar as bibliotecas e configurar a API Key.
    - **Célula 4 (Interface Principal):** Execute esta célula para iniciar a interface do chat do Conrad.
    - Agora você pode começar a conversar com o Conrad!

---

##  Tecnologias Utilizadas

- **Backend:** [Python](https://www.python.org/)
- **IA Generativa:** [API do Google Gemini](https://ai.google.dev/) (padrão atual: `gemini-2.5-flash`)
- **Ambiente de Execução:** [Google Colab](https://colab.research.google.com/)
- **Interface Interativa:** [IPython Widgets (ipywidgets)](https://ipywidgets.readthedocs.io/en/stable/)
- **Processamento de Texto:**
    - [Markdown2](https://github.com/trentm/python-markdown2): Para converter as respostas em Markdown para HTML.
    - [BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/): Para manipular o HTML e adicionar funcionalidades aos blocos de código.
    - [Pygments](https://pygments.org/): Para o realce de sintaxe do código.

---

##  Personalização Avançada

O Conrad foi projetado para ser flexível.

### Alterando o Modelo de IA

Se você quiser experimentar um modelo Gemini diferente (por exemplo, um modelo Pro ou uma versão mais recente), pode usar a **Célula 3 (Listar Modelos Disponíveis)**.

1.  Execute a Célula 3.
2.  Ela listará todos os modelos disponíveis para sua API Key, com seus nomes técnicos e limites.
3.  Copie o `Nome Técnico` do modelo desejado (ex: `models/gemini-2.5-pro`).
4.  Na **Célula 2**, cole este nome na variável `model_name_conrad`.
5.  Reexecute a Célula 2 e a Célula 4 para iniciar o chat com o novo modelo.

### Ajustando a Personalidade do Conrad

A personalidade, regras e todas as estratégias de ensino do Conrad estão definidas na variável `system_instruction_conrad` no topo da **Célula 4**. Você pode editar este longo texto para ajustar seu comportamento, tom ou até mesmo adicionar novas regras e habilidades.

---

##  Histórico de Versões

Para um detalhamento de todas as mudanças, novas funcionalidades e correções em cada versão do Conrad, por favor consulte o arquivo [**CHANGELOG.md**](CHANGELOG.md).

---

##  Contribuição

Contribuições são o que tornam a comunidade de código aberto um lugar incrível para aprender, inspirar e criar. Qualquer contribuição que você fizer será **muito apreciada**.

1.  **Faça um Fork** do Projeto.
2.  **Crie sua Branch de Funcionalidade** (`git checkout -b feature/FuncionalidadeIncrivel`).
3.  **Faça o Commit de suas mudanças** (`git commit -m 'Adiciona uma Funcionalidade Incrível'`).
4.  **Faça o Push para a Branch** (`git push origin feature/FuncionalidadeIncrivel`).
5.  **Abra um Pull Request**.

---

##  Desenvolvido por

**Enrico Souza Afonso** no dia 17/05/2025 durante a Imersão Gemini da Alura.

---

##  Licença
Este projeto está licenciado sob a **Creative Commons CC-BY-NC 4.0**.

[![Licença CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc/4.0/)

Você pode saber mais sobre esta licença [aqui](https://creativecommons.org/licenses/by-nc/4.0/).
