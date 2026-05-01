# projeto-analisador-de-dados


## IA que cria insight
**Projeto: Analisador de dados** 
**Problema que resolve: Ajuda na tomada de decisão** 

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
