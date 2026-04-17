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

A[Usuario] --> B[Frontend]
B --> C[Backend]

C --> D[Leitura de CSV]
D --> E[DataFrame]

C --> F[IA]
F --> G[Geração de Codigo]

E --> H[Executor de Codigo]
G --> H

H --> I[Resultado da Analise]

I --> C
C --> B
B --> A
