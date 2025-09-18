# 📘 Aula 4.4 — Colunas Condicionais

## 📑 Resumo
Nesta aula aprendemos a criar **colunas condicionais** no Power Query, que funcionam como um **IF/ELSE** em lógica de programação. Assim, podemos classificar valores e criar novas categorias com base em condições.

---

## 🔹 Criando uma coluna condicional
1. Ir em **Adicionar Coluna → Coluna Condicional**.
2. Definir o **nome da nova coluna**.
3. Adicionar as regras lógicas desejadas.

---

## 🔹 Exemplo 1: Categoria de Salários
Base: coluna **Salário Base**.  
Nova coluna: **Categoria Salários**.

Condições:
- Se **Salário Base ≥ 20000** → saída **A**.
- Senão, se **Salário Base ≥ 10000** → saída **B**.
- Senão → saída **C**.

> 🔎 Isso equivale a:
> ```pseudo
> if (SalarioBase >= 20000) { "A" }
> else if (SalarioBase >= 10000) { "B" }
> else { "C" }
> ```

---

## 🔹 Exemplo 2: Categoria de Idade
Base: coluna **Idade**.  
Nova coluna: **Categoria de Idade**.

Condições:
- Se **Idade ≥ 40** → saída **Faixa 1**.
- Senão, se **Idade ≥ 30** → saída **Faixa 2**.
- Senão → saída **Faixa 3**.

---

## 🔹 Dicas importantes
- **Comece pelas pontas** (maior valor ou menor valor) → facilita a lógica das condições.
- É possível adicionar várias **cláusulas adicionais**, mas só use o necessário para não complicar.
- Se os dados não tiverem uma chave ou identificador:
  - Criar uma **Coluna de Índice**:  
    `Adicionar Coluna → Coluna de Índice → escolher inicial (0 ou 1)`.
  - Pode mover a coluna de índice para o início da tabela (botão direito → *Mover → Início*).

---

## 🔹 Boas práticas
- Sempre que precisar **excluir uma coluna**, faça pelo **Painel de Etapas Aplicadas**, não apenas clicando com botão direito.  
  ➝ Isso evita acumular etapas desnecessárias e mantém o desempenho do Power BI.

---

## ✅ Conclusão
- Colunas condicionais são a forma de aplicar lógica **if/else** dentro do Power Query.  
- Muito úteis para **classificação de salários, idades e categorias personalizadas**.  
- Colunas de índice ajudam a organizar os dados quando não existe um identificador único.
