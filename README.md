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

Contributing upstream to the tools I run in production:
[pg_partman](https://github.com/pgpartman/pg_partman) ·
[postgres_exporter](https://github.com/prometheus-community/postgres_exporter) ·
[mongodb_exporter](https://github.com/percona/mongodb_exporter) ·
[dynamodump](https://github.com/bchew/dynamodump)

**Merged upstream**

| Project | What it fixes for users | PR | Merged |
|---|---|---|---|
| [mydumper](https://github.com/mydumper/mydumper) | Restoring with `--skip-indexes` no longer fails or warns about index checksums for indexes myloader did not create. | [#2394](https://github.com/mydumper/mydumper/pull/2394) | 2026-11-11 |
| [Amazon DocumentDB tools](https://github.com/awslabs/amazon-documentdb-tools) | The metrics-collector sizing report now shows how many days of data it actually saw, and warns when that is shorter than the period you asked for. | [#232](https://github.com/awslabs/amazon-documentdb-tools/pull/232) | 2026-11-11 |
| [python-mysql-replication](https://github.com/julien-duponchelle/python-mysql-replication) | Reading MariaDB 11.7 binlogs no longer fails on query events such as `CREATE TABLE`. | [#650](https://github.com/julien-duponchelle/python-mysql-replication/pull/650) | 2026-11-11 |
| [mydumper](https://github.com/mydumper/mydumper) | A dump cut short by SIGTERM or Ctrl+C no longer looks complete or leaves the global read lock held. | [#2391](https://github.com/mydumper/mydumper/pull/2391) | 2026-11-11 |
| [mydumper](https://github.com/mydumper/mydumper) | `--ignore-set` is honored when loading with `--optimize-keys=SKIP`, so tables with an invalid `sql_mode` load again. | [#2392](https://github.com/mydumper/mydumper/pull/2392) | 2026-11-10 |
| [Patroni](https://github.com/patroni/patroni) | After a Kubernetes node reboot, Patroni no longer refuses to start because of a stale member record from the old Pod. | [#3770](https://github.com/patroni/patroni/pull/3770) | 2026-11-10 |
| [community.postgresql](https://github.com/ansible-collections/community.postgresql) | `postgresql_alter_system` stops reporting a change on every run for settings that need a restart, like `shared_preload_libraries`. | [#977](https://github.com/ansible-collections/community.postgresql/pull/977) | 2026-11-10 |
| [mydumper](https://github.com/mydumper/mydumper) | Checksums for table-level triggers (`-T`) are written and checked correctly, so restores can verify them. | [#2390](https://github.com/mydumper/mydumper/pull/2390) | 2026-11-10 |

<sub>In review: Patroni, mydumper, gh-ost, postgres_exporter, pg_repack, ProxySQL, WAL-G, pgroll, PyMySQL, PynamoDB, dynamodump, awslabs/mcp, aws-advanced-python-wrapper, pg_partman, pgBouncer, pgcli, CloudNativePG, Postgres Operator, Liquibase, go-sql-driver/mysql, go-mysql, pgstream, mariadb-operator, redis-operator, Apache AGE, ldap2pg, prometheus-rds-exporter. [All my PRs](https://github.com/search?q=author%3Aritojoao+is%3Apr+-user%3Aritojoao&type=pullrequests)</sub>

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

**Merged upstream**

| Projeto | O que resolve para quem usa | PR | Merged |
|---|---|---|---|
| [mydumper](https://github.com/mydumper/mydumper) | Restaurar com `--skip-indexes` não falha nem avisa mais sobre checksum de índices que o myloader não criou. | [#2394](https://github.com/mydumper/mydumper/pull/2394) | 2026-11-11 |
| [Amazon DocumentDB tools](https://github.com/awslabs/amazon-documentdb-tools) | O relatório de dimensionamento do metrics-collector agora mostra quantos dias de dados ele realmente viu, e avisa quando é menos que o período pedido. | [#232](https://github.com/awslabs/amazon-documentdb-tools/pull/232) | 2026-11-11 |
| [python-mysql-replication](https://github.com/julien-duponchelle/python-mysql-replication) | Ler binlogs do MariaDB 11.7 não falha mais em eventos de query como `CREATE TABLE`. | [#650](https://github.com/julien-duponchelle/python-mysql-replication/pull/650) | 2026-11-11 |
| [mydumper](https://github.com/mydumper/mydumper) | Um dump interrompido por SIGTERM ou Ctrl+C não parece mais completo nem deixa o read lock global preso. | [#2391](https://github.com/mydumper/mydumper/pull/2391) | 2026-11-11 |
| [mydumper](https://github.com/mydumper/mydumper) | `--ignore-set` é respeitado ao carregar com `--optimize-keys=SKIP`, então tabelas com `sql_mode` inválido voltam a carregar. | [#2392](https://github.com/mydumper/mydumper/pull/2392) | 2026-11-10 |
| [Patroni](https://github.com/patroni/patroni) | Depois de reiniciar um node do Kubernetes, o Patroni não se recusa mais a subir por causa do registro antigo do Pod. | [#3770](https://github.com/patroni/patroni/pull/3770) | 2026-11-10 |
| [community.postgresql](https://github.com/ansible-collections/community.postgresql) | `postgresql_alter_system` para de acusar mudança a cada execução em parâmetros que pedem restart, como `shared_preload_libraries`. | [#977](https://github.com/ansible-collections/community.postgresql/pull/977) | 2026-11-10 |
| [mydumper](https://github.com/mydumper/mydumper) | Checksum de triggers por tabela (`-T`) é gravado e conferido certo, então o restore consegue validar. | [#2390](https://github.com/mydumper/mydumper/pull/2390) | 2026-11-10 |

<sub>Em revisão: Patroni, mydumper, gh-ost, postgres_exporter, pg_repack, ProxySQL, WAL-G, pgroll, PyMySQL, PynamoDB, dynamodump, awslabs/mcp, aws-advanced-python-wrapper, pg_partman, pgBouncer, pgcli, CloudNativePG, Postgres Operator, Liquibase, go-sql-driver/mysql, go-mysql, pgstream, mariadb-operator, redis-operator, Apache AGE, ldap2pg, prometheus-rds-exporter. [Todos os meus PRs](https://github.com/search?q=author%3Aritojoao+is%3Apr+-user%3Aritojoao&type=pullrequests)</sub>

Sempre topo uma boa conversa sobre banco de dados em produção.

</details>
