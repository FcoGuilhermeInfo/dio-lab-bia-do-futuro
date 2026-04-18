# Base de Conhecimento


---

## 📚 Base de Conhecimento

### 📊 Dados Utilizados

| Arquivo                  | Formato | Utilização no Agente                    |
| ------------------------ | ------- | --------------------------------------- |
| `transacoes.json`        | JSON    | Analisar padrão de gastos do usuário    |
| `perfil_usuario.json`    | JSON    | Personalizar respostas e orientações    |
| `faq_financeiro.json`    | JSON    | Responder dúvidas comuns sobre finanças |
| `dicas_financeiras.json` | JSON    | Sugerir boas práticas financeiras       |

---

### 🔧 Adaptações nos Dados

Os dados foram simulados (mockados) para representar um cenário real de uso.
Foram feitas as seguintes adaptações:

* Criação de perfis de usuário (ex: iniciante, intermediário)
* Simulação de transações financeiras (gastos com alimentação, lazer, contas, etc.)
* Organização dos dados em JSON para facilitar a leitura pelo sistema
* Simplificação das informações para manter respostas rápidas e objetivas

---

## 🔗 Estratégia de Integração

### 📥 Como os dados são carregados?

Os arquivos JSON são carregados no início da execução do sistema.
Eles são lidos e armazenados em memória para acesso rápido durante a conversa.

Exemplo:

```python
import json

with open('data/transacoes.json') as f:
    transacoes = json.load(f)
```

---

### 🧠 Como os dados são usados no prompt?

Os dados são inseridos dinamicamente no contexto do prompt enviado ao modelo.

* Informações do usuário → incluídas no contexto
* Transações → resumidas antes de enviar
* Dicas e FAQs → usadas conforme a intenção da pergunta

A Yas utiliza esses dados para gerar respostas mais personalizadas e evitar respostas genéricas.

---

## 🧾 Exemplo de Contexto Montado

```
Dados do Cliente:
- Nome: João Silva
- Perfil: Iniciante
- Saldo disponível: R$ 1.200

Últimas transações:
- 10/04: Supermercado - R$ 320
- 12/04: Uber - R$ 45
- 15/04: Streaming - R$ 39,90

Comportamento identificado:
- Alto gasto com alimentação
- Frequência moderada de transporte
```

---



