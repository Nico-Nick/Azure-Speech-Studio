# 🧪 Desafio: Ingestão, Indexação e Exploração de Documentos com IA na Azure

Este repositório contém anotações e registros do laboratório voltado para a organização e pesquisa de documentos utilizando ferramentas de **Inteligência Artificial da Microsoft Azure**.

O foco está na ingestão de dados, criação de índices semânticos com **Azure AI Search**, e exploração inteligente com **Azure OpenAI**, formando uma solução de **RAG (Retrieval-Augmented Generation)**.

---

## 🧠 Objetivo do Laboratório

Desenvolver uma solução prática que:

- Ingesta documentos em formatos variados (PDF, DOCX, etc.)
- Indexa esses documentos de forma **semântica** usando **Azure AI Search**
- Permite **consultas em linguagem natural** com base nos dados, utilizando **Azure OpenAI (ChatGPT/GPT-4)**

---

## 🚧 Etapas do Desafio
# 📥 Ingestão de Conteúdo

### O que é?
É o processo de **carregar e preparar documentos** para uso com ferramentas de IA.

Os documentos são enviados para um container no **Azure Blob Storage**.

- Tipos suportados: `.pdf`, `.docx`, `.txt`, `.html`
- Os arquivos passam por extração de texto e limpeza (pré-processamento)

📌 Ferramentas e serviços utilizados:
- `Azure Blob Storage`
- Funções de pré-processamento com `Python` ou `Azure Functions`

---

### 2. 🧾 Indexação Inteligente

### O que é?
Conversão dos documentos em **vetores semânticos** que podem ser buscados de forma eficiente.

Após o processamento, os textos são indexados com **Azure AI Search**, que cria um índice **semântico** e não apenas por palavras-chave.

🧠 Componentes envolvidos:
- **Azure AI Search**
- **Skillsets personalizados** (para OCR, extração de linguagem natural, etc.)
- **Indexers** para conexão com o Blob Storage
- **Cognitive Skills** (opcional)

✅ A indexação pode ser configurada para:
- Separar os documentos em chunks
- Criar campos personalizados
- Ativar busca semântica (Semantic Search)

---

### 3. 🔍 Consulta e Exploração

Com o índice criado, o sistema permite a recuperação dos documentos relevantes usando **busca semântica** e um modelo GPT para responder perguntas contextuais.

📌 Fluxo:
- A consulta em linguagem natural é usada para buscar os documentos mais relevantes no Azure AI Search
- Os resultados são enviados ao **Azure OpenAI (ChatGPT)**, que gera uma resposta contextualizada

✅ Essa arquitetura implementa o padrão **RAG (Retrieval-Augmented Generation)**

---
