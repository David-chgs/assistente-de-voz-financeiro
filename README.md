# 🎙️ FinVoice AI — Assistente de Voz para Conceitos Financeiros
Este projeto foi desenvolvido a partir de um código do DIO (https://web.dio.me/articles/conversando-por-voz-com-o-chatgpt-utilizando-whisper-openai-e-python) com o objetivo de criar um auxiliar de voz em tempo real, para dúvidas sobre conceitos financeiros


## 🧠 Visão Geral

O **Finance Voice AI** é um assistente inteligente de voz projetado para responder dúvidas sobre conceitos financeiros de forma simples, rápida e acessível.

A aplicação combina tecnologias de **Speech-to-Text**, **Large Language Models (LLMs)** e **Text-to-Speech** para permitir uma experiência totalmente conversacional por voz.

> 🎯 Objetivo: transformar dúvidas financeiras em respostas claras, didáticas e em áudio — em poucos segundos.

---

## 🚀 Funcionalidades

* 🎤 Entrada por voz (captura de áudio em tempo real)
* 🧠 Transcrição automática de fala para texto
* 💬 Respostas inteligentes com foco em educação financeira
* 🔊 Conversão de texto para voz (resposta falada)
* 🔁 Estrutura preparada para conversas contínuas (context-aware)

---

## 🏗️ Arquitetura da Solução

```text
Usuário (voz)
   ↓
Speech-to-Text (Whisper)
   ↓
Processamento (LLM - ChatGPT)
   ↓
Resposta em texto
   ↓
Text-to-Speech (gTTS)
   ↓
Resposta em áudio
```

---

## 🧰 Tecnologias Utilizadas

* **Python 3.10+**
* **OpenAI Whisper** → Transcrição de áudio
* **ChatGPT (LLM)** → Geração de respostas
* **Google Text-to-Speech (gTTS)** → Síntese de voz
* **Pydub / SoundDevice** → Manipulação de áudio
* **AsyncIO** → Execução assíncrona (opcional)

---

## 🎯 Casos de Uso

* Educação financeira básica
* Explicação de termos como:

  * Inflação
  * Juros compostos
  * CDI / Selic
* Apoio a iniciantes em investimentos
* Interfaces conversacionais por voz

---

## 💡 Exemplos de Interação

**Usuário:**

> "O que é inflação?"

**Assistente:**

> "Inflação é o aumento geral dos preços ao longo do tempo..."

🔊 *(Resposta também reproduzida em áudio)*

---

## ⚙️ Como Executar o Projeto

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/finance-voice-ai.git
cd financevoice-ai
```

### 2. Crie o ambiente virtual

```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows
```

### 3. Instale as dependências

```bash
pip install -r requirements.txt
```

### 4. Configure as variáveis de ambiente

Crie um arquivo `.env`:

```env
OPENAI_API_KEY=your_api_key_here
```

### 5. Execute a aplicação

```bash
python app/main.py
```

---

## 🧠 Engenharia de Prompt

O sistema utiliza um prompt especializado para garantir respostas:

* Didáticas
* Objetivas
* Com exemplos práticos
* Sem jargões excessivos

**Exemplo de instrução base:**

```text
Você é um especialista em finanças pessoais.
Explique conceitos de forma simples, com exemplos e linguagem acessível.
```

---

## 📊 Possíveis Evoluções

* 📈 Integração com dados financeiros em tempo real
* 🧾 Simulações de investimento
* 🌐 Interface web com Streamlit
* 📱 Versão mobile
* 🧠 Memória de contexto entre interações
* 🔎 RAG com base de conhecimento financeira


> 💬 "Transformando dúvidas financeiras em conversas inteligentes."
