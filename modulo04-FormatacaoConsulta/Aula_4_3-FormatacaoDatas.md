# 📘 Aula 4.3 — Formatação de Datas

## 📑 Resumo
Nesta aula trabalhamos com **colunas de datas** no Power Query, utilizando como base o arquivo **BasesFuncionarios**. O foco foi aprender a extrair informações úteis e formatar corretamente colunas de datas como **Nascimento**, **Data de Contratação** e **Data de Demissão**.

---

## 🔹 Transformar x Adicionar Coluna
- **Transformar** → altera diretamente a coluna existente.
- **Adicionar Coluna** → cria uma nova coluna derivada.  
  - **Recomendação:** preferir *Adicionar Coluna* para preservar os dados originais, especialmente em colunas sensíveis como **Data de Nascimento**.

---

## 🔹 Extrações possíveis em colunas de data
Na aba **Adicionar Coluna → Data**, podemos:
- Extrair apenas o **Dia**.
- Extrair o **Dia da semana** (valor numérico).
- Extrair o **Nome do dia** (texto).
- Extrair o **Mês** (número ou nome).
- Extrair o **Ano**.

> 💡 Diferença:  
> - **Dia da semana**: retorna valores numéricos → Domingo = 0, Segunda = 1, ..., Sexta = 5, Sábado = 6.  
> - **Nome do dia**: retorna o texto → "Domingo", "Segunda-feira", etc.

---

## 🔹 Exemplo prático
- Na coluna **Nascimento**:
  - Criar uma nova coluna para extrair apenas o **Ano**.
  - Outra nova coluna para o **Dia da semana** em que a pessoa nasceu.
- Na coluna **Data de Contratação**:
  - Extrair o **Mês** para análises sazonais.
- Na coluna **Data de Demissão**:
  - Verificar se está em branco ou preenchida.

---

## 🔹 Ajustando formatos de data
- Em alguns casos, o Power Query pode interpretar datas como **números inteiros** (dias desde uma referência) ou até em **horas**.
- Solução:
  - Clicar na coluna → alterar tipo de dado para **Data**, **Data/Hora** ou **Número de dias**, conforme o contexto.
- Exemplo: ao calcular **Idade**, garantir que o formato seja **anos** (e não dias ou horas).

---

## ✅ Conclusão
- Colunas de datas oferecem muitas possibilidades de análise quando bem formatadas.  
- Sempre prefira **Adicionar Coluna** em vez de sobrescrever dados originais.  
- Saber a diferença entre **dia da semana** (numérico) e **nome do dia** (texto) é fundamental para análises corretas.  
- Atenção ao tipo de dado (dias, horas ou anos) ao calcular métricas como idade.
