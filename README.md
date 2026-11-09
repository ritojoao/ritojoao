### Hi, I'm Rito 👋

Staff Database Reliability Engineer who builds platforms. I keep databases fast, boring and recoverable, and I turn the work around them into self-service.

- **Deep:** PostgreSQL and MySQL (RDS, Aurora), DynamoDB
- **Daily:** MongoDB and Amazon DocumentDB
- **Platform:** Apache Airflow as the engine, Backstage as the front door, Python in between
- **Also:** Prometheus monitoring, partitioning, migrations, AI agents for database maintenance
- **Certified:** AWS Solutions Architect Professional, AWS Database Specialty (2023-2026)

#### Things I've shipped

- Migrated 280+ production MySQL databases from RDS to Aurora: cutover under 5 minutes, rollback via reverse replication, about 40% lower cost ([AWS blog](https://aws.amazon.com/pt/blogs/aws-brasil/nuvemshop-com-amazon-aurora-migracao-com-rollback-e-menor-custo/)).
- Fixed DynamoDB throttling on a hot path by splitting reads and writes (CQRS) ([TDC talk](https://thedevconf.com/tdc/2024/sao-paulo/trilha-microservices)).
- Built a hot/warm/cold data lifecycle so large tables stay small and cheap.
- Led an internal developer portal with 40+ self-service capabilities used by 4 teams, cutting database provisioning from days to minutes.
- Run database maintenance as Airflow DAGs with AI agents in the loop ([TDC talk](https://thedevconf.com/tdc/2026/sao-paulo/trilha-ai-code-e-automacao)).

#### Writing and talks

- **AWS Blog:** [Nuvemshop com Amazon Aurora: migração com rollback e menor custo](https://aws.amazon.com/pt/blogs/aws-brasil/nuvemshop-com-amazon-aurora-migracao-com-rollback-e-menor-custo/) (Nov 2025, co-author)
- **TDC São Paulo 2026:** [AI-Driven DBRE Platform: Automação Inteligente com KIRO, CrewAI e Airflow](https://thedevconf.com/tdc/2026/sao-paulo/trilha-ai-code-e-automacao) · [video](https://apps.thedevconf.com/portal/videos/tdc-2026-saopaulo/trilha-ai-code-e-automacao/ai-driven-dbre-platform-automacao-inteligente-com-kiro-crewai-e-airflow) · [slides](https://cdn.thedevconf.com.br/presentations/TDC2026SP/aicodeautomacao/BEC-9155_2026-08-03T020800_dbre-nuvemshop-agentic-db-maintenance-final.pptx)
- **TDC São Paulo 2024:** [CQRS: Como reduzir custos e aumentar performance na cloud](https://thedevconf.com/tdc/2024/sao-paulo/trilha-microservices) · [slides](https://docs.google.com/presentation/d/1MUddJ2Zkv_d1oMYYrhSGPrCq2gbA401d/edit)
- [All my TDC talks](https://thedevconf.com/palestrante/joaorito)
- [Answers on AWS re:Post](https://repost.aws/community/users/USAU0lQ_HCTcWesyNlS-K8Ag)

#### Open source

Contributing upstream to the tools I run in production:
[Apache Airflow](https://github.com/apache/airflow) ·
[pg_partman](https://github.com/pgpartman/pg_partman) ·
[postgres_exporter](https://github.com/prometheus-community/postgres_exporter) ·
[mongodb_exporter](https://github.com/percona/mongodb_exporter) ·
[dynamodump](https://github.com/bchew/dynamodump)

<!-- merged PRs go here as they land -->

---

<details>
<summary>🇧🇷 Em português</summary>

### Oi, sou o Rito 👋

Staff Database Reliability Engineer que constrói plataforma. Mantenho bancos de dados rápidos, previsíveis e recuperáveis, e transformo o trabalho em volta deles em self-service.

- **Fundo:** PostgreSQL e MySQL (RDS, Aurora), DynamoDB
- **Dia a dia:** MongoDB e Amazon DocumentDB
- **Plataforma:** Apache Airflow como motor, Backstage como porta de entrada, Python no meio
- **Também:** monitoração com Prometheus, particionamento, migrações, agentes de IA para manutenção de banco
- **Certificações:** AWS Solutions Architect Professional, AWS Database Specialty (2023-2026)

#### O que já entreguei

- Migrei mais de 280 bancos MySQL de produção do RDS para o Aurora: cutover abaixo de 5 minutos, rollback por replicação reversa, custo cerca de 40% menor ([blog da AWS](https://aws.amazon.com/pt/blogs/aws-brasil/nuvemshop-com-amazon-aurora-migracao-com-rollback-e-menor-custo/)).
- Resolvi throttling do DynamoDB num caminho crítico separando leitura e escrita (CQRS) ([palestra no TDC](https://thedevconf.com/tdc/2024/sao-paulo/trilha-microservices)).
- Montei um ciclo de vida de dados quente/morno/frio para tabelas grandes ficarem pequenas e baratas.
- Liderei um portal interno com mais de 40 capacidades self-service usado por 4 times, levando o provisionamento de banco de dias para minutos.
- Rodo manutenção de banco como DAGs do Airflow, com agentes de IA no meio do fluxo ([palestra no TDC](https://thedevconf.com/tdc/2026/sao-paulo/trilha-ai-code-e-automacao)).

#### Textos e palestras

- **Blog da AWS:** [Nuvemshop com Amazon Aurora: migração com rollback e menor custo](https://aws.amazon.com/pt/blogs/aws-brasil/nuvemshop-com-amazon-aurora-migracao-com-rollback-e-menor-custo/) (nov/2025, coautor)
- **TDC São Paulo 2026:** [AI-Driven DBRE Platform: Automação Inteligente com KIRO, CrewAI e Airflow](https://thedevconf.com/tdc/2026/sao-paulo/trilha-ai-code-e-automacao) · [vídeo](https://apps.thedevconf.com/portal/videos/tdc-2026-saopaulo/trilha-ai-code-e-automacao/ai-driven-dbre-platform-automacao-inteligente-com-kiro-crewai-e-airflow) · [slides](https://cdn.thedevconf.com.br/presentations/TDC2026SP/aicodeautomacao/BEC-9155_2026-08-03T020800_dbre-nuvemshop-agentic-db-maintenance-final.pptx)
- **TDC São Paulo 2024:** [CQRS: Como reduzir custos e aumentar performance na cloud](https://thedevconf.com/tdc/2024/sao-paulo/trilha-microservices) · [slides](https://docs.google.com/presentation/d/1MUddJ2Zkv_d1oMYYrhSGPrCq2gbA401d/edit)
- [Todas as palestras no TDC](https://thedevconf.com/palestrante/joaorito)
- [Respostas no AWS re:Post](https://repost.aws/community/users/USAU0lQ_HCTcWesyNlS-K8Ag)

Sempre topo uma boa conversa sobre banco de dados em produção.

</details>
