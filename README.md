<p align="center">
  <img src="Conrad_Logo.jpg" alt="Logo do Conrad" width="700"/>
</p>

# Conrad - Seu Assistente Pessoal de Aprendizado com IA 🧠✨

**Conrad é um chatbot inteligente projetado para ser um companheiro de aprendizado, utilizando o poder da API Gemini do Google para fornecer explicações claras, engajadoras e personalizadas sobre uma vasta gama de tópicos.**

## 🎯 Sobre o Projeto

Conrad nasceu da ideia de tornar o aprendizado mais acessível, interativo e adaptado às necessidades individuais. Seja você um estudante curioso, um profissional buscando novos conhecimentos ou alguém que simplesmente ama aprender, Conrad está aqui para ajudar a explorar desde conceitos básicos do dia a dia até teorias complexas como a Equação de Drake.

O foco principal é ensinar de forma simples e aprofundada, evitando jargões técnicos desnecessários, para que o máximo de pessoas consiga aprender e se sentir confiante com novos conhecimentos.

## ✨ Funcionalidades Principais

*   **Explicações Claras e Adaptáveis:** Conrad pode explicar tópicos de diversas formas (simples, elaborada, técnica, intuitiva) e em diferentes níveis de profundidade (iniciante, intermediário, avançado).
*   **Estratégias de Ensino Diversificadas:**
    *   **Perguntar de Volta:** Estimula o pensamento crítico e avalia o conhecimento prévio.
    *   **Resumos e Questionários:** Ajuda na consolidação e revisão do aprendizado.
    *   **Analogias e Exemplos Práticos:** Torna conceitos abstratos mais concretos e relevantes.
    *   **Ensino Gradual:** Divide tópicos complexos em partes menores e gerenciáveis.
    *   **Conexão com Interesses:** Personaliza o aprendizado, tornando-o mais engajador.
    *   **Feedback Encorajador:** Motiva e orienta o usuário durante o processo.
    *   **Trilhas de Conhecimento:** Sugere próximos passos lógicos em campos de estudo mais amplos.
    *   **Metacognição:** Incentiva a reflexão sobre o próprio processo de aprendizado.
*   **Recomendações Externas:** Pode sugerir vídeos, sites e outros recursos para complementar o aprendizado.
*   **Interface Interativa em Linha de Comando:** Atualmente implementado para rodar em ambientes como Google Colab.

## 🛠️ Tecnologias Utilizadas

*   **Python:** Linguagem de programação principal.
*   **Google Gemini API:** O cérebro por trás da inteligência e capacidade de geração de texto do Conrad (especificamente o modelo `gemini-1.5-flash` ou similar).
*   **Google Colab:** Ambiente de desenvolvimento e execução principal para este protótipo.
*   **Bibliotecas Python:**
    *   `google-generativeai`: Para interagir com a API Gemini.
    *   `IPython`: Para funcionalidades de display no Colab (`Markdown`, `clear_output`).
    *   `textwrap`: Para formatação de texto.

## 🚀 Como Executar (Exemplo no Google Colab)

1.  **Clone o Repositório (ou crie um novo notebook e copie o código):**
    ```bash
    # Se você tiver os arquivos .py, pode clonar
    # git clone https://github.com/SEU_USUARIO/SEU_REPOSITORIO_CONRAD.git
    # cd SEU_REPOSITORIO_CONRAD
    ```
    Para o Google Colab, você provavelmente copiará e colará o conteúdo das células diretamente.

2.  **Configure sua Chave da API do Google:**
    *   No Google Colab, vá em "Segredos" (ícone de chave no painel esquerdo) e adicione um novo segredo chamado `GOOGLE_API_KEY` com o valor da sua chave.
    *   Certifique-se de que a permissão de acesso ao notebook está habilitada para este segredo.

3.  **Instale as Dependências (Célula 1):**
    ```python
    !pip -q install google-generativeai
    ```

4.  **Execute as Células de Configuração (Célula 2 e parte da Célula 4):**
    *   Célula 2: Contém os imports e a configuração inicial do cliente Gemini, modelo e chave API.
    *   Início da Célula 4: Contém a definição do `chat_config_conrad` (com o `system_instruction`) e do `text_wrapper`.

5.  **Inicie o Chat (Restante da Célula 4):**
    *   Execute a célula que contém o loop `while True:` para começar a interagir com o Conrad.
    *   Digite suas perguntas e explore os tópicos! Para sair, digite "fim".
  
## 📜 **Histórico de Versões (Changelog):**

Para um detalhamento de todas as mudanças, novas funcionalidades e correções em cada versão do Conrad, 
por favor consulte meu arquivo [**CHANGELOG.md**](CHANGELOG.md)

### Feito por Enrico Souza Afonso no dia 17/05/2025.
### Durante a Imersão Gemini da Alura.

### 📄 Licença
Este projeto está licenciado sob a Creative Commons CC-BY-NC 4.0. Saiba mais [aqui](https://creativecommons.org/licenses/by-nc/4.0/).

