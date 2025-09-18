# 📘 Aula 4.1 — Formatação de Texto

## 📑 Resumo
Nesta aula aprendemos a usar a aba **Transformar** e a aba **Adicionar Coluna** dentro do **Power Query**, explorando diferentes formas de manipular textos.

---

## 🔹 Transformar x Adicionar Coluna
- **Transformar**: altera a **coluna já existente**.
- **Adicionar Coluna**: cria uma **nova coluna** baseada na existente, aplicando a transformação escolhida.

Exemplo:
- Selecionar coluna **Nome Completo** → **Transformar → Formato → Maiúscula**  
  ➝ altera a própria coluna, deixando tudo em maiúsculo.
- Selecionar a mesma coluna → **Adicionar Coluna → Formato → Maiúscula**  
  ➝ cria uma **nova coluna** com os nomes em maiúsculo.

> 💡 Caso queira desfazer uma modificação, basta clicar no **X** em *Etapas Aplicadas*.

---

## 🔹 Extraindo dados de uma coluna
Exemplo prático com a coluna **Nome Completo** (arquivo `BasesFuncionarios.xlsx`):

1. Selecionar a coluna **Nome Completo**.
2. Ir em **Adicionar Coluna → Extrair → Texto antes do delimitador**.
   - Escolher o delimitador: `espaço`.
   - Resultado: cria uma nova coluna contendo apenas o **primeiro nome**.
3. Repetir o processo, mas escolher **Texto após o delimitador**:
   - Delimitador: `espaço`.
   - Resultado: nova coluna contendo apenas o **sobrenome**.

> 💡 Opções avançadas permitem escolher quantos delimitadores ignorar e se a contagem será feita do **início ou do fim** do texto.

---

## 🔹 Substituir valores
Exemplo prático com a coluna **Estado Civil**:
1. Selecionar coluna **Estado Civil**.
2. Ir em **Transformar → Substituir Valores**.
3. Configurar:
   - Localizar valor: `C` → Substituir por: `Casado`.
   - Localizar valor: `S` → Substituir por: `Solteiro`.

Resultado: todas as ocorrências de `C` e `S` foram substituídas por palavras completas.

---

## 🔹 Dividir coluna
Exemplo prático com a coluna **Login**:
1. Selecionar coluna **Login**.
2. Ir em **Transformar → Dividir Coluna → Por delimitador → Personalizado**.
3. Digitar o delimitador: `.`
   - Isso separa a coluna em duas partes, dividindo pelo ponto (`.`).

---

## ✅ Conclusão
- A aba **Transformar** modifica diretamente as colunas existentes.  
- A aba **Adicionar Coluna** gera novas colunas com as transformações aplicadas.  
- É possível **extrair nomes**, **separar sobrenomes**, **substituir valores** e **dividir colunas** com base em delimitadores, tudo dentro do **Power Query**.
