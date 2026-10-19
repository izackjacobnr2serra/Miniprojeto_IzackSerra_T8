# Mini-Projeto Avaliativo - Módulo 1 - Semana 07 (Turma T8)
**Aluno:** Izack Jacob Nascimento Ribeiro Serra  
**Curso:** Análise de Dados com Python (SCTEC)  

---

## 1. Objetivo
Desenvolver uma Análise Exploratória de Dados (AED) aplicada ao setor de varejo, transformando dados brutos em informações compreensíveis para tomada de decisões gerenciais. O projeto abrange etapas de leitura, diagnóstico de qualidade, tratamento de valores nulos e duplicatas, padronização de textos, criação de funções reutilizáveis, estatísticas descritivas básicas, filtros, agrupamentos e exportação da base tratada.

## 2. Origem da Base de Dados
* **Fonte Original:** Base Varejo obtida do Kaggle ([Kaggle - Base Varejo](https://www.kaggle.com/datasets/namespaiva/base-varejo/data)).
* **Arquivo de Entrada:** `varejo.csv`
* **Arquivo Tratado de Saída:** `varejo_limpo.csv`

## 3. Significado das Colunas Utilizadas
* **id_cliente:** Código de identificação exclusivo de cada cliente.
* **nome:** Nome registrado do cliente no momento da compra.
* **idade:** Idade do cliente.
* **genero:** Gênero declarado pelo cliente.
* **categoria:** Categoria do produto comercializado.
* **valor_compra:** Valor financeiro total da transação em Reais (BRL).
* **quantidade:** Quantidade de itens adquiridos na operação.

## 4. Processo e Decisões de Limpeza
A leitura da base foi realizada utilizando a biblioteca `pandas`, seguida de um diagnóstico detalhado que identificou valores nulos, linhas duplicadas e inconsistências textuais:
* **Duplicatas:** Apenas linhas inteiramente duplicadas foram removidas (10 registros duplicados encontrados), preservando transações legítimas distintas realizadas pelo mesmo cliente.
* **Padronização Textual:** Espaços em branco excedentes foram removidos com `.str.strip()` e os nomes foram padronizados com iniciais maiúsculas (`.str.title()`). Valores nulos em texto foram tratados para `"Cliente Desconhecido"` ou `"Não Informado"` para evitar descarte desnecessário de dados.
* **Tratamento Numérico:** Valores de compra negativos (inconsistências de digitação) foram convertidos em valores absolutos, e valores nulos de faturamento foram preenchidos utilizando a mediana estatística da coluna para preservar o comportamento da distribuição.
* **Gravação:** A base tratada foi exportada com sucesso para o arquivo `varejo_limpo.csv` sem incluir o índice (`index=False`).

## 5. Conclusões e Resultados Numéricos
1. **Volume Consolidado:** O pipeline tratou e estruturou com segurança um total de 300 registros válidos para análise.
2. **Ticket Médio:** O cálculo estatístico indicou um ticket médio de R$ 230,37 na coluna de valor de compra, balizando o perfil financeiro das transações.
3. **Desempenho por Categoria:** O agrupamento evidenciou que a categoria *Eletrônicos* lidera o volume de compras (69 registros), seguida por *Alimentação* (61 registros).
4. **Distribuição de Faturamento:** A segmentação por gênero mostrou que o público *Feminino* gerou um faturamento total de R$ 25.663,30, enquanto o *Masculino* atingiu R$ 24.913,90.
5. **Recomendação de Negócio:** Recomenda-se direcionar campanhas promocionais de fidelização para as categorias de maior saída e faturamento expressivo.
6. **Limitação da Análise:** A base de dados não contempla uma linha temporal detalhada por horário ou dia da semana, o que limita a identificação de sazonalidades de curto prazo.

## 6. Instruções para Execução
1. Certifique-se de possuir o Python e a biblioteca `pandas` instalados em seu ambiente.
2. Posicione o arquivo `varejo.csv` no mesmo diretório do script ou notebook.
3. Execute as células do projeto sequencialmente.
4. O arquivo final tratado `varejo_limpo.csv` será gerado automaticamente.
