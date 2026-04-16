# MovieFlix Data Platform

## Arquitetura

- Data Lake: CSVs gerados via API OMDb
- Data Warehouse: PostgreSQL
- Data Mart: Queries analíticas

## Pipeline

GitHub Actions:
- Build Docker
- Test container
- Push Docker Hub

## Como rodar

1. docker-compose up -d
2. python extract/extract_pipeline.py
3. python etl/load_to_postgres.py

## Queries

- Top 5 filmes
- Melhor gênero
- País mais ativo
- As consultas analíticas estão disponíveis em:

sql/analytics.sql
