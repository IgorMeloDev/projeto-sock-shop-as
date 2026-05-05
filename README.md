# Projeto Sock Shop - Observabilidade e Automação

Este repositório contém a evolução da aplicação de referência **Sock Shop**, desenvolvida como avaliação para a disciplina de Arquitetura de Software. O objetivo principal é incorporar um ecossistema completo de observabilidade e práticas de DevOps.

## 🛠️ Tecnologias Utilizadas até o momento
* **Docker e Docker Compose:** Orquestração e conteinerização dos microserviços.
* **Sock Shop:** Aplicação base de e-commerce baseada em microserviços.
* **Prometheus:** Coleta de métricas e monitoramento.
* **Grafana:** Visualização de dados e dashboards.

## 🚀 Como executar o projeto localmente

### 1. Pré-requisitos
Certifique-se de ter instalado em sua máquina:
* [Docker Desktop](https://www.docker.com/products/docker-desktop/)
* [Git](https://git-scm.com/)

### 2. Subindo a infraestrutura
Abra o terminal na raiz deste projeto e execute o comando abaixo para baixar as imagens e iniciar todos os containers em segundo plano:

```bash
docker-compose up -d
