# 🎙️ Assistente de Voz Inteligente Multimodal (Gemini + Python)

Este projeto foi desenvolvido como parte do Bootcamp de IA Generativa da DIO, com o objetivo de criar uma interface de comunicação por voz completa. A solução utiliza tecnologias de ponta para realizar o ciclo completo: **Ouvir -> Entender -> Responder -> Falar**.

---

## 🚀 Diferencial Técnico: Arquitetura Híbrida
Diferente da proposta inicial, esta implementação utiliza uma arquitetura híbrida e otimizada:
- **Speech-to-Text (STT):** Google Speech Recognition para transcrição gratuita e eficiente.
- **LLM (Cérebro):** Google Gemini 1.5 Flash, garantindo respostas rápidas e contexto atualizado.
- **Text-to-Speech (TTS):** gTTS (Google Text-to-Speech) para síntese vocal natural.
- **Tratamento de Dados:** Conversão dinâmica de áudio via `Pydub` para garantir compatibilidade de formatos de navegadores (WebM para WAV).

---

## 🛠️ Fluxo de Funcionamento

O sistema opera em quatro camadas principais:

1.  **Captura de Áudio:** Interface via JavaScript integrada ao Google Colab para gravação direta pelo microfone.
2.  **Engenharia de Áudio:** Pré-processamento com `Pydub` para normalizar o formato do arquivo e garantir a integridade dos dados (correção de cabeçalhos RIFF).
3.  **Processamento de Linguagem Natural (NLP):** O áudio é convertido em texto e enviado para a API do Gemini, que gera uma resposta contextualizada.
4.  **Síntese de Voz:** A resposta textual é convertida em um arquivo `.mp3` e reproduzida automaticamente para o usuário.



---

## 💻 Tecnologias Utilizadas

* **Linguagem:** Python 3.12
* **IA Generativa:** Google Generative AI (Gemini API)
* **Bibliotecas de Áudio:** SpeechRecognition, Pydub, gTTS
* **Ambiente:** Google Colab

---

## ⚙️ Como Executar

1. Clone o repositório.
2. Obtenha uma API Key gratuita no [Google AI Studio](https://aistudio.google.com/).
3. No Google Colab, adicione sua chave aos **Secrets** com o nome `GOOGLE_API_KEY`.
4. Execute as células em ordem: Instalação -> Configuração -> Gravador -> Processamento.

---

## 👨‍💻 Sobre o Autor
**Walter Salles**
Profissional da área financeira em transição para Ciência de Dados e BI. Atualmente no último período da graduação, focado em aplicar IA para automação de processos e análise de dados complexos.

---
