<!--START_SECTION:header-->
<div align="center">
  <p align="center">
    <img 
      alt="DIO Education" 
      src="https://raw.githubusercontent.com/digitalinnovationone/template-github-trilha/main/.github/assets/logo.webp" 
      width="100px" 
    />
    <h1>
Assistente de Voz Multi-Idiomas Com Whisper e ChatGPT</h1>
  </p>
</div>
<!--END_SECTION:header-->

# 🌐 Assistente de IA por Voz — Pipeline Completo (Voz → Texto → IA → Voz)

### *Projeto desenvolvido no Google Colab — Documentação Premium para Portfólio*

---

## 📘 Visão Geral

Este projeto implementa um **assistente de Inteligência Artificial multimodal**, capaz de transformar voz em texto, processar a mensagem com IA e devolver a resposta também em áudio.

Fluxo completo:

🎤 **Voz do usuário** → 🧠 **Transcrição (Whisper)** → 🤖 **ChatGPT** → 🔊 **Resposta falada (gTTS)**

O objetivo é demonstrar um pipeline moderno de interação humano–máquina, semelhante ao funcionamento de assistentes como Siri, Alexa e Google Assistant.

---

## 🎯 Objetivos do Projeto

- Criar um fluxo completo de interação por voz usando IA  
- Demonstrar integração entre áudio, transcrição, modelos de linguagem e síntese de voz  
- Construir um protótipo funcional de assistente virtual  
- Servir como base para aplicações mais avançadas em automação, acessibilidade e interfaces conversacionais  

---

## 🧩 Arquitetura e Explicação das Etapas

A seguir, cada etapa do pipeline conforme implementado no notebook.

---

### 🎙️ 1. Gravação de Áudio com Python

O projeto utiliza bibliotecas como `sounddevice` e `scipy` para:

- Capturar áudio diretamente do microfone  
- Definir taxa de amostragem e duração  
- Salvar o áudio em formato `.wav`  

Essa etapa é a porta de entrada do sistema, permitindo interação por voz.

---

### 🧠 2. Reconhecimento de Fala com Whisper

O áudio gravado é enviado ao modelo **Whisper**, responsável por:

- Processar o arquivo `.wav`  
- Converter fala em texto com alta precisão  
- Retornar a transcrição limpa e estruturada  

Whisper é um dos modelos mais robustos para reconhecimento de fala, funcionando bem mesmo com ruído ou sotaques.

---

### 🤖 3. Integração com a API do ChatGPT

Com o texto transcrito, o sistema envia a mensagem para a API do ChatGPT, que:

- Interpreta a intenção do usuário  
- Gera uma resposta contextualizada  
- Retorna um texto claro e natural  

Essa etapa representa o “cérebro” do assistente.

---

### 🔊 4. Sintetizando a Resposta Como Voz (gTTS)

Por fim, o texto gerado pelo ChatGPT é convertido em áudio usando **Google Text-to-Speech (gTTS)**:

- O texto é transformado em fala natural  
- Um arquivo `.mp3` é gerado  
- O áudio é reproduzido diretamente no Colab  

Assim, o assistente fecha o ciclo completo de interação por voz.

---

## 🏗️ Arquitetura do Pipeline


---

## 🚀 Aplicações Possíveis

Este projeto pode ser expandido para diversos cenários reais:

### 🤖 Assistentes Virtuais
- Atendimento automatizado  
- Suporte técnico  
- Chatbots com entrada e saída por voz  

### 🎧 Acessibilidade
- Leitura automática para pessoas com deficiência visual  
- Interfaces sem teclado  
- Sistemas de apoio por voz  

### 📚 Educação
- Tutores inteligentes  
- Explicações faladas  
- Correção e feedback por voz  

### 🏢 Automação Empresarial
- Assistentes internos  
- Triagem de chamados  
- Integração com fluxos corporativos  

### 🎨 Projetos Criativos
- Narradores automáticos  
- Personagens falantes  
- Storytelling interativo  

---

## 🛠️ Tecnologias Utilizadas

- **Python**  
- **Google Colab**  
- **sounddevice / scipy** (captura de áudio)  
- **Whisper** (transcrição de fala)  
- **OpenAI API (ChatGPT)**  
- **gTTS** (síntese de voz)  

---

## 🏁 Conclusão

Este projeto demonstra um pipeline completo de interação por voz com IA, combinando gravação, transcrição, processamento inteligente e síntese de áudio.  
A arquitetura apresentada é sólida, escalável e serve como base para aplicações reais em assistentes virtuais, automação, acessibilidade e interfaces conversacionais.

---

