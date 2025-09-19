# 📘 Aula 5.3 — Importar Pasta com Vários Arquivos

## 📑 Resumo
Nesta aula aprendemos a importar todos os arquivos de uma pasta de forma automática, sem precisar abrir um por um.  
O Power Query identifica todos os arquivos da pasta e combina os dados em uma única tabela.

---

## 🔹 Como funciona
1. No Power BI → **Obter Dados → Pasta**.  
2. Selecionar a pasta desejada (ex.: `BasesDivididas/`).  
3. O Power Query lista todos os arquivos encontrados.  
4. Escolher entre:  
   - **Combinar e Transformar** → junta os arquivos em uma tabela única e abre o Power Query para edição.  
   - **Transformar Dados** → mostra a lista de arquivos e permite manipular manualmente.

---

## 🔹 O que o Power Query cria automaticamente
Quando usamos a opção **Combinar e Transformar**, o Power Query gera consultas auxiliares:
- **Consulta de Pasta** → lista todos os arquivos (nome, extensão, data, etc.).  
- **Sample File** → um arquivo de exemplo usado como modelo.  
- **Função `TransformarArquivo`** → armazena os passos de transformação aplicados ao Sample File.  
- **Consulta Combinada** → aplica a função a todos os arquivos da pasta e reúne os resultados.

👉 Em resumo: você define o tratamento em **um arquivo**, e o Power Query replica para todos os demais.

---

## 🔹 Exemplo prático
Na pasta `BasesDivididas/` existiam os arquivos:
- `FuncionariosAtuais.xlsx`  
- `FuncionariosAntigos.xlsx`

Após importar a pasta:
- O Power Query cria a consulta de pasta listando os dois arquivos.  
- Com a opção **Combinar**, ele junta os dados em uma nova tabela (ex.: `FuncionariosTotais`).  

---

## 🔹 Observações importantes
- Os arquivos precisam ter **estrutura semelhante** (mesmas colunas).  
- Caso existam diferenças, o Power Query mantém todas as colunas e preenche com **null** onde faltar informação.  
- Sempre valide os **tipos de dados** após combinar.  
- Se novos arquivos forem adicionados na pasta, basta atualizar o Power BI para que eles sejam incluídos automaticamente.

---

## ✅ Conclusão
O recurso de importar pastas é essencial para lidar com **grandes volumes de arquivos** (ex.: relatórios mensais).  
Ele cria um fluxo automatizado, aplicando a mesma transformação em todos os arquivos, e mantém os dados consolidados em uma única tabela.
