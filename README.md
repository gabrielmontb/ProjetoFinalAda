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
* sql/analytics.sql

## Organização repositório:

```bash
ProjetoFinalAda/
│
├── extract/
│   ├── extract_pipeline.py
│   └── requirements.txt
│
├── etl/
│   └── load_to_postgres.py
│
├── sql/
│   ├── analytics.sql 
│   └── create_tables.sql
│
├── Dockerfile
├── docker-compose.yml
├── movies.csv
├── ratings.csv
├── users.csv
└── README.md
```

## Resultado execução queries:

### Consulta 1
  <img width="2093" height="426" alt="query_1" src="https://github.com/user-attachments/assets/dc641b6e-7c6d-47ad-86f3-b37d6834cf2c" />
  
### Consulta 2

<img width="523" height="598" alt="query_2" src="https://github.com/user-attachments/assets/b275c79a-b0a2-48de-9c0f-08a6e35d307b" />

### Consulta 3

<img width="452" height="291" alt="query_3" src="https://github.com/user-attachments/assets/eab1bb24-1c45-4f2d-9595-1d3e297df106" />


