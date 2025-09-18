# 📘 Aula 3.2 — O que fazer após importar dados

## 📑 Resumo
Nesta aula aprendemos a trabalhar com o **Power Query**, aplicando transformações e melhorias nos dados importados a partir do arquivo `BasesFuncionarios.xlsx`.

---

## 🔹 Passos principais

### 1. Importação com Power Query
- Ir em **Importar dados → Transformar dados** (ao invés de apenas carregar).
- Isso abre a tela do **Power Query**, onde podemos editar a base antes de carregar.

### 2. Primeiras alterações
- **Renomear tabela**: alterar `Plan1` para `BaseFuncionarios`.
- **Excluir colunas desnecessárias**:
  - Exemplo: coluna **Bandeira** → verificar se contém apenas `null`, então clicar com o botão direito → *Remover coluna*.
  - Coluna **IdPessoal** também foi removida.
- **Ordenar tabelas**:
  - Exemplo: ordenar coluna **IdRH** → escolher crescente ou decrescente.

### 3. Limpeza de dados
- **Remover linhas em branco ou com erro**:  
  `Página Inicial → Remover Linhas → Remover Linhas em Branco`.
- **Remover duplicadas**:  
  - Garante que não haja registros clonados (ex.: dois funcionários iguais).
  - Mantém apenas uma ocorrência.

> 💡 Todas as modificações ficam registradas na aba **Etapas Aplicadas**, ajudando a acompanhar as transformações.

### 4. Formatação de colunas
- Exemplo: coluna **Data de Nascimento** estava como número inteiro.
- Ajuste: clicar no ícone da coluna ou botão direito → *Alterar tipo* → selecionar **Data**.

### 5. Aplicando alterações
- Após editar, vá em **Página Inicial → Fechar e Aplicar**.
- Os dados são carregados no Power BI já tratados.

### 6. Reabrindo Power Query
- Se precisar ajustar de novo:  
  `Página Inicial → Transformar Dados`.

---

## 🔹 Sobre salvamento
- Ao salvar, o Power BI cria um arquivo `.pbix`.
- Esse arquivo funciona como **manipulador dos dados**.
- Importante manter o **.pbix** e a **base de dados original** (`BasesFuncionarios.xlsx`) no **mesmo diretório**.
- Caso o arquivo de origem esteja em outra pasta, será necessário indicar o novo caminho.

---

## ✅ Conclusão
- Esta aula focou em **limpeza e preparação da base de dados**.
- Agora temos a tabela ajustada no Power BI, pronta para análises.
