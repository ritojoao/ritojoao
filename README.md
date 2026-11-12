### Hi, I'm Rito 👋

Staff Database Reliability Engineer who builds platforms. I keep databases fast, boring and recoverable, and I turn the work around them into self-service.

- **Deep:** PostgreSQL and MySQL (RDS, Aurora), DynamoDB
- **Daily:** MongoDB and Amazon DocumentDB
- **Platform:** Apache Airflow as the engine, Backstage as the front door, Python in between
- **Also:** Prometheus monitoring, partitioning, migrations, AI agents for database maintenance
- **Certified:** AWS Solutions Architect Professional, Astronomer DAG Authoring for Apache Airflow 3, AWS Database Specialty (2023-2026), MongoDB skill badges in indexing design and CRUD ([Credly](https://www.credly.com/users/joao-victor-carvalho-rito/badges))

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

<img src="https://img.shields.io/badge/upstream%20PRs-84-1F6FEB?style=flat-square" alt="84 upstream PRs"> <img src="https://img.shields.io/badge/merged-12-2EA44F?style=flat-square" alt="12 merged"> <img src="https://img.shields.io/badge/projects-48-8250DF?style=flat-square" alt="48 projects"> <img src="https://img.shields.io/badge/thanked%20by%20maintainers-5-E5A00D?style=flat-square" alt="thanked by maintainers 5">

Contributing upstream to the tools I run in production:
[pg_partman](https://github.com/pgpartman/pg_partman) ·
[postgres_exporter](https://github.com/prometheus-community/postgres_exporter) ·
[dynamodump](https://github.com/bchew/dynamodump)

<details open>
<summary><b>Critical database infrastructure</b></summary>

| Project | Pull request | Merged by | Kind words |
|---|---|---|---|
| <img src="https://img.shields.io/badge/Patroni-database-1F6FEB?style=flat-square" alt="Patroni"><br>[patroni/patroni](https://github.com/patroni/patroni) | [Skip ensure_unique_name() with the Kubernetes DCS](https://github.com/patroni/patroni/pull/3770) | [@hughcapet](https://github.com/hughcapet) | |
| <img src="https://img.shields.io/badge/mydumper-database-1F6FEB?style=flat-square" alt="mydumper"><br>[mydumper/mydumper](https://github.com/mydumper/mydumper) | [Skip index checksum verification when --skip-indexes is used](https://github.com/mydumper/mydumper/pull/2394) | [@davidducos](https://github.com/davidducos) | |
| <img src="https://img.shields.io/badge/mydumper-database-1F6FEB?style=flat-square" alt="mydumper"><br>[mydumper/mydumper](https://github.com/mydumper/mydumper) | [Honor --ignore-set when --optimize-keys=SKIP is used](https://github.com/mydumper/mydumper/pull/2392) | [@davidducos](https://github.com/davidducos) | |
| <img src="https://img.shields.io/badge/mydumper-database-1F6FEB?style=flat-square" alt="mydumper"><br>[mydumper/mydumper](https://github.com/mydumper/mydumper) | [Handle SIGTERM and non-interactive SIGINT without holding locks or reporting success](https://github.com/mydumper/mydumper/pull/2391) | [@davidducos](https://github.com/davidducos) | 🙏 [@frankii91](https://github.com/mydumper/mydumper/pull/2391#issuecomment-6806876453) <i>"Thanks @ritojoao."</i> |
| <img src="https://img.shields.io/badge/mydumper-database-1F6FEB?style=flat-square" alt="mydumper"><br>[mydumper/mydumper](https://github.com/mydumper/mydumper) | [Fix table-level trigger checksum options](https://github.com/mydumper/mydumper/pull/2390) | [@davidducos](https://github.com/davidducos) | |
| <img src="https://img.shields.io/badge/python--mysql--replication-database-1F6FEB?style=flat-square" alt="python-mysql-replication"><br>[julien-duponchelle/python-mysql-replication](https://github.com/julien-duponchelle/python-mysql-replication) | [fix: parse MariaDB 11.7 Q_GTID_FLAGS3 and Q_CHARACTER_SET_COLLATIONS status variables](https://github.com/julien-duponchelle/python-mysql-replication/pull/650) | [@dongwook-chan](https://github.com/dongwook-chan) | 🙏 [@dongwook-chan](https://github.com/julien-duponchelle/python-mysql-replication/pull/650#issuecomment-6793818463) <i>"Thanks for the focused fix and regression test."</i> |
| <img src="https://img.shields.io/badge/MCP--PostgreSQL--Ops-database-1F6FEB?style=flat-square" alt="MCP-PostgreSQL-Ops"><br>[call518/MCP-PostgreSQL-Ops](https://github.com/call518/MCP-PostgreSQL-Ops) | [fix: scope pg_class joins by schema in get_table_schema_info](https://github.com/call518/MCP-PostgreSQL-Ops/pull/82) | [@call518](https://github.com/call518) | 🙏 [@call518](https://github.com/call518/MCP-PostgreSQL-Ops/pull/82#issuecomment-6831483641) <i>"Thanks @ritojoao for the fix and the clear reproduction!"</i> |
| <img src="https://img.shields.io/badge/MCP--PostgreSQL--Ops-database-1F6FEB?style=flat-square" alt="MCP-PostgreSQL-Ops"><br>[call518/MCP-PostgreSQL-Ops](https://github.com/call518/MCP-PostgreSQL-Ops) | [fix: scope constraint lookups in get_table_schema_info to the table](https://github.com/call518/MCP-PostgreSQL-Ops/pull/83) | [@call518](https://github.com/call518) | 🙏 [@call518](https://github.com/call518/MCP-PostgreSQL-Ops/pull/83#issuecomment-6831484378) <i>"Nice work tracking this one down."</i> |
| <img src="https://img.shields.io/badge/MCP--PostgreSQL--Ops-database-1F6FEB?style=flat-square" alt="MCP-PostgreSQL-Ops"><br>[call518/MCP-PostgreSQL-Ops](https://github.com/call518/MCP-PostgreSQL-Ops) | [Apply wait_event_type filter to get_wait_events session summary on PG 17+](https://github.com/call518/MCP-PostgreSQL-Ops/pull/84) | [@call518](https://github.com/call518) | 🙏 [@call518](https://github.com/call518/MCP-PostgreSQL-Ops/pull/84#issuecomment-6831485042) <i>"Good catch on the PG 17+ path drifting from the older one."</i> |
| <img src="https://img.shields.io/badge/pg__repack-database-1F6FEB?style=flat-square" alt="pg_repack"><br>[reorg/pg_repack](https://github.com/reorg/pg_repack) | [Cancel in-progress index builds on SIGINT with --jobs](https://github.com/reorg/pg_repack/pull/489) | [@za-arthur](https://github.com/za-arthur) | |
| <img src="https://img.shields.io/badge/community.postgresql-database-1F6FEB?style=flat-square" alt="community.postgresql"><br>[ansible-collections/community.postgresql](https://github.com/ansible-collections/community.postgresql) | [fix(postgresql_alter_system): compare with the pending value when a restart is required](https://github.com/ansible-collections/community.postgresql/pull/977) | [@hunleyd](https://github.com/hunleyd) | |
| <img src="https://img.shields.io/badge/Amazon%20DocumentDB%20tools-database-1F6FEB?style=flat-square" alt="Amazon DocumentDB tools"><br>[awslabs/amazon-documentdb-tools](https://github.com/awslabs/amazon-documentdb-tools) | [metrics-collector v2.5.2: report the observed data window, not only the requested period (#209)](https://github.com/awslabs/amazon-documentdb-tools/pull/232) | [@tmcallaghan](https://github.com/tmcallaghan) | |

</details>

**In review** · 69 open pull requests in 45 projects · [All my PRs](https://github.com/search?q=author%3Aritojoao+is%3Apr+-user%3Aritojoao&type=pullrequests)

Patroni, mydumper, gh-ost, postgres_exporter, pg_repack, ProxySQL, WAL-G, pgroll, pgstream, PyMySQL, PynamoDB, dynamodump, awslabs/mcp, Aurora DSQL tools, connectors and ORMs, aws-advanced-python-wrapper, pg_partman, pgBouncer, pgcli, psycopg, CloudNativePG, Postgres Operator, Liquibase, go-sql-driver/mysql, go-mysql, mariadb-operator, redis-operator, Apache AGE, ldap2pg, prometheus-rds-exporter, pev2, pgbadger, pgAdmin, powa-web, libpg_query, asyncpg, aiomysql, pg_auto_failover, pg_cron, pg_activity, pgcopydb, Percona XtraDB Cluster Operator, sqlc.

---

<details>
<summary>🇧🇷 Em português</summary>

### Oi, sou o Rito 👋

Staff Database Reliability Engineer que constrói plataforma. Mantenho bancos de dados rápidos, previsíveis e recuperáveis, e transformo o trabalho em volta deles em self-service.

- **Fundo:** PostgreSQL e MySQL (RDS, Aurora), DynamoDB
- **Dia a dia:** MongoDB e Amazon DocumentDB
- **Plataforma:** Apache Airflow como motor, Backstage como porta de entrada, Python no meio
- **Também:** monitoração com Prometheus, particionamento, migrações, agentes de IA para manutenção de banco
- **Certificações:** AWS Solutions Architect Professional, Astronomer DAG Authoring for Apache Airflow 3, AWS Database Specialty (2023-2026), badges de MongoDB em design de índices e CRUD ([Credly](https://www.credly.com/users/joao-victor-carvalho-rito/badges))

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

#### Open source

<img src="https://img.shields.io/badge/PRs%20upstream-84-1F6FEB?style=flat-square" alt="84 PRs upstream"> <img src="https://img.shields.io/badge/merged-12-2EA44F?style=flat-square" alt="12 merged"> <img src="https://img.shields.io/badge/projetos-48-8250DF?style=flat-square" alt="48 projetos"> <img src="https://img.shields.io/badge/agradecimentos%20de%20mantenedores-5-E5A00D?style=flat-square" alt="5 agradecimentos de mantenedores">

<details open>
<summary><b>Infraestrutura crítica de banco de dados</b></summary>

| Projeto | Pull request | Merged por | Palavras gentis |
|---|---|---|---|
| <img src="https://img.shields.io/badge/Patroni-database-1F6FEB?style=flat-square" alt="Patroni"><br>[patroni/patroni](https://github.com/patroni/patroni) | [Skip ensure_unique_name() with the Kubernetes DCS](https://github.com/patroni/patroni/pull/3770) | [@hughcapet](https://github.com/hughcapet) | |
| <img src="https://img.shields.io/badge/mydumper-database-1F6FEB?style=flat-square" alt="mydumper"><br>[mydumper/mydumper](https://github.com/mydumper/mydumper) | [Skip index checksum verification when --skip-indexes is used](https://github.com/mydumper/mydumper/pull/2394) | [@davidducos](https://github.com/davidducos) | |
| <img src="https://img.shields.io/badge/mydumper-database-1F6FEB?style=flat-square" alt="mydumper"><br>[mydumper/mydumper](https://github.com/mydumper/mydumper) | [Honor --ignore-set when --optimize-keys=SKIP is used](https://github.com/mydumper/mydumper/pull/2392) | [@davidducos](https://github.com/davidducos) | |
| <img src="https://img.shields.io/badge/mydumper-database-1F6FEB?style=flat-square" alt="mydumper"><br>[mydumper/mydumper](https://github.com/mydumper/mydumper) | [Handle SIGTERM and non-interactive SIGINT without holding locks or reporting success](https://github.com/mydumper/mydumper/pull/2391) | [@davidducos](https://github.com/davidducos) | 🙏 [@frankii91](https://github.com/mydumper/mydumper/pull/2391#issuecomment-6806876453) <i>"Thanks @ritojoao."</i> |
| <img src="https://img.shields.io/badge/mydumper-database-1F6FEB?style=flat-square" alt="mydumper"><br>[mydumper/mydumper](https://github.com/mydumper/mydumper) | [Fix table-level trigger checksum options](https://github.com/mydumper/mydumper/pull/2390) | [@davidducos](https://github.com/davidducos) | |
| <img src="https://img.shields.io/badge/python--mysql--replication-database-1F6FEB?style=flat-square" alt="python-mysql-replication"><br>[julien-duponchelle/python-mysql-replication](https://github.com/julien-duponchelle/python-mysql-replication) | [fix: parse MariaDB 11.7 Q_GTID_FLAGS3 and Q_CHARACTER_SET_COLLATIONS status variables](https://github.com/julien-duponchelle/python-mysql-replication/pull/650) | [@dongwook-chan](https://github.com/dongwook-chan) | 🙏 [@dongwook-chan](https://github.com/julien-duponchelle/python-mysql-replication/pull/650#issuecomment-6793818463) <i>"Thanks for the focused fix and regression test."</i> |
| <img src="https://img.shields.io/badge/MCP--PostgreSQL--Ops-database-1F6FEB?style=flat-square" alt="MCP-PostgreSQL-Ops"><br>[call518/MCP-PostgreSQL-Ops](https://github.com/call518/MCP-PostgreSQL-Ops) | [fix: scope pg_class joins by schema in get_table_schema_info](https://github.com/call518/MCP-PostgreSQL-Ops/pull/82) | [@call518](https://github.com/call518) | 🙏 [@call518](https://github.com/call518/MCP-PostgreSQL-Ops/pull/82#issuecomment-6831483641) <i>"Thanks @ritojoao for the fix and the clear reproduction!"</i> |
| <img src="https://img.shields.io/badge/MCP--PostgreSQL--Ops-database-1F6FEB?style=flat-square" alt="MCP-PostgreSQL-Ops"><br>[call518/MCP-PostgreSQL-Ops](https://github.com/call518/MCP-PostgreSQL-Ops) | [fix: scope constraint lookups in get_table_schema_info to the table](https://github.com/call518/MCP-PostgreSQL-Ops/pull/83) | [@call518](https://github.com/call518) | 🙏 [@call518](https://github.com/call518/MCP-PostgreSQL-Ops/pull/83#issuecomment-6831484378) <i>"Nice work tracking this one down."</i> |
| <img src="https://img.shields.io/badge/MCP--PostgreSQL--Ops-database-1F6FEB?style=flat-square" alt="MCP-PostgreSQL-Ops"><br>[call518/MCP-PostgreSQL-Ops](https://github.com/call518/MCP-PostgreSQL-Ops) | [Apply wait_event_type filter to get_wait_events session summary on PG 17+](https://github.com/call518/MCP-PostgreSQL-Ops/pull/84) | [@call518](https://github.com/call518) | 🙏 [@call518](https://github.com/call518/MCP-PostgreSQL-Ops/pull/84#issuecomment-6831485042) <i>"Good catch on the PG 17+ path drifting from the older one."</i> |
| <img src="https://img.shields.io/badge/pg__repack-database-1F6FEB?style=flat-square" alt="pg_repack"><br>[reorg/pg_repack](https://github.com/reorg/pg_repack) | [Cancel in-progress index builds on SIGINT with --jobs](https://github.com/reorg/pg_repack/pull/489) | [@za-arthur](https://github.com/za-arthur) | |
| <img src="https://img.shields.io/badge/community.postgresql-database-1F6FEB?style=flat-square" alt="community.postgresql"><br>[ansible-collections/community.postgresql](https://github.com/ansible-collections/community.postgresql) | [fix(postgresql_alter_system): compare with the pending value when a restart is required](https://github.com/ansible-collections/community.postgresql/pull/977) | [@hunleyd](https://github.com/hunleyd) | |
| <img src="https://img.shields.io/badge/Amazon%20DocumentDB%20tools-database-1F6FEB?style=flat-square" alt="Amazon DocumentDB tools"><br>[awslabs/amazon-documentdb-tools](https://github.com/awslabs/amazon-documentdb-tools) | [metrics-collector v2.5.2: report the observed data window, not only the requested period (#209)](https://github.com/awslabs/amazon-documentdb-tools/pull/232) | [@tmcallaghan](https://github.com/tmcallaghan) | |

</details>

**Em revisão** · 69 pull requests abertos em 45 projetos · [Todos os meus PRs](https://github.com/search?q=author%3Aritojoao+is%3Apr+-user%3Aritojoao&type=pullrequests)

Patroni, mydumper, gh-ost, postgres_exporter, pg_repack, ProxySQL, WAL-G, pgroll, pgstream, PyMySQL, PynamoDB, dynamodump, awslabs/mcp, Aurora DSQL tools, conectores e ORMs, aws-advanced-python-wrapper, pg_partman, pgBouncer, pgcli, psycopg, CloudNativePG, Postgres Operator, Liquibase, go-sql-driver/mysql, go-mysql, mariadb-operator, redis-operator, Apache AGE, ldap2pg, prometheus-rds-exporter, pev2, pgbadger, pgAdmin, powa-web, libpg_query, asyncpg, aiomysql, pg_auto_failover, pg_cron, pg_activity, pgcopydb, Percona XtraDB Cluster Operator, sqlc.

Sempre topo uma boa conversa sobre banco de dados em produção.

</details>
