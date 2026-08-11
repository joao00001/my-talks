# PostgreSQL como Motor de Inferência: Tokens, Embeddings e Gradients

**Event:** PgConf Brasil 2026  
**Date:** 2026-MM (a confirmar)  
**Location:** Brasil  
**Track:** PostgreSQL + IA aplicada  
**Duration:** 45 min (a confirmar)  
**Speaker:** João Detomini (EDB / Barman Team)

## Abstract

Esta talk mostra como usar PostgreSQL como núcleo de uma arquitetura de inferência local, cobrindo tokenização, embeddings, RAG completo com `pgvector`, estratégia de indexação (HNSW vs IVFFlat), benchmark real contra serviço externo e uso de ACID/WAL para preservar consistência semântica em fluxos de atualização e fine-tuning.

## Público-alvo

- Engenheiros de dados e backend que já usam PostgreSQL
- Times que estão avaliando RAG local ou híbrido
- Pessoas interessadas em IA aplicada com foco em arquitetura e consistência

## Principais aprendizados

- Como texto vira tokens e quais impactos isso causa no desenho da solução
- Como modelar embeddings no PostgreSQL sem sacrificar manutenção
- Quando escolher HNSW e como pensar no ponto de cruzamento com scan sequencial
- Onde está o gargalo real de latência em pipelines RAG
- Como evitar embedding drift com transações e rollback

## Resumo dos slides

1. Unidade fundamental: tokenização real e custo por idioma/operação.
2. Contexto e storage: TOAST, chunking semântico e organização de tabelas.
3. Similaridade vetorial: operadores `<=>`, `<#>` e `<->` em cenários reais.
4. Pipeline RAG local: embedding, busca vetorial, montagem de contexto e geração.
5. Índices vetoriais: trade-offs práticos entre HNSW e IVFFlat.
6. Benchmark: comparação de latência e arquitetura entre pgvector e Pinecone.
7. Consistência: embedding drift, gradientes simulados e rollback atômico.
8. Encerramento: PostgreSQL como epicentro de RAG + fine-tuning.

## Slides

- [slides.pdf](slides.pdf)

## Pré-requisitos

- Conhecimento básico de PostgreSQL
- Familiaridade com conceitos de embeddings e RAG
- Noções de SQL e planejamento de índices

## Referências

- pgvector: https://github.com/pgvector/pgvector
- MLX (Apple Silicon): https://github.com/ml-explore/mlx
- HNSW paper: https://arxiv.org/abs/1603.09320
- PostgreSQL TOAST docs: https://www.postgresql.org/docs/16/storage-toast.html
- Barman docs: https://pgbarman.org/documentation/

## Recursos

- Event page: https://2026.pgconf.com.br/
- Recording: to be added when available
