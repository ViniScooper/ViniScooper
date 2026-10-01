  <div align="center">

    # Vinicius Lourenço
    ### Database Administrator & Cloud / DevOps Engineer

    <p>
      <i>Sustentação de bancos de dados de missão crítica, arquitetura multi-cloud e engenharia de software de alta
  performance.</i>
    </p>

    [![Website](https://img.shields.io/badge/Portfólio-viniscooper.com.br-0d9488?style=flat-square&logo=google-
  chrome&logoColor=white)](https://viniscooper.com.br)
    [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077b5?style=flat-
  square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/jose-vinicius-louren%C3%A7o-1a6b9014a/)
    [![Email](https://img.shields.io/badge/Email-vviniciuslourenco%40gmail.com-ea4335?style=flat-
  square&logo=gmail&logoColor=white)](mailto:vviniciuslourenco@gmail.com)
    [![GitHub](https://img.shields.io/badge/GitHub-ViniScooper-181717?style=flat-
  square&logo=github&logoColor=white)](https://github.com/ViniScooper)

    </div>

    ---

    ### ⚡ Resumo Profissional

    - 🗃️ **Administração de Bancos de Dados (DBA):** Experiência em sustentação, arquitetura e engenharia de bancos de
  dados corporativos OLTP em produção (**Oracle 19c/21c** e **PostgreSQL na AWS RDS**), mantendo SLA de **99.98% de
  disponibilidade**.
    - ⚙️ **Performance Tuning & Resiliência:** Análise profunda de planos de execução (`EXPLAIN ANALYZE`, relatórios
  **AWR**, **ADDM** e `pg_stat_statements`), ajuste fino de `autovacuum`, mitigação de locks concorrentes e rotinas de
  Disaster Recovery com **RMAN** e **Data Pump**.
    - 🔄 **Migrações Heterogêneas:** Planejamento e execução de migrações de dados (Oracle ➔ PostgreSQL na AWS) com
  mapeamento de tipos, conversão de schemas e replicação contínua via **CDC** (**AWS DMS**).
    - ☁️ **Multi-Cloud & Zero Trust:** Gestão e provisionamento de infraestrutura em nuvem (**Oracle Cloud Infrastructure -
  OCI**, **AWS**, **Vercel** e **Render**), redes seguras via **Cloudflare Zero Trust Tunnels**, containers **Docker** e
  automação com **Terraform (IaC)**.
    - 🚀 **Engenharia Full-Stack:** Desenvolvimento de soluções web corporativas orientadas a dados e escalabilidade com
  **Next.js**, **React (PWA)**, **Node.js** e **Fastify**.

    ---

    ### 🛠️ Stack Tecnológica & Especialidades

    | Área | Tecnologias & Ferramentas |
    | :--- | :--- |
    | **Bancos de Dados & DBA** | **Oracle Database (19c, 21c, ATP Exadata)**, **PostgreSQL (AWS RDS)**, MySQL 8.0,
  MongoDB, PL/SQL, Flyway |
    | **Cloud & DevOps** | **Oracle Cloud (OCI)**, **AWS (RDS, DMS, S3)**, **Docker**, **Cloudflare Zero Trust**,
  **Terraform**, Linux (Ubuntu/Oracle Linux), Nginx |
    | **Linguagens & Frameworks** | **Node.js**, **Next.js 16**, **React 19 (PWA)**, **TypeScript**, **Python**, Fastify,
  Express, Prisma ORM, Bash Script |
    | **Observabilidade & CI/CD** | GitHub Actions, Render PaaS, Vercel Edge, Telemetria via Webhooks e Crons |

    ---

    ### 🔥 Projetos de Destaque

    #### ☁️ [CloudOps Hub — Multi-Cloud Control Plane & DevOps Console](https://github.com/ViniScooper/CloudOps_Hub)
    > **Plataforma corporativa centralizada para gerenciamento de servidores em nuvem, orquestração de containers Docker,
  túneis Zero Trust e automação de deploys com IA nativa.**
    - **Arquitetura & Stack:** Next.js 16 (App Router), Node.js, Fastify, Docker, Cloudflare Zero Trust e Oracle Cloud
  (OCI sa-saopaulo-1).
    - **Funcionalidades Chave:**
      - 🖥️ **Telemetria ao Vivo:** Monitoramento em tempo real de instâncias em nuvem (consumo de CPU AMD EPYC, RAM,
  armazenamento NVMe e status dos nós).
      - 🛡️ **Guardião Anti-Sleep:** Agendador interno de micro-tarefas (Crons) para prevenir hibernação de serviços PaaS
  (zero cold-start).
      - 🌐 **Orquestração de Frontends & Backends:** Painéis dedicados para gerenciar deploys contínuos integrados às APIs
  da **Vercel** e do **Render**.
      - 🤖 **Odisseu AI Copilot:** Assistente autônomo com motor RAG integrado para análise de logs, status de containers
  e execução de scripts de infraestrutura.
    - 🔗 **Console em Produção:** [cloudops-hub-dun.vercel.app](https://cloudops-hub-dun.vercel.app/)

    ---

    #### 💼 [FinControl — Gestão Financeira Inteligente & Amortização](https://github.com/ViniScooper/controle-financeiro)
    > **PWA mobile-first focado em quitação acelerada de contratos, eliminação de juros compostos e automações proativas
  de orçamento.**
    - **Arquitetura & Stack:** React (Vite PWA), Node.js, Express, Oracle Cloud Autonomous Database (ATP Exadata) e JWT.
    - **Funcionalidades Chave:**
      - 🧮 **Simulador de Amortização:** Algoritmo matemático para simular aplicação de rendas extras (13º salário,
  bonificações), calculando economia real de juros e parcelas antecipadas.
      - 📱 **Progressive Web App (PWA):** Aplicativo 100% instalável em iOS e Android com Service Worker para resiliência
  e suporte a operações offline.
      - 🤖 **Bot de Notificações WhatsApp:** Rotina automatizada com CallMeBot para envio de lembretes de faturas a vencer
  e registro ágil de despesas por mensagem de texto.
    - 🔗 **Acesse o App:** [controle-financeiro-mauve-two.vercel.app](https://controle-financeiro-mauve-two.vercel.app/)

    ---

    ### 🛡️ Boas Práticas de Engenharia que Aplico

    > **Diagram exceeds terminal width (173 > 124 cols)**
    > Displayed as code block. Widen terminal to view inline.

    ```mermaid
    flowchart LR
        subgraph Edge["🛡️ Segurança & Acesso"]
            CF["Cloudflare Zero Trust"] -->|Túnel Privado sem IP exposto| NGINX["Nginx Reverse Proxy"]
        end

        subgraph Compute["🖥️ Camada de Aplicação"]
            NGINX --> DOCKER["Docker Containers (Node / Next / Python)"]
        end

        subgraph Data["🗃️ Persistência de Missão Crítica"]
            DOCKER --> ORA["Oracle 19c/21c (RMAN + Data Pump)"]
            DOCKER --> PG["PostgreSQL AWS RDS (CDC + Multi-AZ)"]
        end

  • Zero Exposure: Portas de banco e SSH nunca abertas para a internet pública; todo tráfego passa por túneis
  criptografados Zero Trust.
  • Database As Code: Versionamento estrito de schemas (DDL/DML) via migrations integradas às esteiras de CI/CD.
  • Resiliência e SLA: Políticas automatizadas de backup quente, exportação lógica e monitoramento proativo de métricas
  vitais.
  ──────
  ### 📊 Telemetria do GitHub
  ──────Vamos nos conectar? Fique à vontade para me chamar para conversar sobre bancos de dados, infraestrutura ou
  projetos desafiadores!

  💡 "O Oracle Database começou em 1977 rodando com apenas 128 KB de RAM. Performance e estabilidade importam desde o
  primeiro byte."
  ```
