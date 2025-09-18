# 📘 Aula 4.5 — Exercício de Revisão (Formatações)

## 📑 Resumo
Nesta aula utilizamos **arquivos externos** disponibilizados na pasta de exercícios do módulo 4 para praticar as ferramentas vistas até agora no Power Query.

---

## 🔹 Arquivos utilizados
- `gabarito - modulo 4.pbix`
- `modulo 4.pbix`
- `tabela clientes.xlsx`
- `tabela produtos.xlsx`
- `tabela vendas.xlsx`

> 💡 Para alterar o diretório de um arquivo:  
> clicar na engrenagem ao lado de **Fonte** → selecionar a nova pasta onde o arquivo se encontra.

---

## 🔹 Objetivos do exercício

### 1. Nome completo e separação do e-mail (Tabela Clientes)
- Criar nova coluna **Nome Completo**:
  - `Adicionar Coluna → Coluna Personalizada`
  - Fórmula: `[Nome] & " " & [Sobrenome]`
- Alternativa: usar **Transformar → Dividir Coluna** pelo delimitador `espaço`.
- Separar o **servidor do e-mail**:
  - `Transformar → Dividir Coluna → Por delimitador "@"`.

---

### 2. Criar coluna de desconto (Tabela Produtos)
- Objetivo: calcular desconto de **20% do valor total**.
- Selecionar a coluna de **Valor Total** →  
  `Adicionar Coluna → Número → Padrão → Multiplicar por 0,2`.
- Resultado: nova coluna **Desconto**.

---

### 3. Criar categoria de cliente por tamanho da família (Tabela Clientes)
- Base: coluna **Filhos**.
- `Adicionar Coluna → Coluna Condicional`.
- Regras:
  - Se **Filhos = 0** → saída **Pequena**.
  - Se **Filhos entre 1 e 2** → saída **Média**.
  - Se **Filhos > 2** → saída **Grande**.

---

## 🔹 Boas práticas aplicadas
- Sempre **renomear as colunas** após modificações para manter clareza.
- Preferir **Adicionar Coluna** em vez de sobrescrever, para não perder dados originais.
- Revisar o **Painel de Etapas Aplicadas** para garantir que as alterações estão corretas.

---

## ✅ Conclusão
Esse exercício consolidou os principais recursos de:
- Combinação de colunas (nome completo).
- Operações matemáticas simples (cálculo de desconto).
- Criação de colunas condicionais (categoria por número de filhos).
- Manipulação de texto (separação de servidor do e-mail).

Tudo isso reforça a importância de **organização e boas práticas** ao trabalhar no Power Query.

