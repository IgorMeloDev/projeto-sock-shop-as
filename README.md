# 🧦 Sock Shop - Observabilidade e Automação DevOps

Este repositório contém a evolução da aplicação de referência [Sock Shop](https://microservices-demo.github.io/), desenvolvida como projeto prático para a disciplina de Arquitetura de Software. 

O objetivo principal deste projeto é aplicar práticas reais de DevOps, implementando um ecossistema completo de observabilidade (métricas e logs) e integração contínua (CI/CD) em uma arquitetura baseada em microserviços.

## 🚀 Tecnologias Utilizadas

*   **Aplicação:** Docker, Docker Compose, Microserviços
*   **Monitoramento (Métricas):** Prometheus, cAdvisor, Grafana
*   **Logging Centralizado:** Elastic Stack (Elasticsearch, Kibana), Filebeat
*   **Integração Contínua (CI):** GitHub Actions

## 🎯 Funcionalidades Implementadas

1.  **Monitoramento de Infraestrutura e Microserviços:**
    *   Coleta de métricas de contêineres em tempo real utilizando o **cAdvisor**.
    *   Armazenamento de séries temporais via **Prometheus**.
    *   Dashboards interativos no **Grafana** para visualização de consumo de CPU, memória e tráfego de rede.
2.  **Logging Distribuído e Estruturado:**
    *   Captura de logs brutos de todos os microserviços (payment, orders, shipping, etc.) via **Filebeat**.
    *   Indexação de dados no **Elasticsearch**.
    *   Visualização centralizada e análise através de Data Views no **Kibana**.
3.  **Pipeline CI/CD (Atividade Extra):**
    *   Workflow automatizado no **GitHub Actions** (`docker-check.yml`).
    *   Validação automática de sintaxe e estrutura do arquivo `docker-compose.yml` a cada push ou pull request na branch `main`, garantindo a integridade da infraestrutura como código (IaC).

## 🛠️ Como Executar o Projeto

**Pré-requisitos:** Você precisará ter o [Docker](https://docs.docker.com/get-docker/) e o [Docker Compose](https://docs.docker.com/compose/install/) instalados na sua máquina.

1. Clone este repositório:
   ```bash
   git clone https://github.com/IgorMeloDev/projeto-sock-shop-as

2. Acesse a pasta do projeto:
 ```bash
cd projeto-sock-shop-as

3. Suba a infraestrutura completa em segundo plano:
 ```bash
docker compose up -d

🌐 Acessando os Serviços
Após iniciar os contêineres, aguarde alguns instantes para que todos os serviços fiquem disponíveis. Você pode acessá-los através dos links abaixo no seu navegador:

Serviço,URL,Descrição
Sock Shop,http://localhost,A loja virtual funcionando (Front-end).
Grafana,http://localhost:3000,Dashboard de métricas (cAdvisor + Prometheus).
Kibana,http://localhost:5601,Dashboard para visualização e busca de logs estruturados.
Prometheus,http://localhost:9090,Status dos targets e coleta de métricas brutas.

🎓 Contexto Acadêmico
Instituição: SECTRAS - Sistemas de Ensino em Ciências e Tecnologia

Curso: Análise e Desenvolvimento de Sistemas (ADS)

Componente Curricular: Arquitetura de Software

Semestre: 2026.1

Professor: Renato Leite

Desenvolvido por: Igor Melo


