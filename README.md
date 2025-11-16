->B.A.R.B.A.T.O.S.

---Binary Automated Reliability Bot for Analysis and Token-Oriented Serialization

Sistema inteligente de análise de telemetria e logs utilizando IA generativa (Google Gemini) com arquitetura resiliente, compressão otimizada de tokens e observabilidade completa.

---

## Descrição

B.A.R.B.A.T.O.S. é uma plataforma full-stack que automatiza a análise de logs e telemetria de sistemas complexos, reduzindo custos operacionais em 40% á 92% através de compressão inteligente de tokens (TOON Engine) e cache distribuído. O sistema utiliza Google Gemini para análise contextual, implementa padrões de resiliência (Circuit Breaker, Retry, Timeout) e oferece observabilidade completa via Grafana e Prometheus.

**Problema Resolvido:** Análise manual de logs consome tempo e recursos. B.A.R.B.A.T.O.S. automatiza este processo, fornecendo insights em tempo real com redução significativa de custos de API através de compressão e caching.

---

## Tecnologias Utilizadas

### Backend
- **Java 21** (Eclipse Adoptium JDK)
- **Spring Boot 3.5.7** (Web, Security, Data JPA, WebFlux)
- **LangChain4j 0.36.2** (Integração Google Gemini)
- **Resilience4j** (Circuit Breaker, Retry, Time Limiter)
- **Redis** (Cache distribuído)
- **MongoDB Atlas** (Persistência de telemetria)
- **H2 Database** (Autenticação e sessões)
- **JWT** (Autenticação stateless)
- **Micrometer + Prometheus** (Métricas)
- **Maven 3.x** (Build tool)

### Frontend
- **React 19.2.0** (UI framework)
- **Vite 7.2.2** (Build tool e dev server)
- **React Router 7.9.6** (Roteamento SPA)
- **Tailwind CSS 3.4.17** (Estilização)
- **Axios** (Cliente HTTP)

### DevOps
- **Docker + Docker Compose** (Containerização)
- **GitHub Actions** (CI/CD)
- **Grafana** (Dashboards e visualização)
- **Prometheus** (Coleta de métricas)
- **Nginx** (Servidor web para frontend)

---

## Funcionalidades

### Core
- Análise inteligente de telemetria via Google Gemini (gemini-2.5-flash e gemini-2.5-PRO)
- Compressão TOON (Token-Oriented Optimization Network) com redução de até 70% no tamanho dos logs
- Cache Redis com TTL configurável (30 min padrão, redução de 40% em custos de API)
- Autenticação JWT com refresh tokens
- Rate limiting (10 requisições/minuto por cliente)

### Resiliência
- Circuit Breaker (Resilience4j) com 50% de threshold de falha
- Retry automático (3 tentativas com backoff exponencial)
- Timeout de 45 segundos por requisição
- Fallback para mensagens de erro padronizadas

### Observabilidade
- Métricas Prometheus (`/actuator/prometheus`)
- Dashboards Grafana pré-configurados (5 dashboards, 41 painéis)
- Alertas automatizados (10 regras de alerta)
- Tracing distribuído
- Health checks (`/actuator/health`)

### Segurança
- CORS configurável via variáveis de ambiente
- Sanitização de logs (remoção de informações sensíveis)
- Autenticação baseada em JWT
- Proteção contra força bruta via rate limiting

---

### Pré-requisitos para rodar localmente

- **Java 21** (Eclipse Adoptium ou Oracle JDK)
- **Maven 3.9+**
- **Node.js 20+** e **npm 10+**
- **Docker** e **Docker Compose** (É opcional, por que ninguém merece esse castigo chamado docker).
- **Redis Server** (para cache distribuído)
- **MongoDB Atlas**
- **chave do Gemini:** https://aistudio.google.com/app/apikey

### Instalar Dependências

#### Backend
```bash
cd backend
mvn clean install -DskipTests
```

#### Frontend
```bash
cd frontend
npm install
```

### Executar com Docker Compose (Recomendado mais eu não recomendo)

```bash
# Na raiz do projeto
docker-compose up --build
```

**URLs:**
Eu gosto de rodar a versão localnetwork por conta dos elementos do frontend.
---

## Roadmap 

### Fase 1: Estabilização e Otimização (Q1 2025 ou 2026 kkkkkk)
- [x] Implementar arquitetura de resiliência (Circuit Breaker, Retry, Timeout)
- [x] Adicionar cache Redis com estratégia de invalidação
- [x] Refatorar LogController aplicando SOLID (InputValidator, ResponseBuilder)
- [x] Criar dashboards Grafana (5 dashboards, 41 painéis)
- [x] Modularizar frontend (9 componentes reutilizáveis)
- [x] Pipeline CI/CD com GitHub Actions
- [ ] Implementar rate limiting distribuído (Redis-based)
- [ ] Adicionar testes end-to-end (Playwright/Cypress)
- [ ] Otimizar algoritmo TOON para 80% de compressão

### Fase 2: Escalabilidade e IA Avançada (Q2 2025 ou 2026 kkkkkk)
- [ ] Migrar para arquitetura de microserviços
- [ ] Implementar API Gateway (Spring Cloud Gateway)
- [ ] Adicionar suporte a múltiplos modelos de IA (ou pelo menos tentar)
- [ ] Sistema de treinamento de modelo personalizado
- [ ] Análise preditiva de falhas
- [ ] Auto-scaling baseado em carga (Kubernetes HPA)
- [ ] Implementar CQRS e Event Sourcing
- [ ] Implementar nova função de automação de pipelines

### Fase 3: Features Enterprise (Q3 2025 ou 2026 kkkkkk)
- [ ] Multi-tenancy com isolamento de dados
- [ ] SSO via OAuth2 (Google, Microsoft, GitHub)
- [ ] Auditoria completa (logs de ações de usuários)
- [ ] Integração com ferramentas de ITSM (Jira, ServiceNow)
- [ ] Webhooks para notificações em tempo real
- [ ] Exportação de relatórios (PDF, Excel)
- [ ] API GraphQL complementar à REST

### Fase 4: Inteligência de Negócio (Q4 2025 ou 2026 kkkkkk)
- [ ] Dashboard executivo com KPIs estratégicos
- [ ] Machine Learning para classificação automática de logs
- [ ] Detecção de anomalias com algoritmos não supervisionados
- [ ] Correlação de eventos multi-sistema
- [ ] Recomendações automáticas de otimização
- [ ] Integração com plataformas de APM (New Relic, Datadog)

### Backlog Técnico
- [ ] Migrar de H2 para PostgreSQL em produção
- [ ] Implementar gRPC para comunicação interna
- [ ] Adicionar suporte a Kafka para streaming de eventos
- [ ] Criar SDK para integração com sistemas legados
- [ ] Implementar versionamento de API (v1, v2)
- [ ] Adicionar suporte a deployment Blue-Green
- [ ] Criar Helm Charts para Kubernetes

### Melhorias Contínuas
- [ ] Aumentar cobertura de testes para 90%
- [ ] Reduzir tempo de build de CI/CD para < 5 minutos
- [ ] Documentar todas as APIs com OpenAPI 3.0
- [ ] Criar tutoriais em vídeo
- [ ] Tradução para inglês (i18n)
- [ ] Acessibilidade WCAG 2.1 AAA

---

## Licença

Este projeto está licenciado sob a **MIT License**.

```
MIT License

Copyright (c)2025 www.SPARDA.dev Tekkadan B.A.R.B.A.T.O.S. Hub.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## Contato e Suporte

Só rezando e não me chama.

---

**Desenvolvido por www.SPARDA.dev Tekkadan B.A.R.B.A.T.O.S. Hub.
