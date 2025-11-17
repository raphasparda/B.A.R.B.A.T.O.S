<div>
<pre>
                                                                                                                  
                                                                                                :                 
                                                                                               t#,               .
.                               j.            .                                             ;##W.             ;W
Ef.                       ..    EW,           Ef.                       ..                 :#L:WE            f#E
E#Wi                     ;W,    E##j          E#Wi                     ;W,     ,;;L#K;;.   .KG  ,#D         .E#f 
E#K#D:                  j##,    E###D.        E#K#D:                  j##,        t#E      EE    ;#f       iWW;  
E#t,E#f.               G###,    E#jG#W;       E#t,E#f.               G###,        t#E     f#.     t#i     L##Lffi
SPARDA##Wt            :E####,    E#t t##f     E#WEE##Wt            :E####,        t#E     :#G     GK     tLLG##L 
E##Ei;;;;.          ;W#DG##,    E#t  :K#E:    E##Ei;;;;.          ;W#DG##,        t#E      ;#L   LW.       ,W#i  
E#DWWt             j###DW##,    E#SPARDA###i  E#DWWt             j###DW##,        t#E       t#f f#:       j#E.   
E#t f#K;          G##i,,G##,    E#f,t#Wi,,,   E#t f#K;          G##i,,G##,        t#E        f#D#;      .D#j     
E#Dfff##E,      :K#K:   L##,    E#t  ;#W:     E#SPARDA#E,      :K#K:   L##,       t#E         G#t      ,WK,      
jLLLLLLLLL; .j ;##D.    L##, .j DWi   ,KK: .j jLLLLLLLLL; .j ;##D.    L##, .j     fE  .j      t    .j EG.       
           ;f.,,,      .,,  ;f.           ;f.            ;f.,,,      .,,  ;f.     :  ;f.          ;f.,         
                                                                                                          
                ❏Binary Automated Reliability Bot for Analysis and Token-Oriented Serialization❐
</pre>
</div>

Sistema inteligente de análise de telemetria e logs utilizando IA generativa (Google Gemini) com arquitetura resiliente, compressão otimizada de tokens e observabilidade completa.

---

⊳⊳⊳ Descrição

B.A.R.B.A.T.O.S. é uma plataforma full-stack que automatiza a análise de logs e telemetria de sistemas complexos, reduzindo custos operacionais de 40% até 90% através de compressão inteligente de tokens (TOON Engine) e cache distribuído. O sistema utiliza Google Gemini para análise contextual, implementa padrões de resiliência (Circuit Breaker, Retry, Timeout) e oferece observabilidade completa via Grafana e Prometheus.

**Problema Resolvido:** Análise manual de logs consome tempo e recursos. B.A.R.B.A.T.O.S. automatiza este processo, fornecendo insights em tempo real com redução significativa de custos de API através de compressão e caching.

---

⊳⊳⊳ Tecnologias Utilizadas

- ❏Backend
- ⊳[Java 21](https://adoptium.net/temurin/releases/) (Eclipse Adoptium JDK)
- ⊳[Spring Boot 3.5.7](https://spring.io/projects/spring-boot) (Web, Security, Data JPA, WebFlux)
- ⊳[Resilience4j](https://resilience4j.readme.io/) (Circuit Breaker, Retry, Time Limiter)
- ⊳[Redis](https://redis.io/docs/) (Cache distribuído)
- ⊳[MongoDB Atlas](https://www.mongodb.com/docs/atlas/) (Persistência de telemetria)
- ⊳[H2 Database](https://www.h2database.com/html/main.html) (Autenticação e sessões)
- ⊳[JWT](https://jwt.io/introduction) (Autenticação stateless)
- ⊳[Micrometer](https://micrometer.io/docs) + [Prometheus](https://prometheus.io/docs/introduction/overview/) (Métricas)
- ⊳[Maven 3.x](https://maven.apache.org/guides/) (Build tool)

- ❏Frontend
- ⊳[React 19.2.0](https://react.dev/) (UI framework)
- ⊳[Vite 7.2.2](https://vite.dev/guide/) (Build tool e dev server)
- ⊳[React Router 7.9.6](https://reactrouter.com/en/main) (Roteamento SPA)
- ⊳[Tailwind CSS 3.4.17](https://tailwindcss.com/docs) (Estilização)
- ⊳[Axios](https://axios-http.com/docs/intro) (Cliente HTTP)

- ❏DevOps
- ⊳[Docker](https://docs.docker.com/) + [Docker Compose](https://docs.docker.com/compose/)** (Containerização)
- ⊳[GitHub Actions](https://docs.github.com/en/actions) (CI/CD)
- ⊳[Grafana](https://grafana.com/docs/grafana/latest/) (Dashboards e visualização)
- ⊳[Prometheus](https://prometheus.io/docs/introduction/overview/) (Coleta de métricas)
- ⊳[Nginx](https://nginx.org/en/docs/) (Servidor web para frontend)

- ❏Inteligência Artificial & Dados
- ⊳[LangChain4j 0.36.2](https://docs.langchain4j.dev/) (Integração Google Gemini)
- ⊳[TOON](https://github.com/toon-format/toon) (Token-Oriented Optimization Network/Notation)
---

> ❏Funcionalidades

⊳⊳ Core
- ⊳Análise inteligente de telemetria via Google Gemini (gemini-2.5-flash e gemini-2.5-PRO)
- ⊳Compressão TOON (Token-Oriented Optimization Network) com redução de até 70% no tamanho dos logs
- ⊳Cache Redis com TTL configurável (30 min padrão, redução de 40% em custos de API)
- ⊳Autenticação JWT com refresh tokens
- ⊳Rate limiting (10 requisições/minuto por cliente)

⊳⊳ Resiliência
- ⊳Circuit Breaker (Resilience4j) com 50% de threshold de falha
- ⊳Retry automático (3 tentativas com backoff exponencial)
- ⊳Timeout de 45 segundos por requisição
- ⊳Fallback para mensagens de erro padronizadas

⊳⊳ Observabilidade
- ⊳Métricas Prometheus (`/actuator/prometheus`)
- ⊳Dashboards Grafana pré-configurados (5 dashboards, 41 painéis)
- ⊳Alertas automatizados (10 regras de alerta)
- ⊳Tracing distribuído
- ⊳Health checks (`/actuator/health`)

⊳⊳ Segurança
- ⊳CORS configurável via variáveis de ambiente
- ⊳Sanitização de logs (remoção de informações sensíveis)
- ⊳Autenticação baseada em JWT
- ⊳Proteção contra força bruta via rate limiting

---

⊳⊳ Pré-requisitos para rodar localmente

- ⊳Java 21** (Eclipse Adoptium ou Oracle JDK)
- ⊳Maven 3.9+**
- ⊳Node.js 20+** e **npm 10+**
- ⊳Docker** e **Docker Compose** (É opcional, por que ninguém merece esse castigo chamado docker).
- ⊳Redis Server** (para cache distribuído)
- ⊳MongoDB Atlas**
- ⊳chave do Gemini:** https://aistudio.google.com/app/apikey

⊳⊳ Instalar Dependências

⊳⊳⊳ Backend
```bash
cd backend
mvn clean install -DskipTests
```

⊳⊳⊳ Frontend
```bash
cd frontend
npm install
```

⊳⊳⊳ Executar com Docker Compose (Recomendado mais eu não recomendo)

```bash
# Na raiz do projeto
docker-compose up --build
```

⊳⊳⊳URLs
Eu gosto de rodar a versão localnetwork por conta dos elementos do frontend.
---

⊳⊳ Roadmap 

⊳⊳⊳ Fase 1: Estabilização e Otimização (Q1 2025 ou 2026 kkkkkk)
- [x] Implementar arquitetura de resiliência (Circuit Breaker, Retry, Timeout)
- [x] Adicionar cache Redis com estratégia de invalidação
- [x] Refatorar LogController aplicando SOLID (InputValidator, ResponseBuilder)
- [x] Criar dashboards Grafana (5 dashboards, 41 painéis)
- [x] Modularizar frontend (9 componentes reutilizáveis)
- [x] Pipeline CI/CD com GitHub Actions
- [ ] Implementar rate limiting distribuído (Redis-based)
- [ ] Adicionar testes end-to-end (Playwright/Cypress)
- [ ] Otimizar algoritmo TOON para 80% de compressão

⊳⊳⊳ Fase 2: Escalabilidade e IA Avançada (Q2 2025 ou 2026 kkkkkk)
- [ ] Migrar para arquitetura de microserviços
- [ ] Implementar API Gateway (Spring Cloud Gateway)
- [ ] Adicionar suporte a múltiplos modelos de IA (ou pelo menos tentar)
- [ ] Sistema de treinamento de modelo personalizado
- [ ] Análise preditiva de falhas
- [ ] Auto-scaling baseado em carga (Kubernetes HPA)
- [ ] Implementar CQRS e Event Sourcing
- [ ] Implementar nova função de automação de pipelines

⊳⊳⊳ Fase 3: Features Enterprise (Q3 2025 ou 2026 kkkkkk)
- [ ] Multi-tenancy com isolamento de dados
- [ ] SSO via OAuth2 (Google, Microsoft, GitHub)
- [ ] Auditoria completa (logs de ações de usuários)
- [ ] Integração com ferramentas de ITSM (Jira, ServiceNow)
- [ ] Webhooks para notificações em tempo real
- [ ] Exportação de relatórios (PDF, Excel)
- [ ] API GraphQL complementar à REST

⊳⊳⊳ Fase 4: Inteligência de Negócio (Q4 2025 ou 2026 kkkkkk)
- [ ] Dashboard executivo com KPIs estratégicos
- [ ] Machine Learning para classificação automática de logs
- [ ] Detecção de anomalias com algoritmos não supervisionados
- [ ] Correlação de eventos multi-sistema
- [ ] Recomendações automáticas de otimização
- [ ] Integração com plataformas de APM (New Relic, Datadog)

⊳⊳⊳ Backlog Técnico
- [ ] Migrar de H2 para PostgreSQL em produção
- [ ] Implementar gRPC para comunicação interna
- [ ] Adicionar suporte a Kafka para streaming de eventos
- [ ] Criar SDK para integração com sistemas legados
- [ ] Implementar versionamento de API (v1, v2)
- [ ] Adicionar suporte a deployment Blue-Green
- [ ] Criar Helm Charts para Kubernetes

⊳⊳⊳ Melhorias Contínuas
- [ ] Aumentar cobertura de testes para 90%
- [ ] Reduzir tempo de build de CI/CD para < 5 minutos
- [ ] Documentar todas as APIs com OpenAPI 3.0
- [ ] Criar tutoriais em vídeo
- [ ] Tradução para inglês (i18n)
- [ ] Acessibilidade WCAG 2.1 AAA

---

</pre>
</td>
<td align="center" valign="center">
<pre>
  　　　　　　　　　　　　　　　　　　 　 　 　 ――i┐
　　　　　　　　　　　　　　　　　　　 　 　 /：rﾏ,.Ｙ＼
　　　　　　　　　　　　　 　 　 ＿_　Ｆｌ＿_〉’Y7ﾉ〉_　/７ 　 /￣ ＼
　　 　 　 　 　 　 　 　 　 　 / ／￣└一'´￣／./ ￣￣ //￣l＼|
　　　　　　　　　　 　 　 　 〈　l三|￣|　|三三l　〈 ＿＿ // ｢　 ＼l
　　　　　　 　 　 　 　 　 　 _〉 〉-|一|　|――ﾍ_∧__|　//　　　　｜
　　　　　　 　 　 　 　 　 ／ )/二|＿|_/￣＼/_/　　| _| |　　　　　〕
　　　　　　　　　 　 ／￣ /￣〉_/７ //￣〉７7､　　〔」_| |　　　 　 |        www.SPARDA.dev Tekkadan B.A.R.B.A.T.O.S. RAISE YOUR FLAG!
　　　 　 　 　 　 ／ ／) 〈＿/__/　/〈＿/ /// 〉　/　 | |　　　 　 |
　　 　 　 　 　 // .(／〈_＿_|＿|. 〈＿＿_//〈_/　〈―‐| |　　　 　 |
　　　　　< ＼// 　 ＿/　　 ＼ ＼_/　　　∨　 〆/＼| |　　　　 /
　　　　　　,>　_　<´/＼ / 　 / ￣　|　　　 |　　ヽ ＼/| |　　 　 /
　　　　 ／_／　＼/　　|､　ノ 　 　 ｜｢　￣|　　　￣　| |.　　　/
.　　 ／／　　　　｜　　|（(/）　　　 _| | ＿_ |_　 　 　 ｜￣＼/
　／／ 　 　 　 　 | 　 / 　 |　　　 〔_l |　 　 |_〕　 　 　 ￣＼/
く／　　　　　　　　〉､「　　丿 　 　 /　|　 　 | ヽ
　　　　　　　　　 /　 丶イ 　 　 　 |　 ヽ.　 /　 |
　 　 　 　 　 　 /　 /　 ｜　　　　｜　|　Ｌl　|　|
　　　 　 　 　 / ＼＿＿_〉　 　 　 ヽ、|　　　 ｌ丿
　　　　　　　 /＼/＿（(/）　　　　　　 |　　 　 ｌ
　　　　　　 /＼＿_／／　　　　　 　 _|　 　 　 l _
　　　 　 　 ＼/＿_／ 　 　 　 　 　 〔_||￣￣￣|_〕
　　　　　　　　　　　　　 　 　 　 　 　 ||ｰ――‐||
　　　　　　　　　　 　 　 　 　 　 　 　 |ヽ.＿＿ /|
　　　　　　　　　　 　 　 　 　 　 　 　 ∨＿＿_∨
</pre>
</td>

