<p align="center">
  <img src="Conrad_Logo.jpg" alt="Conrad's Logo" width="700"/>
</p>

# Conrad - Your Personal AI Learning Assistant

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/) [![Google Gemini](https://img.shields.io/badge/Google-Gemini%20API-purple.svg)](https://ai.google.dev/) [![Google Colab](https://img.shields.io/badge/Google%20Colab-notebook-orange.svg)](https://colab.research.google.com/)

**Conrad is an intelligent chatbot designed to be a learning companion, leveraging the power of Google's Gemini API to provide clear, engaging, and personalized explanations on a wide range of topics.**

---

## 📋 Table of Contents

- [About the Project](#about-the-project)
- [Key Features](#key-features)
- [Getting Started with Conrad](#getting-started-with-conrad)
- [Technologies Used](#technologies-used)
- [Advanced Customization](#advanced-customization)
- [Version History](#version-history)
- [Contributing](#contributing)
- [Developed by](#developed-by)
- [License](#license)

---

## About the Project

Conrad was born from the idea of making learning more accessible, interactive, and tailored to individual needs. Its mission is not just to provide answers, but to guide users through a process of discovery, using a Socratic and constructivist approach to help build a deep understanding of any subject.

Whether you are a curious student, a professional seeking new knowledge, or someone who simply loves to learn, Conrad is here to help you explore everything from basic everyday concepts to complex theories like the Drake Equation.

---

## Key Features

- **Interactive Chat Interface in Colab:** A rich and friendly chat experience created with `ipywidgets`, styled with CSS, and enhanced with JavaScript, all within a notebook.
- **Socratic Pedagogy:** Conrad strives to ask questions and use analogies to guide reasoning, rather than just providing direct answers.
- **Dynamic Multilingual Support:** Detects the user's language and adapts its responses to maintain a fluid and natural conversation.
- **Advanced Code Generation:**
    - Code blocks with automatic **syntax highlighting** for hundreds of languages.
    - **Copy** and **Download** buttons for each code snippet.
    - A visual indicator of the detected programming language.
- **AI Model Customization:** Includes a utility cell to list available Gemini models and allows for easy replacement of the default model.
- **Visible Context Management:** A token counter informs the user about the conversation's context window usage, helping to manage longer learning sessions.
- **Empathetic and Patient Persona:** Designed to recognize user frustration, validate their feelings, and proactively suggest new learning strategies.

---

## Getting Started with Conrad

Follow these steps to get your own instance of Conrad running in minutes.

1.  **Get your Google Gemini API Key:**
    - Go to [Google AI Studio](https://aistudio.google.com/).
    - Click on "**Get API key**" and create a new key.
    - **Copy and save this key**, you will need it in step 3.

2.  **Open the Project in Google Colab:**
    - Click the button below to open the notebook directly in Google Colab.
      [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/EnricoSouzaAfonso/ImersaoGemini_Alura_Conrad/blob/main/Conrad.ipynb)

3.  **Configure the API Key:**
    - In the Google Colab notebook you opened, click on the **key icon (Secrets)** in the left sidebar.
    - Create a new secret named `GOOGLE_API_KEY`.
    - In the "Value" field, paste the API Key you obtained in step 1.
    - Make sure the "Notebook access" toggle is enabled for this secret.

4.  **Run the Cells:**
    - **Cell 1 (`!pip install`):** Run this first to install all the necessary dependencies.
    - **Cell 2 (Initial Setup):** Run this to import the libraries and configure the API Key.
    - **Cell 4 (Main Interface):** Run this cell to start Conrad's chat interface.
    - You can now start chatting with Conrad!

---

## Technologies Used

- **Backend:** [Python](https.python.org/)
- **Generative AI:** [Google Gemini API](https://ai.google.dev/) (current default: `gemini-2.5-flash`)
- **Execution Environment:** [Google Colab](https://colab.research.google.com/)
- **Interactive Interface:** [IPython Widgets (ipywidgets)](https://ipywidgets.readthedocs.io/en/stable/)
- **Text Processing:**
    - [Markdown2](https://github.com/trentm/python-markdown2): To convert Markdown responses into HTML.
    - [BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/): To manipulate the HTML and add features to the code blocks.
    - [Pygments](https://pygments.org/): For code syntax highlighting.

---

## Advanced Customization

Conrad is designed to be flexible.

### Altering the AI Model

If you want to try a different Gemini model (e.g., a Pro model or a newer version), you can use **Cell 3 (List Available Models)**.

1.  Run Cell 3.
2.  It will list all models available to your API Key, with their technical names and limits.
3.  Copy the `Technical Name` of the desired model (e.g., `models/gemini-2.5-pro`).
4.  In **Cell 2**, paste this name into the `model_name_conrad` variable.
5.  Rerun Cell 2 and Cell 4 to start the chat with the new model.

### Adjusting Conrad's Personality

Conrad's personality, rules, and all teaching strategies are defined in the `system_instruction_conrad` variable at the top of **Cell 4**. You can edit this long text to adjust its behavior, tone, or even add new rules and abilities.

---

## Version History

For a detailed breakdown of all changes, new features, and fixes in each version of Conrad, please see the [**CHANGELOG.md**](CHANGELOG.md) file.

---

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  **Fork** the Project.
2.  **Create your Feature Branch** (`git checkout -b feature/AmazingFeature`).
3.  **Commit your Changes** (`git commit -m 'Add some AmazingFeature'`).
4.  **Push to the Branch** (`git push origin feature/AmazingFeature`).
5.  **Open a Pull Request**.

---

## Developed by

By **Enrico Souza Afonso** on May 17, 2025, during the Alura Gemini Immersion.

---

## License
This project is licensed under the **Creative Commons CC-BY-NC 4.0**.

[![License: CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/88x31.png)](https://creativecommons.org/licenses/by-nc/4.0/)

You can learn more about this license [here](https://creativecommons.org/licenses/by-nc/4.0/).
