# projeto-analisador-de-dados


## IA que cria insight
**Projeto: Analisador de dados** 
**Problema que resolve: Ajuda na tomada de decisão** 

## Como Funciona
O sistema recebe como entrada um arquivo CSV enviado pelo usuário, contendo dados que ele deseja analisar. A partir disso, no processamento, o backend utiliza IA (Google Gemini) para padronizar e organizar os dados, transformando-os em um formato estruturado. Em seguida, o sistema consulta uma API de CEPs (como a ViaCEP) para enriquecer os dados com informações adicionais. Com os dados já tratados e enriquecidos, a IA realiza uma análise completa e gera insights relevantes. Por fim, na saída, o usuário recebe os resultados dessa análise, que podem ser apresentados em forma de texto explicativo, tabelas ou gráficos, facilitando a interpretação dos dados.

## Integrantes
| Nome | GitHub |
|------|--------|
| [Vinicius Bueno] | [@vinnyBueno] |
| [Raquel Brito] | [@kel0508] |
| [Lucas Canto] | [@lucascantoo] |

## Arquitetura
```mermaid
flowchart LR

A[Usuario] -->|Upload CSV| B[Frontend]
B --> C[Backend API]

C --> D[Gemini - Padronizacao de Dados]
D --> E[DataFrame Padronizado]

E --> F[API de CEPs]
F --> G[Dados Enriquecidos]

G --> H[Gemini - Geracao de Insights]
H --> I[Resultados e Graficos]

I --> C
C --> B
B --> A
