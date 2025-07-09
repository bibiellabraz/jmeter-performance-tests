<p align="center">
  <img src="https://img.shields.io/badge/Java-23+-blue.svg" />
  <img src="https://img.shields.io/badge/JMeter-5.6.3-orange.svg" />
  <img src="https://img.shields.io/badge/License-MIT-green.svg" />
  <img src="https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow.svg" />
</p>


#  Testes de Performance com JMeter e BlazeMeter

Este repositório reúne testes de performance desenvolvidos com **Apache JMeter** e **BlazeMeter**, aplicados em diferentes contextos de aplicações web. O objetivo é demonstrar minhas habilidades práticas em testes de carga, análise de desempenho e automação de simulações com múltiplos usuários.

---

##  Objetivo

Avaliar a performance de aplicações através da simulação de acessos simultâneos, verificando tempo de resposta, status das requisições e estabilidade do sistema sob carga.

---

## Ferramentas Utilizadas

- [Apache JMeter](https://jmeter.apache.org/)
- [BlazeMeter](https://www.blazemeter.com/)
- CSV DataSet Config
- HTTP Request Sampler
- Assertions, Timers e Listeners (Dashboards)

---

## Requisitos / Versões
- Java 23+
- JMeter v5.6.3 (https://jmeter.apache.org/)
- BlazeMeter Plugin v6.6.7

## Como executar localmente
> Ler EXECUTE.txt

---

## Plataforma testada
> https://bugbank.netlify.app/

---

##  Tipos de Testes Realizados

- 🔹 Teste de Carga com 10 e 30 usuários simultâneos
> Verifica o desempenho da aplicação com um número fixo de usuários simultâneos (10, 30).

- 🔹 Teste de Estresse com aumento progressivo de 100 usuários simultâneos
> Avalia o comportamento da aplicação com aumento progressivo de usuários até o limite de quebra.

- 🔹 Validação de tempo de resposta e status HTTP
> Mede o tempo médio e máximo das requisições com base no status HTTP.

- 🔹 Execução com massa de dados via CSV
> Valida cenários dinâmicos usando múltiplas credenciais ou dados externos.

- 🔹 Análise de performance com gráficos e relatórios HTML
> Automatiza a criação de dashboards visuais com base nos testes executados.


---

## Estrutura do Repositório

```bash

├── load-tests/
│   ├── AggregateReport10users.csv
│   ├── AggregateReport30users.csv
│   └── Report/
│       └── index/
|       └── index/
│   ├── Plans/
|       └── TestPlan10.jmx/
|       └── TestPlan30.jmx/
├── stress-tests/
│   |── AggregateReport100.csv
│   ├── SummaryReport100.csv
│   ├── ViewResultsTree100.csv
|   └── Report 1/
|       └── index/
|   └── Report 2/
|       └── index/
|   └── Report 3/
|       └── index/
│   ├── Plans/
|       └── TestPlan100.jmx/
└── LICENSE.md
└── EXECUTE.md
└── README.md
