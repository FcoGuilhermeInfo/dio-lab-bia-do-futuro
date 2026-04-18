

---

## 📊 Avaliação e Métricas

### 🧪 Como Avaliar o Agente

A avaliação da **Yas** foi feita de duas formas:

1. **Testes estruturados:** perguntas com respostas esperadas
2. **Feedback real:** testes com usuários simulados

---

## 📈 Métricas de Qualidade

| Métrica           | O que avalia                       | Exemplo de teste                            |
| ----------------- | ---------------------------------- | ------------------------------------------- |
| **Assertividade** | Se a Yas responde corretamente     | Perguntar gastos e receber valores corretos |
| **Segurança**     | Se evita inventar informações      | Pergunta fora do contexto                   |
| **Coerência**     | Se responde de acordo com o perfil | Sugestões compatíveis com o usuário         |

---

## 🧾 Exemplos de Cenários de Teste

### ✅ Teste 1: Consulta de gastos

* **Pergunta:** "Quanto gastei com alimentação?"
* **Resposta esperada:** Valor baseado nos dados
* **Resultado:** [x] Correto  [ ] Incorreto

---

### ✅ Teste 2: Recomendação de investimento

* **Pergunta:** "Qual investimento você recomenda?"
* **Resposta esperada:** Solicitar perfil antes de recomendar
* **Resultado:** [x] Correto  [ ] Incorreto

---

### ✅ Teste 3: Pergunta fora do escopo

* **Pergunta:** "Qual a previsão do tempo?"
* **Resposta esperada:** Informar limitação
* **Resultado:** [x] Correto  [ ] Incorreto

---

### ✅ Teste 4: Informação inexistente

* **Pergunta:** "Quanto rende o produto XYZ?"
* **Resposta esperada:** Admitir que não possui a informação
* **Resultado:** [x] Correto  [ ] Incorreto

---

## 📌 Resultados

### ✔️ O que funcionou bem:

* Respostas claras e objetivas
* Boa adaptação ao contexto do usuário
* Segurança ao evitar informações inexistentes
* Linguagem simples e natural

### ⚠️ O que pode melhorar:

* Tornar respostas ainda mais personalizadas
* Melhorar análise de gastos com mais dados
* Adicionar memória de conversas
* Expandir base de conhecimento

---

## 🚀 Métricas Avançadas (Opcional)

Para evolução do projeto, podem ser utilizadas métricas técnicas como:

* Tempo de resposta (latência)
* Consumo de tokens
* Taxa de erro
* Logs de interação

Ferramentas recomendadas:

* LangWatch
* LangFuse

---

