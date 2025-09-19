# 📘 Aula 5.3 — Importar Pasta com Vários Arquivos

## 📑 Resumo
Nesta aula aprendemos a importar **todos os arquivos de uma pasta** de forma automática, sem precisar abrir cada arquivo individualmente.  
O Power Query consegue **combinar** os dados, facilitando o trabalho com bases divididas em múltiplos arquivos.

---

## 🔹 Passo a passo
1. **Obter Dados → Pasta**.  
2. Selecionar a **pasta desejada** (ex.: `BasesDivididas/`).  
3. O Power Query mostra uma **lista de arquivos encontrados**.  
4. Existem duas opções:  
   - **Combinar e Transformar**: junta os arquivos em uma tabela única e abre o editor para aplicar transformações.  
   - **Transformar Dados**: carrega a lista de arquivos e permite manipular manualmente.

---

## 🔹 O que acontece internamente?
- O Power BI cria duas consultas:
  1. **Consulta de pasta** → lista todos os arquivos (nome, extensão, data de modificação, etc.).  
  2. **Consulta combinada** → aplica automaticamente o mesmo processo de transformação em cada arquivo e junta os resultados.

- Isso é feito com a ajuda de uma **função gerada pelo Power Query**, chamada algo como:
