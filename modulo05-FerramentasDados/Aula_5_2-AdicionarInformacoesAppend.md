# 📘 Aula 5.2 — Adicionar Informações na Base de Dados (Append)

## 📑 Resumo
Nesta aula aprendemos a usar o recurso **Append (Anexar/Adicionar consultas)** no Power Query, que serve para **empilhar linhas** de tabelas com a mesma estrutura (ou compatível).  
Diferente do **Merge (Mesclar)**, que adiciona colunas de outra tabela, o **Append** cria uma tabela com mais linhas.

---

## 🔹 Diferença: Merge x Append
- **Mesclar (Merge):** adiciona **novas colunas** relacionadas (join).  
- **Append (Anexar):** adiciona **novas linhas** embaixo, juntando registros de tabelas diferentes.  

👉 Ótima forma de lembrar:  
- **Merge** → colunas.  
- **Append** → linhas.  

---

## 🔹 Exemplo prático com funcionários
Arquivos utilizados:  
- `FuncionariosAtuais.xlsx`  
- `FuncionariosAntigos.xlsx`

### Passo a passo
1. No Power Query → **Página Inicial → Acrescentar Consultas como Nova**.  
2. Selecionar as tabelas:
   - Primeira tabela: **Funcionários Atuais**.  
   - Segunda tabela: **Funcionários Antigos**.  
3. Confirmar em **OK**.  
4. Será criada uma nova tabela → renomear para **FuncionariosTotais**.  

---

## 🔹 O que acontece se as colunas não forem iguais?
- O Power Query **mantém todas as colunas existentes**.  
- Se uma tabela não tiver determinada coluna, os valores dessa coluna aparecerão como **null**.  
- Exemplo:  
  - `FuncionariosAtuais` tem a coluna **Benefícios**.  
  - `FuncionariosAntigos` não tem.  
  - Após o Append, a coluna **Benefícios** é mantida, e as linhas de `FuncionariosAntigos` ficam com valor **null** nessa coluna.

---

## 🔹 Dicas importantes
- **Excluir bases de referência originais** se não forem mais usadas (acelera a atualização).  
- Sempre **renomear a tabela final** para algo intuitivo (ex.: `FuncionariosTotais`).  
- Antes do Append, confirme que as colunas estão com **tipos de dados corretos**.  

---

## ✅ Conclusão
- O **Append** é usado para **unir registros de várias tabelas em uma só**, empilhando as linhas.  
- Muito útil quando temos dados de períodos diferentes (ex.: funcionários antigos e atuais, vendas de diferentes anos, etc.).  
- As colunas não precisam ser exatamente iguais — o Power Query mantém todas, preenchendo com **null** onde não houver correspondência.
