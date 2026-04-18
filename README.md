# 🤖 Agente Financeiro Inteligente com IA Generativa



---

# 🤖 Yas — Assistente Financeira com IA (Ollama + Streamlit)

Projeto desenvolvido como desafio final do curso **GenAI & Dados da DIO**.

A **Yas** é um chatbot inteligente inspirado em assistentes bancários, criado para ajudar usuários a entender, organizar e melhorar suas finanças pessoais de forma simples, rápida e acessível — rodando **100% local com IA usando Ollama**.

---

## 🚀 Demonstração

💬 Interface estilo chat
🧠 IA local (sem depender de API paga)
📊 Base de dados simulada para análise financeira

---

## 🎯 Objetivo do Projeto

Criar um agente conversacional que:

* Ajude no controle financeiro
* Responda dúvidas sobre finanças
* Analise gastos do usuário
* Evite alucinações com base em dados estruturados
* Utilize IA generativa de forma segura

---

## 🧠 Funcionalidades

* ✅ Chat interativo com memória de sessão
* ✅ Análise de gastos baseada em dados
* ✅ Respostas personalizadas com contexto do usuário
* ✅ Integração com LLM local (Ollama)
* ✅ Uso de base de conhecimento (JSON)
* ✅ Estratégias anti-alucinação

---

## 🏗️ Arquitetura

```mermaid id="f5y8tk"
flowchart TD
    A[Usuário] --> B[Streamlit]
    B --> C[Prompt + Contexto]
    C --> D[Ollama (LLM Local)]
    D --> E[Resposta]
    E --> B
```

---

## 📚 Base de Conhecimento

O sistema utiliza dados simulados para contextualizar respostas:

* `perfil_usuario.json` → Dados do usuário
* `transacoes.json` → Histórico financeiro
* `dicas_financeiras.json` → Sugestões
* `faq_financeiro.json` → Perguntas frequentes

---

## 🧠 Tecnologias Utilizadas

* Python
* Streamlit
* Ollama (LLM local)
* JSON (armazenamento de dados)
* Requests (integração com API local)

---

## ⚙️ Pré-requisitos

Antes de rodar o projeto, instale o **Ollama**:

👉 [https://ollama.com](https://ollama.com)

Depois, baixe um modelo:

```bash
ollama run llama3
```

---

## 🚀 Como Executar

```bash
# Clone o repositório
git clone https://github.com/FcoGuilhermeInfo/yas-financebot

# Acesse a pasta
cd yas-financebot

# Instale as dependências
pip install -r requirements.txt

# Execute o projeto
streamlit run app.py
```

---

## 💬 Exemplos de Uso

**Usuário:**

```
Gastei muito esse mês
```

**Yas:**

```
Entendi! Seus maiores gastos foram com alimentação e lazer.
Talvez valha revisar essas áreas. Quer dicas pra economizar?
```

---

## 🔒 Segurança e Confiabilidade

A Yas foi projetada para evitar erros comuns de IA:

* ❌ Não inventa informações
* ✅ Usa apenas dados fornecidos
* ⚠️ Informa quando não sabe algo
* 🔒 Não acessa dados reais

---

## 📊 Avaliação

O agente foi testado com:

* ✔️ Perguntas sobre gastos
* ✔️ Perguntas fora do escopo
* ✔️ Solicitações sem contexto
* ✔️ Tentativas de extrair dados sensíveis

Resultados:

* Alta assertividade
* Boa coerência
* Segurança mantida

---

## ⚠️ Limitações

* Não acessa contas bancárias reais
* Não realiza transações
* Não substitui um consultor financeiro
* Depende de dados simulados

---

## 🚀 Melhorias Futuras

* 📈 Dashboard com gráficos de gastos
* 🧠 Memória persistente de conversas
* 🔍 Classificação de intenções
* ☁️ Deploy online
* 🔗 Integração com banco de dados real

---

## 👨‍💻 Autor

Projeto desenvolvido por **Namorado da Yasmim** 💙
Curso: **GenAI & Dados - DIO**

---

## 📌 Status

🚧 Em desenvolvimento

---


