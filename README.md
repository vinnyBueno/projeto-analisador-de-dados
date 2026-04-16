# projeto-analisador-de-dados


## IA que cria insight
**Projeto: Analisador de dados** 
**Problema que resolve: Ajuda na tomada de decisão** 
## Integrantes
| Nome | GitHub |
|------|--------|
| [Vinicius Bueno] | [@vinnyBueno] |
| [Raquel Brito] | [@kel0508] |
## Arquitetura
flowchart TD

A[Usuário] --> B[Frontend]
B --> C[Backend]

C --> D[Leitura de CSV]
D --> E[DataFrame]

C --> F[IA]
F --> G[Geração de Código]

E --> H[Executor de Código]
G --> H

H --> I[Resultado da Análise]

I --> C
C --> B
B --> A
