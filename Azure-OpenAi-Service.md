## 🤖 Microsoft Azure OpenAI – Exploração Prática com Copilot & IA Assistida

Este repositório foi criado como parte de um desafio prático com foco na **exploração das ferramentas de Inteligência Artificial da Microsoft Azure**, especialmente os recursos providos pelo **Azure OpenAI Service** e pelo **Copilot**.

O objetivo principal é compreender e aplicar funcionalidades de **criação assistida**, com atenção especial aos **filtros de conteúdo**, segurança e **responsabilidade no uso de IA**.

---

## 🧠 Objetivo do Desafio

Explorar e documentar:

- Como funcionam os recursos do **Azure OpenAI**
- Experimentos com **Copilot (Word, Excel, GitHub)**
- Aplicação de **prompts criativos e produtivos**
- Avaliação de **filtros de conteúdo**, segurança e governança
- Análise das melhores práticas no uso de IA Generativa com responsabilidade

📌 **Entregável**: Repositório contendo exemplos práticos, prompts utilizados e insights obtidos.

---

## ☁️ Tecnologias Utilizadas

| Tecnologia               | Finalidade                                      |
|--------------------------|-------------------------------------------------|
| **Azure OpenAI Service** | Acesso a modelos como GPT-4, GPT-3.5, DALL·E    |
| **Microsoft Copilot**    | Assistente inteligente no Word, Excel, etc.     |
| **Azure Content Filters**| Controle de uso responsável e moderação         |
| **GitHub Copilot**       | Geração assistida de código                     |
| **Python + REST API**    | Chamadas diretas ao endpoint da OpenAI na Azure |

---

---

## 🔍 Exemplos de Uso

### 🧾 Word & Excel Copilot
- Resumo automático de documentos
- Geração de e-mails formais e relatórios
- Análise de planilhas com explicação de tendências

### 💻 GitHub Copilot
- Completação automática de código
- Sugestões inteligentes para funções em Python e Java
- Testes automatizados gerados por IA

### 🌐 Azure OpenAI API
- Geração de texto com GPT-4 via REST ou SDK
- Geração de imagens com DALL·E
- Análise de sentimentos e extração de tópicos

---

## 🚨 Filtros de Conteúdo e IA Responsável

A Azure implementa **filtros automáticos** para moderação de conteúdo por padrão nas chamadas à API OpenAI.

🛡️ Funcionalidades importantes:
- **Detection categories**: hate, violence, self-harm, sexual
- **Logging e monitoramento**
- **Parâmetros de segurança configuráveis**
- **Compliance com princípios de IA responsável da Microsoft**

🔗 [Mais sobre filtros de conteúdo na Azure](https://learn.microsoft.com/pt-br/azure/ai-services/openai/concepts/safety)

---
## 📋 Exemplos de Prompts Usados

### 📄 Word
```text
Reescreva este parágrafo com um tom mais formal e acadêmico.
----

### 📈 Excel

Analise esta planilha e identifique tendências nas vendas por região.

---
### GPT via API

``{
  "prompt": "Resuma os principais pontos do Manifesto Ágil em 3 frases.",
  "temperature": 0.5,
  "max_tokens": 100
}``
