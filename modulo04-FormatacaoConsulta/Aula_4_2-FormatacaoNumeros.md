# 📘 Aula 4.2 — Formatação de Números

## 📑 Resumo
Nesta aula aprendemos a trabalhar com **formatação de números** no Power Query, destacando diferenças em relação ao Excel e explorando recursos de arredondamento, atalhos e operações matemáticas.

---

## 🔹 Diferença Power BI x Excel
- No **Excel**, valores monetários aparecem com símbolos (R$, $, € etc.).
- No **Power BI**, os valores **não exibem símbolo de moeda** no Power Query.  
  - O símbolo só aparecerá no momento de visualização, no **Relatório**.
- Mesmo selecionando a opção de cifrão, ele **não mostra o símbolo no editor**.

---

## 🔹 Exemplo prático: coluna Salário Base
- Ícone `123` ao lado do nome → indica que a coluna é reconhecida como **Número Inteiro**.
- Correção:
  - Alterar o **tipo de dados** para **Número decimal fixo**.
  - Assim, o Power BI entende que a coluna deve ter **duas casas decimais**.
  - Caso haja mais decimais, o valor será **arredondado**.

---

## 🔹 Ajuste em outras colunas
- Colunas: **Salário Base, Benefício VT, Benefício VR**.  
- Todas foram ajustadas para **Número decimal fixo**.

---

## 🔹 Arredondamento
- Na aba **Número**, é possível:
  - Arredondar para **cima**.
  - Arredondar para **baixo**.
  - Escolher **quantas casas decimais** manter.
- Recurso útil e prático para projetos → normalmente a opção de **1 casa decimal** é a mais aplicada.

---

## 🔹 Atalhos úteis
- Selecionar várias colunas em sequência:
  - Clique na primeira → segure **Shift** → clique na última.
- Selecionar colunas não sequenciais:
  - Clique em cada coluna segurando **Ctrl + Shift**.

---

## 🔹 Estatística e Operações
- Na guia **Transformar**:
  - Exemplo: soma em uma coluna → substitui valores existentes (menos eficiente).
- Na guia **Adicionar Coluna**:
  - É possível criar uma **nova coluna** aplicando soma, multiplicação, média, etc.
  - Mais recomendado, pois mantém os dados originais.

---

## 🔹 Exemplo prático: aumento de 10% no VR
- Selecionar coluna **VR**.
- Ir em **Adicionar Coluna → Padrão → Multiplicar**.
- Multiplicar por **1,1**.
- Resultado: nova coluna criada com valor de VR acrescido em 10%.

---

## ✅ Conclusão
- O Power Query exige **definição correta do tipo de dado** (inteiro, decimal fixo etc.).
- Ferramentas de arredondamento e atalhos aceleram o processo.
- Melhor prática: usar **Adicionar Coluna** para operações, preservando os dados originais.
