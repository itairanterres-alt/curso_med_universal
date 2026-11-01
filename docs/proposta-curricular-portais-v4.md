# Curso de Medicina em arquitetura de portais

**Documento de trabalho consolidado — versão 4**

| | |
|---|---|
| **Data** | 01/11/2026 |
| **Responsável** | Itairan da Silva Terres (Coordenação Adjunta do Curso de Medicina) |
| **Natureza** | Documento de trabalho para discussão no NDE. **Não aprovado.** Não substitui o PPC vigente |
| **Base normativa** | Resolução CNE/CES nº 3, de 30/09/2025 (DCN de Medicina) |
| **Histórico** | v1 (proposta inicial) → contraproposta externa (GPT) → v2 → revisão externa → v3 → análise do PPC Unidavi → descritivo real do Capi → **v4 (este documento)** |

---

## Sumário

0. [Como ler este documento](#0-como-ler-este-documento)
1. [Base normativa: o que a DCN 2025 exige](#1-base-normativa-o-que-a-dcn-2025-exige)
2. [O conceito: a operação de um parque temático aplicada ao currículo](#2-o-conceito-a-operação-de-um-parque-temático-aplicada-ao-currículo)
3. [Ponto de partida: o curso atual da Unidavi](#3-ponto-de-partida-o-curso-atual-da-unidavi)
4. [Arquitetura curricular](#4-arquitetura-curricular)
5. [Carga horária e internato](#5-carga-horária-e-internato)
6. [Fluxo, capacidade e filas virtuais](#6-fluxo-capacidade-e-filas-virtuais)
7. [Avaliação e progressão](#7-avaliação-e-progressão)
8. [Pessoas: mentoria, desenvolvimento docente e apoio ao estudante](#8-pessoas-mentoria-desenvolvimento-docente-e-apoio-ao-estudante)
9. [Hub e espaços físicos](#9-hub-e-espaços-físicos)
10. [Ecossistema digital: Mentor Web, Google Workspace e Capi](#10-ecossistema-digital-mentor-web-google-workspace-e-capi)
11. [Governança de dados e ética](#11-governança-de-dados-e-ética)
12. [Lacunas do curso atual frente à DCN 2025](#12-lacunas-do-curso-atual-frente-à-dcn-2025)
13. [Transição, cronograma e riscos](#13-transição-cronograma-e-riscos)
14. [Decisões para o NDE](#14-decisões-para-o-nde)
15. [Informações a confirmar](#15-informações-a-confirmar)
16. [Referências](#16-referências)
- [Anexo A — Checagem de conformidade com a DCN 2025](#anexo-a--checagem-de-conformidade-com-a-dcn-2025)
- [Anexo B — Correções incorporadas ao longo das versões](#anexo-b--correções-incorporadas-ao-longo-das-versões)

---

## 0. Como ler este documento

**Propósito.** Reunir num só lugar uma proposta inovadora de curso de Medicina, inspirada na engenharia operacional de grandes parques temáticos (fluxo, capacidade, portais, narrativa e feedback), e aproximá-la da realidade do curso da Unidavi: PPC, manuais docentes, laboratórios, rede de saúde de Rio do Sul e ecossistema digital (Mentor Web, Google Workspace e Capi).

**Dois níveis de leitura.**
- As **ideias do modelo** (seções 2, 4, 6 e 7) foram mantidas de propósito, mesmo quando vão além do que existe hoje. O objetivo do exercício foi trazer ideias novas.
- A **aproximação com a Unidavi** (seções 3, 5, 10, 12 e 13) mostra o que já existe, o que precisa ser adaptado e o que é preciso criar.

**Convenções.**
- ✔ atende · ⚠ decisão do NDE · 🔴 risco alto · 🟠 risco médio · 🟡 risco baixo.
- Números marcados como **(dado real)** vêm de documentos institucionais; os demais são **parâmetros de planejamento** a validar.

**Fontes consultadas para este documento.**

| Fonte | Leitura |
|---|---|
| Resolução CNE/CES nº 3/2025 | Integral |
| PPC do curso (versão de setembro de 2023, 277 p.) | Matriz curricular, internato e cenários (Quadros 5, 8, 9 e 10), sistema de avaliação, laboratórios, rede de saúde, apoio ao estudante, regime docente e histórico. **Não lidos:** ementário completo e regulamentos anexos |
| Manual Docente da 7ª fase (2026/2) | Estrutura, Comitê de Acompanhamento Acadêmico, anexos |
| Semana Padrão 2026/2 (1ª a 8ª fase) | Integral |
| Descritivo do sistema Capi MedUNIDAVI (01/11/2026) | Integral |
| Protótipo MED-UNIDAVI 2027, Diretriz Canônica do Dr. Capi, documentação do mini-curso de Dermatologia | Parcial |
| Manuais do internato e das demais fases | **Não lidos em detalhe** |
| Código do repositório do Capi | **Não lido** (sem acesso nesta sessão) |

---

## 1. Base normativa: o que a DCN 2025 exige

### 1.1 Perfil e competências
- **Perfil (Arts. 2º a 4º):** formação geral, crítica, reflexiva e ética; atuação em todos os níveis de atenção, nos setores público e privado; cuidado centrado na pessoa, família e comunidade; compromisso com o SUS.
- **Três áreas (Art. 6º):** Atenção, Gestão e Educação em Saúde.
- **27 competências (Art. 8º).** Agrupamento usado neste documento:

| Agrupamento | Incisos | Destaques novos em relação a 2014 |
|---|---|---|
| Cuidado integral e raciocínio clínico | I, II, III, VI, XX, XXI | Cuidados paliativos e terminalidade; APS como coordenadora do cuidado |
| Ética, direitos e diversidade | IV, V, XI, XXIII, XXIV | Populações vulnerabilizadas nominadas; dever de notificação |
| Comunicação e trabalho interprofissional | VIII, IX, XII, XXII, Art. 11 | Língua estrangeira recomendada; liderança colaborativa |
| Evidência, qualidade e segurança | X, XX, XXV | Avaliação de tecnologias por custo-efetividade |
| Saúde digital e dados | VII, VIII, XXVI, XXVII, Art. 10 | IA, telemedicina, aprendizado de máquina, Big Data, LGPD, documentação médica |
| Saúde planetária e crises | XIV, XV | Emergências sanitárias, desastres, mudanças climáticas, envelhecimento |
| Gestão e sistema | XVI, XVIII, XXV | Mercado de trabalho, saúde suplementar, uso racional de recursos |
| Educação e identidade profissional | XIII, XIX | Educação permanente; corresponsabilidade pela formação de outros |
| Autocuidado do médico | XVII | Competência do egresso, não apenas política institucional |

### 1.2 Parâmetros quantitativos

| Exigência | Artigo |
|---|---|
| Mínimo de **7.200 h**, presencial, períodos anuais ou semestrais | 13 |
| Internato com **≥ 35%** da carga total e **≥ 2 anos** | 32 |
| **≥ 30% do internato** em ambientes de **MFC e Urgência/Emergência do SUS**, com distribuição proporcional | 32, §2º |
| 70% restantes: **Clínica Médica, Cirurgia, GO, Pediatria e Saúde Mental**, englobando Saúde Coletiva, Medicina Intensiva e Traumato-Ortopedia | 32, §3º |
| Até **25%** do internato em instituição externa, **somente com residência credenciada pela CNRM** | 32, §1º |
| **5% a 15%** de carga teórica em cada área do internato | 34 |
| Plantões de até **12 h/dia**, limite de **40 h/semana** | 35 |
| Extensão curricularizada (Res. CNE/CES nº 7/2018: ≥ 10% da carga total) | 16 |

### 1.3 Princípios e estruturas obrigatórias
- Currículo **baseado em competências**, orientado pelas necessidades de saúde e pelos princípios do SUS; conteúdos derivados das competências (Art. 19).
- **Metodologias ativas**, integração curricular e interdisciplinaridade (Arts. 18 e 20).
- **Prática desde o início**, progressiva até o internato (Art. 31), nos três níveis de atenção (Art. 23).
- **Simulação é preparatória**; a prática em serviço deve **predominar** ao longo de todo o curso (Art. 24).
- Preceptoria **sempre supervisionada por docente da IES**; internato **integralmente supervisionado** por docentes (Arts. 25 e 32).
- Formação dos profissionais da rede (Art. 26).
- **NDE** (14), **NAPED** (21), política de **saúde do estudante** (27), **áreas verdes em todos os períodos, inclusive no internato** (28), **mentoria longitudinal** (29), **núcleo de inclusão e pertencimento** (30), acessibilidade e neurodiversidade (12).

### 1.4 Avaliação
- **Avaliação programática**, padronizada em todos os componentes, com dimensões formativa, somativa e diagnóstica e **feedback individual obrigatório e tempestivo** (Art. 36).
- **Avaliação somativa abrangente obrigatória imediatamente antes do internato** (Art. 36, parágrafo único).
- Três domínios: **cognitivo, psicomotor e atitudinal** (Art. 37).
- **Plano individualizado** em caso de baixo desempenho (Art. 37, §1º).

### 1.5 Prazos
- **Art. 39:** cursos em funcionamento têm 1 ano a partir da publicação (~01/10/2026) para aplicar a DCN às turmas que ingressarem depois disso.
- **Art. 38:** implantação integral em 4 anos (~10/2029).
- Segundo o ofício ABEM/ANUP (nov/2025), os alunos já matriculados permanecem no currículo de ingresso. Há tensão interpretativa entre os Arts. 38 e 39.

---

## 2. O conceito: a operação de um parque temático aplicada ao currículo

**Premissa.** O parque serve de modelo para a **operação** do curso (fluxo, capacidade, transições, sinalização, feedback), **não para o conteúdo**. Não há "brinquedos de médico". O conteúdo é medicina baseada em evidência, dentro da DCN.

| Mecânica do parque | Tradução no curso | Fundamento |
|---|---|---|
| Hub central que distribui para os mundos | **Hub de Integração**: o caso da semana nasce e fecha ali; os portais o aprofundam | Art. 20 |
| Mundos temáticos com portais de transição | **Portais permanentes** visitados ao longo de todo o curso, com peso que muda por etapa | Arts. 18–20 |
| Fila virtual e reserva de horário | **Agendamento por cotas** para simulação e prática deliberada | Art. 24 |
| Requisito de acesso à atração | **Pré-requisito de competência** para cenários de maior risco | Art. 8º, X e XX |
| Acesso prioritário | **Prioridade de agenda para quem está em plano de recuperação**, não para quem tem melhor nota | Art. 37, §1º |
| Centro de operações em tempo real | **Centro de Operações Acadêmicas (COA)** | Art. 36 |
| Narrativa contínua entre os mundos | **Município-Âncora**: cidade fictícia com famílias acompanhadas ao longo do curso | Art. 8º, VI |
| Áreas de descanso planejadas | **Áreas verdes** fixas na semana-padrão | Art. 28 |
| Atração parada → plano de contingência | **Reposição por equivalência documentada** quando um cenário suspende a atividade | Art. 36 |

**O que o modelo não usa:** ranking, placar, pontos ou troféus. O que se poderia chamar de "gamificação" é, aqui, **progressão por marcos de competência** (seção 7). Isso respeita também um princípio já adotado pelo Capi.

---

## 3. Ponto de partida: o curso atual da Unidavi

### 3.1 Estrutura vigente (PPC 2023) — dado real

- **12 fases semestrais**, ingresso semestral, cerca de **410 a 420 estudantes**.
- **Currículo integrado em três ciclos:** (1) ser humano saudável; (2) processos clínicos e manifestações das doenças; (3) internato.
- **Pré-internato (1ª a 8ª fase)**, por fase:
  - **3 UCs tutoriais temáticas** (ABP com tutorial de abertura e de fechamento, conferências e morfofuncional);
  - **Integração do Ensino em Saúde na Comunidade (IESC I–VIII)**, 80 h por fase, semanal, em UBS;
  - **Habilidades Profissionais (HP I–VIII)**: comunicação, habilidades clínicas, saúde digital, ambulatórios em subturmas a partir da 5ª/6ª fase, urgência e emergência na 7ª/8ª;
  - **Conhecimentos Gerais I–III** (Libras, saúde e ambiente, relações étnico-raciais, ética e bioética, empreendedorismo);
  - **Trabalho de Curso I–II** (7ª e 8ª fases).
- **Internato (9ª a 12ª fase), 4 × 720 h:** IX Saúde da Criança · X Saúde da Mulher · XI Clínica Cirúrgica (com até 180 h eletivas em instituição conveniada) · XII Clínica Médica 480 h + Saúde da Família e Comunidade 240 h. **18 semanas de 40 h.**

| Componente | Horas (dado real) |
|---|---|
| Componentes curriculares (1ª a 8ª fase) | 4.632 |
| Internato | 2.880 (35,86%) |
| TC e orientação | 160 |
| Atividades complementares | 360 |
| **Total** | **8.032** |
| Extensão curricularizada (contida no total) | 810 (10,08%) |

**Avaliação vigente:** conceitos S (Suficiente), PM (Precisa Melhorar) e I (Insuficiente); Exercício de Melhoria durante a fase; Exercício Final; dependência. Instrumentos: portfólio reflexivo, OSCE, avaliação de desempenho no internato, **Teste de Progresso anual** (120 itens, 1º ao 6º ano). **Comitê de Acompanhamento Acadêmico** por fase, com 2 encontros por semestre, já referenciado às competências da DCN 2025.

### 3.2 Infraestrutura — dado real

| Recurso | Descrição |
|---|---|
| **Núcleo de Práticas da Saúde** | 6.740 m², 4 pavimentos |
| Laboratórios básicos | Anatomia; integrado de bioquímica, biologia molecular e farmacologia; microscopia; fisiologia e biofísica; microbiologia e parasitologia; **2 morfofuncionais** (10 bancadas em U, plataforma multidisciplinar tridimensional) |
| **Laboratório de habilidades** | **12 consultórios** com áudio e comunicação com sala de capacitação |
| **Simulação clínica** | **5 simuladores de alta fidelidade** (adulto masculino e feminino, pediátrico, neonatal), 1 de RCP de média fidelidade, 3 de baixa; **unidade de internação simulada** com 5 leitos adultos e 2 pediátricos; sala de comando com vidro unidirecional; sala de debriefing; ambiente simulado de visita domiciliar |
| Habilidades cirúrgicas | Laboratório próprio |
| Informática | Laboratórios de informática e laboratório móvel |
| Salas de tutoria | ~10 salas observadas na Semana Padrão 2026/2 |
| **Casa do Ser / Dasein Haus** | Espaço de convivência aberto todos os dias, com horta, jardim, livros |

### 3.3 Rede de saúde de Rio do Sul — dado real (PPC)

- **16 UBS, todas com Estratégia Saúde da Família**, + 3 unidades de extensão; 2 equipes NASF.
- **CAPS**, Centro Municipal de Atenção à Saúde Mental, Centro de Atendimento à Mulher, Centro de Atendimento à Criança e ao Adolescente, Centro de Atendimento ao Adulto e Especialidades, CTA/IST, policlínica.
- **SAMU** (USB e USA) e **1 UPA 24 h**.
- **Hospital Regional Alto Vale** (190 leitos, incluindo UTI adulto, pediátrica e neonatal, UCIN e obstetrícia) e **Hospital Samária** (inclui leitos psiquiátricos). **328 leitos** nos dois hospitais.
- Gestores parceiros: Secretaria Municipal de Saúde e FUSAVI.

### 3.4 Semana Padrão 2026/2 — dado real

- Blocos de **110 minutos** (07:50–09:40, 10:00–11:50, 13:30–15:20, 15:40–17:30, 17:40–19:40, 19:50–21:50).
- **Áreas verdes já marcadas** em todas as fases.
- Turmas divididas em **TA e TB** para habilidades; **4 grupos tutoriais** por fase; **6 grupos de IESC**.
- **Habilidades em Saúde Digital** na 1ª e 2ª fases.
- Ambulatórios em subturmas a partir da 6ª fase (CAPS, geriatria, policlínica, UPA, endoscopia, especialidades).

### 3.5 Achado principal

**A Unidavi já tem cerca de 60% da proposta, com outros nomes.** Para este curso, a proposta não é uma ruptura de estrutura: é uma **camada de integração, fluxo e dados** sobre uma base que já funciona em ABP.

| Proposta | Já existe |
|---|---|
| Portais visitados toda semana | UCs tutoriais + IESC semanal + HP + morfofuncional + conferências |
| Caso-fio com abertura e fechamento | Situações-problema com tutorial de abertura e fechamento |
| Áreas verdes | Marcadas na Semana Padrão |
| Portal de saúde digital | Habilidades em Saúde Digital (1ª–2ª fase) |
| Comitê de competência | Comitê de Acompanhamento Acadêmico |
| Recuperação individualizada | Exercício de Melhoria e Exercício Final |
| Avaliação longitudinal externa | Teste de Progresso anual |
| Hub | Núcleo de Práticas da Saúde |
| Área verde física | Casa do Ser |
| Treino formativo, revisão espaçada, painel agregado | Capi (seção 10) |

---

## 4. Arquitetura curricular

### 4.1 Semestre por fora, unidades integradas por dentro
- O **semestre (fase)** continua sendo a estrutura administrativa: matrícula, financiamento, registro no Mentor Web.
- Dentro de cada fase do pré-internato: **4 Unidades Curriculares Integradas de cerca de 5 semanas**, cada uma com uma **pergunta central**, casos relacionados, objetivos por portal, atividades e supervisores discriminados, critérios de progressão e **recuperação prevista na própria programação**.
- **Progressão:** tempo fixo, com barreiras de competência entre Atos. Modelo de tempo totalmente variável foi descartado por inviabilidade regulatória e financeira.
- **Regimento:** aprovação por unidade; recuperação dentro do semestre; regra de dependência que não trave o semestre inteiro.
- Práticas longitudinais (IESC, famílias acompanhadas), extensão e mentoria atravessam as unidades, com horas contadas uma única vez.

### 4.2 Seis portais, uma linha transversal e um eixo de ciclos de vida

| Portal | Pergunta organizadora | Componentes atuais que o alimentam | O que muda |
|---|---|---|---|
| **BIOS** — Mecanismos | O que explica o funcionamento e o adoecimento do organismo? | UCs tutoriais, morfofuncional (**só da 1ª à 5ª fase**), conferências | Coordenação de portal. Da 6ª à 8ª fase, as ciências básicas são sustentadas por objetivos de mecanismo obrigatórios em cada situação-problema, conferências e minicursos do Capi |
| **TERRITÓRIO** — Pessoa, família e comunidade | Quem precisa de cuidado e em quais condições vive? | IESC I–VIII | Separar a **prática assistencial** da **extensão formal** |
| **CLÍNICA** — Investigação e decisão | Qual é o problema e que decisão faz sentido? | HP I–VIII (comunicação, clínicas, ambulatórios) | Ficha de rastreabilidade e APCs |
| **AGUDO** — Intervenção e cuidado crítico | O que fazer, com que prioridade e com que segurança? | HP VII–VIII (urgência e emergência), simulação de alta fidelidade, UPA, SAMU, UC Emergências | Antecipar suporte básico de vida e reconhecimento de gravidade para o Ato II |
| **CONTINUIDADE** — Recuperação, saúde mental, paliativos e transições | Como sustentar o cuidado depois da intervenção? | HP VI (CAPS, geriatria), Processo de Envelhecimento, Problemas Mentais e de Comportamento | **Dar identidade à Saúde Mental**, agora área obrigatória do internato |
| **SISTEMA** — Gestão, evidência e saúde digital | Como o sistema, os dados e as evidências moldam o cuidado? | Saúde Digital (1ª–2ª), Abrangência das Ações de Saúde, Empreendedorismo, TC I–II, política institucional de IA (em elaboração) | **Estender a saúde digital até a 8ª fase** (IA, dados, LGPD, telessaúde) |
| *Linha ETHOS* | *Que tipo de médico estou me tornando?* | Ética e Bioética (CG III), portfólio reflexivo, Libras, relações étnico-raciais | Atividade identificável em **todas as fases**, não só numa UC |
| *Eixo Ciclos de Vida* | *Criança · adolescente · mulher · adulto · idoso* | Distribuídos | **Matriz de cobertura obrigatória** em todos os portais |

**Alternativa aceitável (⚠ NDE):** cinco portais, com CONTINUIDADE incorporado a CLÍNICA, **desde que** exista uma **trilha obrigatória de Saúde Mental e Cuidados Paliativos** com coordenação própria, carga mínima por Ato e APCs específicas.

**Portal ≠ modalidade.** O portal diz **o quê** se aprende; a modalidade diz **onde e como** (serviço, fundamentos, simulação, integração). As horas são contadas **uma única vez, por modalidade**.

### 4.3 Gradiente de peso dos portais (metas de planejamento, tolerância de ±5 p.p.)

| Ato (fases) | BIOS | TERRIT. | CLÍNICA | AGUDO | CONTIN. | SISTEMA |
|---|---|---|---|---|---|---|
| I — Imersão (1ª–2ª) | 35 | 25 | 20 | 5 | 5 | 10 |
| II — Mecanismos (3ª–4ª) | 30 | 20 | 25 | 10 | 5 | 10 |
| III — Cuidado (5ª–6ª) | 15 | 20 | 30 | 10 | 15 | 10 |
| IV — Complexidade (7ª–8ª) | 10 | 15 | 25 | 25 | 15 | 10 |
| V — Internato (9ª–12ª) | Prática real nas áreas obrigatórias (seção 5) | | | | | |

Os percentuais são revistos quando a matriz de experiências for fechada. A unidade de controle continua sendo a **competência**.

### 4.4 Caso-fio e tarefa de transição

Um caso atravessa vários portais na mesma semana. Exemplo ("Dona Lurdes, 58 anos, poliúria e perda de peso"):

| Momento | Portal | Atividade |
|---|---|---|
| Abertura | Hub | Hipóteses e objetivos de aprendizagem |
| | BIOS | Insulina, glicotoxicidade, fisiologia renal da glicosúria |
| | TERRITÓRIO | Rastreamento e manejo de DM2 na UBS |
| | CLÍNICA | Exame do pé diabético; entrevista motivacional em consultório simulado |
| | SISTEMA | Base sintética de diabéticos do Município-Âncora; leitura crítica de ensaio clínico |
| Fechamento | Hub | Síntese, plano, dilema ETHOS (autonomia × adesão), feedback |

**Tarefa de transição** em toda passagem entre portais: *"O que você precisa explicar, verificar ou comunicar para dar continuidade ao cuidado?"* Treina, desde a 1ª fase, a passagem de caso estruturada.

**Requisito de fechamento** do caso longitudinal: explicar **o que aconteceu depois** da consulta, da intervenção ou da alta.

**Regra de consulta a fontes no ciclo tutorial:** UpToDate, Capi ou qualquer IA entram **depois** das hipóteses do grupo, nunca antes. Coerente com a vedação de IA nas provas individual e em equipe do TBL prevista na minuta de política de IA.

### 4.5 Município-Âncora

**O que é:** uma cidade fictícia com cerca de 12 famílias e uma rede de serviços, acompanhada pelo estudante ao longo do curso. As famílias nascem, adoecem, envelhecem e morrem, cobrindo naturalmente o ciclo de vida, os cuidados paliativos e a terminalidade (Art. 8º, I).

**Componentes:**
- **Histórias clínicas longitudinais** e casos complementares para garantir cobertura curricular.
- **Base de prontuários sintéticos** (gerada com ferramentas como o *Synthea* e adaptada à epidemiologia brasileira) para epidemiologia, gestão, pesquisa e IA, **sem dado real** (Art. 8º, VII e XXVI).
- **Calibração por indicadores públicos agregados** do Alto Vale do Itajaí (DATASUS, IBGE): DCNT, envelhecimento, arboviroses, leptospirose pós-enchente.

**Regras:**
- **Equipe editorial docente** mantém coerência clínica, cronológica e social. Cada episódio tem versão, objetivos, referências e gabarito pedagógico.
- **Revisão de diversidade e estereótipos** em cada episódio (Art. 8º, XI aplicado ao material didático): evitar, por exemplo, que pessoas negras ou LGBTQIAPN+ apareçam apenas em casos de violência ou IST.
- **O vínculo com pacientes reais é independente da história fictícia.** O estudante acompanha pessoas reais conforme as necessidades delas, a pactuação com a equipe e o consentimento. Não se procura paciente para "encaixar" no roteiro, nem se supõe que uma família real fique disponível por 6 anos.
- **Implantação gradual:** as situações-problema existentes (cerca de 14 por fase) são reescritas aos poucos dentro do universo comum de famílias, sem reescrever tudo de uma vez.
- **Suporte no Capi:** o módulo de Casos Clínicos Evolutivos (hoje carregado para o internato) é o embrião; ver seção 10.

### 4.6 Jornada em 5 Atos e ritos de passagem

| Ato | Identidade em construção | Rito de passagem |
|---|---|---|
| I — Imersão | Observador do cuidado | **Primeiro Território**: mapeamento do território e início do vínculo com a UBS de referência, após preparação e pactuação |
| II — Mecanismos | Investigador | Apresentação pública da investigação de um caso do Município-Âncora |
| III — Cuidado | Cuidador supervisionado | **Compromisso do Cuidado**: cerimônia antes do primeiro atendimento com responsabilidade parcial |
| IV — Complexidade | Decisor em formação | **Exercício de Crise** + avaliação pré-internato |
| V — Internato | Interno de Medicina | Entrada após a avaliação pré-internato; na saída, fechamento do caso longitudinal |

### 4.7 Experiências-âncora

| Âncora | Ato | Desenho | Competências |
|---|---|---|---|
| Primeiro Território | I | Inserção na UBS: mapa do território, determinantes sociais | VI, XI, XV |
| Laboratório do Município | II | Investigação de surto fictício com dados sintéticos | VII, X, XXI |
| Consultório Longitudinal | III | Acompanhamento supervisionado de pessoas reais, conforme a rede | II, III, XXIII |
| **Exercício de Crise: enchente no Alto Vale** | IV | Simulação interprofissional com SAMU e Defesa Civil: múltiplas vítimas, leptospirose, saúde mental pós-desastre, continuidade do cuidado de doentes crônicos | XIV, XV, IX |
| Projeto de Saúde Digital | IV | Desenvolvimento longitudinal de solução para necessidade pactuada com a rede; avaliado por compreensão do problema, segurança, utilidade e viabilidade. Pode ser apresentado na SAM | VII, XXV, XXVI |
| Avaliação pré-internato | IV→V | Prova cognitiva + OSCE + revisão de portfólio | Art. 36 |
| Cuidado até o fim | V | Cuidados paliativos supervisionados, com suporte emocional ao interno | I, XVII |

---

## 5. Carga horária e internato

### 5.1 Princípio
A Unidavi **não precisa reduzir** sua carga atual (8.032 h) para adotar o modelo. O modelo genérico de referência usa 7.680 h (4.800 pré-internato + 2.880 internato); para a Unidavi, a recomendação é **manter o total próximo do atual e redistribuir**.

**Regra:** qualquer hora acrescentada fora do internato (inclusive atividades complementares) aumenta o denominador do percentual do internato. Recalcular a cada mudança.

### 5.2 Contagem em hora-relógio (🟡 verificar)
O PPC registra que a matriz foi alterada de hora-aula para hora-relógio "sem que ocorresse a conversão". Os blocos da Semana Padrão têm 110 minutos (cerca de 3h40 por turno de dois blocos). O total de 8.032 h dá folga sobre as 7.200 h exigidas, mas **a conta precisa ser explícita no novo PPC**: horas de 60 minutos, intervalos fora da contagem.

### 5.3 Pré-internato: categorias de contabilização (referência)
Para o modelo de 4.800 h: **1.600 h em serviço e comunidade · 1.600 h de fundamentos e raciocínio integrado · 800 h de habilidades e simulação · 800 h de integração, pesquisa, avaliação e aprofundamento.** Na Unidavi, a mesma lógica deve ser aplicada às 4.632 h atuais para demonstrar o **predomínio da prática em serviço sobre a simulação** (Art. 24).

### 5.4 Extensão
- A extensão (≥ 10%) é **projeto formal com a comunidade**: interação dialógica, objetivos pactuados, acompanhamento e avaliação (Res. CNE/CES nº 7/2018).
- **Estar na UBS não é, por si só, extensão.** Separar no PPC a prática assistencial do IESC dos projetos extensionistas.
- Envolver **usuários do SUS e o conselho local de saúde** como coeducadores (paciente-parceiro), no codesenho dos projetos e na avaliação 360°.

### 5.5 Internato redistribuído (proposta para a Unidavi)
Mantém **4 × 720 h = 2.880 h** e a lógica de uma área-âncora por fase, que a rede e os preceptores já conhecem. MFC e U/E passam a ser distribuídas.

| Fase | Área-âncora | Componente MFC/U/E ou Saúde Mental | Total |
|---|---|---|---|
| **IX** | Pediatria 432 h | U/E pediátrica no SUS (PS/UPA) 144 h + MFC (puericultura na ESF) 144 h | 720 |
| **X** | GO 432 h | MFC (pré-natal e saúde da mulher na ESF) 288 h | 720 |
| **XI** | Cirurgia + Traumato-Ortopedia 432 h | U/E adulto (PS, UPA, SAMU) 288 h | 720 |
| **XII** | Clínica Médica + Medicina Intensiva 432 h | **Saúde Mental (CAPS, Hospital Samária, matriciamento) 288 h** | 720 |

| Área | Horas | % |
|---|---|---|
| MFC (SUS) | 432 | 15 |
| U/E (SUS) | 432 | 15 → **30% ✔** |
| Pediatria | 432 | 15 |
| GO | 432 | 15 |
| Cirurgia + Traumato-Ortopedia | 432 | 15 |
| Clínica Médica + Medicina Intensiva | 432 | 15 |
| **Saúde Mental** | 288 | **10 ✔** |
| Saúde Coletiva | Transversal, com objetivos e avaliação explícitos em MFC e U/E | — |

**Mudanças em relação ao atual:** Clínica Médica passa de 480 h para 432 h; Saúde da Família deixa de ser um bloco de 6 semanas e passa a ter presença em três fases; Saúde Mental ganha carga própria.

**Outras regras do internato:**
- **Teoria:** cerca de 10% em cada área (DCN: 5% a 15%).
- **Estágio externo:** até 720 h (25%), **somente em instituições com residência credenciada pela CNRM**. Verificar os convênios usados hoje nas 180 h eletivas da 11ª fase.
- **Áreas verdes no internato (⚠ NDE):**
  - (a) **20 semanas de 36 h** por fase, com calendário próprio do internato; ou
  - (b) manter 18 semanas e converter 4 h semanais em janela protegida, compensando a carga em outro ponto.
- **Ocupação média ponderada** com 160 internos: ~24 em cada área de 15% e ~16 em Saúde Mental. **Saúde Mental e a ocupação do HRAV (Pediatria e GO) são os gargalos prováveis.**

---

## 6. Fluxo, capacidade e filas virtuais

### 6.1 Princípios de capacidade
- **Capacidade de um cenário = menor valor entre capacidade física, capacidade de supervisão e oportunidades reais de participação.** Um ambulatório com 8 cadeiras pode comportar apenas 4 estudantes.
- **Vagas efetivas = soma das vagas seguras de cada sessão confirmada.** Verificar também a **variedade** de experiências: 40 vagas em atendimentos iguais não são 40 oportunidades de desenvolver todas as competências.
- **Ocupação-alvo de 75% a 85%.** Abaixo: ociosidade. Acima: filas e perda de margem para recuperação.

### 6.2 Grupos
- **Tutoria:** hoje 4 grupos de ~10 por fase. **Alternativa (⚠ NDE):** 5 grupos de 6 a 8. Com ~10 salas: 4 grupos ocupam ~64% das salas; 5 grupos, ~80% — **cabe nas salas, mas exige +8 tutores**.
- **Subgrupos de 3 a 4** em serviço, conforme a capacidade do cenário.
- **Simulação:** alternância explícita de papéis, com atuação individual observável.
- **Vínculos longitudinais não giram:** UBS de referência, equipe e famílias permanecem estáveis.

### 6.3 Circuito rotativo
Para experiências cuja ordem pode variar, rodízio em "quadrado latino" (cada grupo passa por cada estação uma vez, em ordem diferente):

| Encontro | Grupo A | Grupo B | Grupo C | Grupo D | Grupo E |
|---|---|---|---|---|---|
| 1 | Mecanismos | Tutoria | Simulação | Serviço | Evidências |
| 2 | Tutoria | Simulação | Serviço | Evidências | Mecanismos |
| 3 | Simulação | Serviço | Evidências | Mecanismos | Tutoria |
| 4 | Serviço | Evidências | Mecanismos | Tutoria | Simulação |
| 5 | Evidências | Mecanismos | Tutoria | Simulação | Serviço |

Preparação obrigatória e habilitação para uma tarefa **sempre antecedem** a execução; essas não giram.

### 6.4 Agenda única
- A agenda é calculada **para todas as turmas ao mesmo tempo** (salas, equipamentos, docentes, supervisores, deslocamentos, pré-requisitos), **incluindo as turmas do PPC antigo** durante a transição.
- O **contrafluxo** (fases ímpares e pares com grades espelhadas) serve como heurística de partida, não como solução.
- **Turno inteiro no campo** para cenários externos (o deslocamento não conta como carga horária).
- Ferramentas de montagem de grade com restrições (por exemplo, Google OR-Tools ou UniTime) podem gerar a melhor grade a partir das regras informadas.

### 6.5 Cotas e fila virtual

| Finalidade | Parcela inicial da capacidade |
|---|---|
| Atividades curriculares previamente agendadas | 65% |
| Recuperação e reavaliação (**faixa prioritária**) | 10% |
| Prática facultativa e aprofundamento | 10% |
| Reserva para contingências | 15% |

**Regras:**
1. A oferta obrigatória precisa caber na agenda **antes** de abrir reservas opcionais.
2. **Prioridade explicável:** necessidade pedagógica, prazo curricular e tempo de espera. O estudante vê por que recebeu a vaga, o que preparar e que evidência produzir. Ninguém disputa obrigação curricular pela velocidade no aplicativo.
3. **Falha de oferta da instituição é registrada separadamente de dificuldade de aprendizagem.** Quando a instituição não ofereceu a vaga, o problema não recai sobre o estudante.
4. **Requisito de acesso:** cenários de maior risco (procedimentos invasivos, plantão real na UPA) são liberados após o marco de competência correspondente. É regra de segurança do paciente.
5. **O recurso é escolhido pelo objetivo**, não por "nível tecnológico": comunicação pede paciente padronizado; procedimento pede treinador específico; coordenação de equipe pode justificar alta fidelidade.
6. **Reposição por equivalência documentada** (mesma competência, mesma natureza, mesmas horas). Exemplo: UPA suspende atividade → antecipar outra experiência prevista e reagendar; a pendência fica visível.
7. **Recuperação obrigatória tem horário curricular próprio.** Área verde não pode ser ocupada sistematicamente com obrigação.

**Implementação simples:** as **páginas de agendamento do Google Calendar** permitem que cada laboratório (12 consultórios, simulação, morfofuncional) tenha uma página de reserva. As cotas obrigatórias continuam na Semana Padrão. O Capi apenas mostra a pendência e o link (seção 10).

### 6.6 Números reais e fórmulas

| Recurso | Dado | Cálculo | Leitura |
|---|---|---|---|
| Salas de tutoria | ~10 salas | 4 grupos × 8 fases × 2 sessões = 64 de ~100 meios-turnos | 5 grupos: ~80% |
| Simulação | 1 unidade simulada, 5 simuladores de alta fidelidade | 8 turmas × 5 grupos × 3 h = 120 h de sala por semana → ≥ 4 salas | Alta fidelidade só para objetivos que dependem dela; o restante nos 12 consultórios |
| UBS | 16 UBS com ESF | Turnos-equipe = alunos × turnos por semana ÷ alunos por equipe. Ex.: 320 × 1,5 ÷ 3 = 160 turnos-equipe por semana | Somado ao internato (~24 internos em MFC). **Pactuar no COAPES** |
| OSCE | — | 10 estações de 10 min: 1 circuito avalia 10 alunos a cada 100 min → **40 alunos em 6h40**; 2 circuitos → 3h20 (recursos duplicados) | — |
| Horas-docente | Plano Individual de Trabalho (PIT) no Mentor Web | Demanda semanal = Σ(grupos × horas de contato × fator de preparo 1,3–1,5). Ex.: 40 grupos × 6 h × 1,3 = 312 h-docente/semana só em tutoria | Comparar com a soma dos regimes dos ~100 docentes |

### 6.7 Centro de Operações Acadêmicas (COA)
Função da **Secretaria de Apoio Pedagógico**, não do Capi.

| Horizonte | Trabalho |
|---|---|
| Semestral | Construir a agenda, verificar capacidade, reservar atividades obrigatórias |
| Semanal | Antecipar cancelamentos, acompanhar demandas, organizar recuperação |
| Diário | Confirmar funcionamento, resolver conflitos, registrar reposições |

O COA administra **oportunidades e recursos**. Decisões sobre aprendizagem e progressão ficam com docentes e colegiados.

**Indicadores do COA (cada um ligado a uma decisão):**

| Indicador | Decisão |
|---|---|
| Demanda × oferta de vagas por competência | Ampliar ou redistribuir capacidade |
| Tempo de espera para recuperação | Antecipar oportunidades |
| Oportunidades realizadas por estudante | Corrigir desigualdades entre grupos |
| Prazo de feedback | Ajustar carga e formação dos avaliadores |
| Cancelamentos e reposições pendentes | Rever estabilidade dos campos |
| Cumprimento das áreas verdes | Corrigir sobrecarga |
| Experiência de estudantes, preceptores e usuários | Rever qualidade e impacto no serviço |

---

## 7. Avaliação e progressão

### 7.1 Avaliação programática
- **Muitos pontos de dados de baixo peso; decisões de alto peso por colegiado.** O **Comitê de Acompanhamento Acadêmico** (já existente) é a instância de decisão.
- Os conceitos atuais (S/PM/I) e o Exercício de Melhoria são compatíveis com o modelo e podem ser mantidos.

| Domínio (Art. 37) | Instrumentos |
|---|---|
| Cognitivo | Prova de abertura do TBL, questões de aplicação, Teste de Progresso, simulados no padrão ENAMED |
| Psicomotor | Checklists em simulação, observação direta de procedimentos (DOPS), mini-CEX em cenário real, OSCE |
| Atitudinal | Avaliação 360° (paciente, equipe, pares), debriefing ETHOS, portfólio reflexivo |

### 7.2 Atividades Profissionais Confiáveis (APCs) — lista preliminar para o NDE
Construída a partir das 27 competências e das necessidades do SUS. As 13 EPAs da AAMC são referência, não modelo a copiar.

1. Realizar anamnese e exame físico adequados ao contexto.
2. Formular e priorizar diagnóstico diferencial.
3. Indicar e interpretar exames complementares.
4. Propor plano de cuidado, incluindo prescrição, para discussão com o supervisor.
5. Registrar em prontuário e elaborar documentos médicos (receita, atestado, notificação compulsória).
6. Apresentar caso clínico oralmente.
7. Comunicar uma transição de cuidado (passagem de caso, alta, referência).
8. Reconhecer deterioração clínica, iniciar o atendimento e pedir ajuda.
9. Realizar procedimentos gerais previstos para a etapa.
10. Conduzir conversa difícil e decisão compartilhada.
11. Acompanhar longitudinalmente uma família no território.
12. Avaliar criticamente evidências e usar tecnologias, inclusive IA, de forma ética.
13. Atuar em equipe interprofissional e participar da melhoria de um processo assistencial (segurança do paciente).

**Escala de confiança:** 1 — observa · 2 — executa com supervisor presente · 3 — executa com supervisor disponível de imediato. **Na graduação, o alvo máximo é o nível 3.** Níveis de supervisão indireta e de supervisão de outros pertencem à residência.

**A confiança é específica para tarefa, contexto e etapa.** Bom desempenho em simulação não libera a mesma tarefa com qualquer paciente.

**Estados da evidência no portfólio:** em desenvolvimento → demonstrado em simulação → demonstrado em prática real supervisionada → demonstrado de forma consistente em diferentes situações.

### 7.3 Feedback

| Momento | Devolutiva | Responsável |
|---|---|---|
| Durante tarefa com risco | Intervenção imediata | Supervisor |
| Após simulação ou atendimento observado | Comportamento observado, efeito, próximo passo | Docente ou preceptor |
| **Até 48 h** | Registro breve da observação e da orientação | Avaliador |
| Semanal | Revisão de pendências e agenda | Tutor |
| A cada unidade integrada | Síntese de evolução e plano seguinte | Mentor e equipe |

Exemplo de devolutiva útil: *"Você reuniu os achados relevantes, mas não explicitou quais exigiam prioridade. Na próxima atividade, comece pelos riscos identificados; essa parte será observada novamente."*

### 7.4 Decisões de progressão
- Regulamento do Comitê publicado com: competências mínimas por etapa, evidências necessárias, **critérios críticos de segurança e profissionalismo**, recuperação e reavaliação, fundamentação e possibilidade de revisão.
- **Requisitos essenciais não se compensam por média.** Evento grave de segurança ou profissionalismo permite interrupção imediata da atividade e análise própria.
- **Alerta não é sanção.** Antes de criar plano individual, o docente verifica: dificuldade de aprendizagem, falta de oportunidade, divergência entre avaliadores, necessidade de acessibilidade, sobrecarga.
- **Plano individual (Art. 37, §1º):** objetivo, responsável, oportunidades reservadas na faixa prioritária, prazo e critério de conclusão.

### 7.5 Avaliação somativa abrangente pré-internato (Art. 36, parágrafo único)
Ao fim da 8ª fase (fim do 4º ano):
- **Componente cognitivo:** os **Simulados UNIDAVI do 4º ano** (já existentes no Capi), alinhados à Matriz de Referência do ENAMED (Portaria Inep nº 478/2025). Para uso somativo, **correção no servidor**.
- **Componente de desempenho:** OSCE. O número de estações é definido pela confiabilidade desejada (literatura: 10 a 16 para decisão de alto peso).
- **Componente longitudinal:** revisão do portfólio e das APCs pelo Comitê.
- **Nota de corte defensável:** Angoff modificado (prova cognitiva) e regressão de casos limítrofes (OSCE).
- **Teste de Progresso** continua como calibração externa longitudinal.

### 7.6 Carga cognitiva
O calendário coordena as entregas entre docentes para **não concentrar avaliações decisivas** nem tarefas inéditas de alta exigência na mesma semana.

---

## 8. Pessoas: mentoria, desenvolvimento docente e apoio ao estudante

### 8.1 Casas (mentoria longitudinal — Art. 29)
- **8 Casas verticais**, cada uma com estudantes de todas as fases (~50 a 55 por Casa).
- **~5 mentores por Casa, ~40 mentores no total, 9 a 12 estudantes por mentor**, com **horas formalmente alocadas** no PIT. O mentor acompanha uma carteira estável, com substituição planejada.
- **Mentoria entre pares:** veteranos apoiam ingressantes, como atividade educacional supervisionada, sem responsabilidade assistencial (Art. 8º, XIX).
- A Casa é unidade de **pertencimento e bem-estar**, **sem competição por pontos**.
- **Nome:** "Casas" ou "Mentoria Longitudinal". **Não usar "Mentor"**, para não confundir com o Mentor Web nem com o papel "Mentor do erro" do Capi.
- **Acesso aos dados de desempenho:** ver seção 10.4.

### 8.2 NAPED (Art. 21)
Formalizar o núcleo a partir das ações atuais de educação permanente. Certificação em três trilhas **antes** de assumir a função:
1. **Tutor** (ABP, TBL, fechamento tutorial, feedback);
2. **Avaliador** (observação direta, OSCE, calibração entre avaliadores, nota de corte);
3. **Mentor** (escuta, plano de desenvolvimento, encaminhamento).

### 8.3 Formação de preceptores (Art. 26)
Programa conjunto com a Secretaria Municipal de Saúde e a FUSAVI, via COAPES:
- **O Capi oferece** trilhas e casos.
- **O NAPED cuida** da governança, da certificação e da calibração.

### 8.4 Apoio ao estudante e inclusão
- **Já existem:** SAPEM (apoio psicológico ao estudante de Medicina), apoio psicopedagógico, orientação pedagógica, NAI (acessibilidade), Casa do Ser.
- **A criar ou ampliar:** núcleo de inclusão e pertencimento que inclua diversidade étnico-racial, de gênero e orientação sexual (Art. 30), a partir do NAI.
- **Desenho Universal para a Aprendizagem nas estações (Art. 12):** guia prévio do que acontece em cada simulação (ruído de alarmes, estímulos), pré-briefing individual quando necessário, materiais em formatos múltiplos.
- **Informações de apoio psicológico ficam em fluxo confidencial próprio**, separado da avaliação acadêmica.

### 8.5 Educação interprofissional
Unidades compartilhadas com outros cursos da saúde da Unidavi (simulação de crise, portal CONTINUIDADE, território), se houver oferta.

---

## 9. Hub e espaços físicos

**O Núcleo de Práticas da Saúde é o Hub natural.**

| Zona | Função | Adaptação |
|---|---|---|
| Sala flexível de integração | Abertura e fechamento de caso, TBL com a Sessão de Questões do Capi, ritos de passagem | Uma sala para pelo menos uma turma, mobiliário móvel; ampliar se houver demanda justificada |
| Salas tutoriais | Tutoria por grupo, próximas à sala de integração | ~10 salas atuais |
| Laboratórios de habilidades e simulação | CLÍNICA e AGUDO | 12 consultórios + unidade simulada |
| Debriefing | Análise estruturada | Sala existente junto à simulação |
| Posto do COA | Agenda, conflitos, reposições | Integrado à Secretaria de Apoio Pedagógico |
| **Casa do Ser** | Área verde física, convivência das Casas | Já existe |
| Ambientes reservados | Apoio, acessibilidade, recuperação entre atividades | Separação acústica |

**Regras de desenho:**
- Arena de 80 a 120 lugares e distância máxima de 5 minutos entre espaços são **opções a testar**, não requisitos.
- O estudante pode ir **direto ao cenário externo**; orientação e registro não exigem passagem física pelo Hub.
- O investimento prioriza supervisão, acessibilidade, acústica e flexibilidade, não sofisticação tecnológica.

---

## 10. Ecossistema digital: Mentor Web, Google Workspace e Capi

### 10.1 Três camadas, cada dado com uma casa oficial

| Camada | Sistema | Papel |
|---|---|---|
| **Registro oficial** | **Mentor Web** | Matrícula, planos de ensino, conceitos finais, extensão, PIT docente |
| **Identidade e agenda** | **Google Workspace** | Login institucional, Calendar (Semana Padrão e páginas de reserva), Drive (manuais), Forms e Sheets, Meet |
| **Experiência e dados pedagógicos** | **Capi MedUNIDAVI** | Treino formativo, cards, simulados, sessões em sala, painéis agregados, minicursos, casos, simulação, avaliação e portfólio (piloto) |

### 10.2 O Capi hoje (descritivo de 01/11/2026)
- Site único com login Google institucional, **13 módulos (9 em uso)**, cerca de 400 alunos, professores e coordenação.
- **Princípios:** formativo, não classificatório (sem ranking, placar ou gamificação); a IA ajuda a pensar e não decide; evidência antes de eloquência; privacidade por padrão (nome ligado a desempenho só para a coordenação geral); regras de acesso garantidas no banco de dados.
- **Assistente com 6 papéis limitados** (ajuda de uso, mentor do erro, leitura da sessão, ajuda e material da SAM, cenário de simulação), teto de gasto diário, nada vira nota ou decisão sem uma pessoa.
- **Não é implantação oficial** da Unidavi nem está integrado aos sistemas institucionais.

### 10.3 Onde cada ideia encontra o Capi

| Ideia | Módulo de partida | O que falta |
|---|---|---|
| Caso-fio e Município-Âncora | Casos Clínicos Evolutivos (internato) + Simulação Clínica | Levar casos evolutivos ao pré-internato; cadastro comum de famílias no banco; situações-problema referenciando as famílias |
| TBL no Hub | Sessão de Questões (fases 4 a 8) | Modo individual → equipe para prova individual e em equipe |
| Feedback ao tutor sobre a turma | Leitura da Sessão | Estender ao fechamento tutorial (objetivos não sustentados pela turma) |
| Fila virtual | Início ("Agora") | Mostrar prática pendente com link para a página de reserva do Google Calendar. **O Capi não aloca** |
| Cadastro de cenários e capacidade | Pessoas e Turmas (lotação por fase, área e cenário) | Cenário como entidade: vagas seguras, supervisor, dias. Núcleo de dados do COA |
| Avaliação pré-internato | Simulados UNIDAVI do 4º ano | Somar OSCE e portfólio; correção no servidor para uso somativo |
| APCs, Comitê e portfólio | Avaliação e Portfólio (piloto com dados fictícios) | Validação pelo NDE e Colegiado; tabelas reais (ver 10.6) |
| Prática deliberada cognitiva | Meu Treino + Capi-Cards + Mentor do Erro | Já funciona |
| Rastreabilidade | Banco de itens marcado por SP, OA e DCN | Acrescentar **portal, modalidade, cenário e APC** às marcações |
| Cobertura curricular | Princípio "cobertura antes de saturação" | Aplicar à matriz de experiências, não só às questões |
| SISTEMA, pesquisa e extensão | SAM | Vitrine de projetos de extensão e de saúde digital |
| Indicadores de oferta | Painel de Desempenho | Indicadores do curso: vagas oferecidas × realizadas, espera, prazo de feedback |
| Lacuna de cenário | Minicursos (ECG, Dermatologia) | Modelo de "portal digital" para faltas de capacidade física, sem substituir prática obrigatória |

### 10.4 Tensões e como resolvê-las

**a) Mentoria × privacidade (a mais importante).** A proposta prevê que mentor e tutor vejam a trajetória dos seus alunos; a regra vigente do Capi restringe nomes ligados a desempenho à coordenação geral.
1. **Agora:** o **estudante compartilha o próprio painel** na mentoria, ou leva um resumo exportado por ele. Nenhuma regra muda.
2. **Depois da formalização da LGPD:** papel **mentor** com acesso restrito por regra de banco **apenas aos seus 9 a 12 mentorados**, com base legal e aprovação institucional.
3. **Nunca:** abrir nomes para todos os professores.

**b) "Gamificação".** O termo sai do PPC e do Capi. O conjunto passa a se chamar **progressão por marcos de competência** (requisito de acesso = segurança do paciente; microcertificação = nível de APC; mapa da jornada = portfólio).

**c) O nome "Mentor".** Mentor Web (sistema) · "Mentor do erro" (IA) · mentoria do Art. 29. Sugestão: mentoria institucional = **Casas**; papel da IA = **"Conversa sobre o erro"**.

**d) O Capi não é oficial.** Toda função **exigida pela DCN** precisa de **caminho oficial independente do Capi** (conceito no Mentor Web, ata do Comitê, OSCE com registro próprio). O Capi qualifica essas funções, mas não as sustenta sozinho até virar serviço institucional.

**e) Item com apoio de IA × julgamento por IA.** Item gerado com apoio de IA e **curado por humanos** pode compor avaliação somativa. Correção ou julgamento feito pela IA é **sempre formativo**.

### 10.5 Condições para o Capi sustentar funções oficiais
(do próprio descritivo)
- Contas de serviço institucionais, com mais de um responsável.
- Identidade ligada ao cadastro acadêmico (Mentor Web).
- LGPD formalizada: base legal, termo de uso, encarregado de dados, contratos com provedores de IA e hospedagem.
- Correção no servidor para qualquer uso em prova.
- **Responsável técnico institucional** (hoje uma pessoa decide e opera, com desenvolvimento apoiado por agentes de IA).
- Orçamento institucional para IA e hospedagem.

### 10.6 Sequência de encontro entre currículo e Capi
1. **NDE** define a lista de APCs (seção 7.2) e a escala de confiança.
2. **Colegiado** aprova o regulamento do Comitê e a avaliação pré-internato.
3. **LGPD formalizada** (pode correr em paralelo).
4. **Só então** o Capi cria as tabelas reais de APC e portfólio e o papel de mentor com acesso restrito.

---

## 11. Governança de dados e ética

**Dados permitidos (processo educacional):** reservas e presença em atividades; desempenho em avaliações formativas; observações de APC; prazo de feedback docente.

**Vedados:** reconhecimento facial de emoções; rastreamento contínuo de localização; monitoramento de redes sociais; ranking entre estudantes.

**Regras:**
- **Base legal identificada para cada tratamento.** Consentimento é uma das bases possíveis e não deve ser aplicado genericamente à gestão acadêmica.
- Acesso por função, registro de acessos, finalidade e prazo de retenção definidos.
- **Comitê de governança de dados acadêmicos com participação discente.**
- Alerta precoce sempre com **decisão humana**; nunca sanção automática.
- Alternativa acessível ao check-in digital.
- **Dados de pacientes nunca entram** em ferramentas de IA. Casos fictícios ou anonimizados (LGPD, art. 12). Vedação de fotos e capturas de prontuário.
- Presença, cliques e tempo de tela têm valor contextual limitado; engajamento se avalia por evidências de participação e aprendizagem.

O desenho **ensina pelo exemplo** o uso ético de dados e IA que a DCN exige do egresso (Art. 8º, VII, VIII e XXVI; Art. 10).

---

## 12. Lacunas do curso atual frente à DCN 2025

| # | Lacuna | Situação atual | Exigência | Risco |
|---|---|---|---|---|
| 1 | **MFC + U/E no internato** | 240 h explícitas de Saúde da Família (8,3%); U/E diluída nos rodízios | ≥ 30% (864 h) em ambientes de MFC e U/E do SUS (Art. 32, §2º) | 🔴 |
| 2 | **Saúde Mental no internato** | Dentro da 12ª fase, sem carga própria | Área obrigatória explícita (Art. 32, §3º) | 🔴 |
| 3 | **Áreas verdes no internato** | 40 h × 18 semanas | Inclusive no internato (Art. 28) | 🟠 |
| 4 | **Internato externo** | Até 180 h em conveniada à escolha | Até 25%, apenas com residência CNRM (Art. 32, §1º) | 🟠 verificar convênios |
| 5 | **Avaliação pré-internato** | TP e OSCE existem; sem barreira formal | Obrigatória (Art. 36, parágrafo único) | 🟠 |
| 6 | **Mentoria longitudinal** | Orientação por agendamento e SAPEM | Programa de mentoria ao longo do curso (Art. 29) | 🟠 |
| 7 | **NAPED** | Ações de educação permanente sem núcleo formal | NAPED ou equivalente (Art. 21) | 🟡 formalizar |
| 8 | **Inclusão e pertencimento** | NAI (acessibilidade) | Inclui diversidade (Art. 30) | 🟡 ampliar |
| 9 | **Hora-relógio** | Conversão não realizada segundo o PPC | Carga em hora-relógio | 🟡 verificar |
| 10 | **Saúde digital** | Só até a 2ª fase | Competências VII, XXVI e Art. 10 ao longo do curso | 🟡 |

**Já atende:** carga total (8.032 h), internato ≥ 35% (35,86%), extensão ≥ 10% (10,08%), áreas verdes no pré-internato, metodologias ativas, prática desde a 1ª fase (IESC), Comitê de Acompanhamento.

---

## 13. Transição, cronograma e riscos

### 13.1 Urgência
Pela leitura mais conservadora do Art. 39, **a turma de 2027/1 já deveria ingressar em PPC adequado à DCN 2025.** As turmas da 2ª à 12ª fase seguem o PPC de 2023: **dois currículos conviverão por cerca de 6 anos**, disputando os mesmos laboratórios, docentes e campos.

### 13.2 Três frentes

| Frente | Prazo | Conteúdo |
|---|---|---|
| **1. PPC 2027/1** | Antes do ingresso de 2027/1 | Nova arquitetura para a 1ª fase (impacto pequeno: a 1ª fase já tem áreas verdes, saúde digital e IESC); regimento das unidades integradas; regras de transição |
| **2. Internato para todas as turmas** | Até ~10/2029 (Art. 38) | Redistribuição MFC + U/E e Saúde Mental aplicada a todas as turmas por regra de transição. **Confirmar com assessoria jurídica e regulatória** à luz do ofício ABEM/ANUP |
| **3. Pré-internato** | Uma fase nova por semestre | Portais, APCs, Município-Âncora gradual, Casas, avaliação pré-internato quando a primeira turma nova chegar ao fim da 8ª fase |

**Piloto:** a primeira unidade integrada da primeira turma nova, com revisão a cada unidade de 5 semanas.

**Critério de expansão:** cada experiência obrigatória precisa ter **objetivo, vaga, supervisor, tempo, avaliação e recuperação assegurados** para todos os estudantes previstos.

### 13.3 Roteiro de implantação
1. **Inventário operacional:** salas, equipamentos, horas docentes (PIT), preceptoria, vagas por serviço, deslocamentos.
2. **Matriz de experiências completa** com ficha de rastreabilidade: competência DCN → objetivo da etapa → conhecimentos → atividade → cenário → supervisão → avaliação → carga horária → recuperação.
3. **Simulação da agenda** de todas as turmas, incluindo as do PPC antigo.
4. **Piloto** na primeira unidade da turma 2027/1.
5. **Revisão e expansão** gradual, com ajustes documentados.

### 13.4 Riscos principais

| Risco | Mitigação |
|---|---|
| Dois currículos disputando capacidade | Agenda única com todas as turmas |
| Rede sem vagas suficientes (Saúde Mental, HRAV) | Pactuação via COAPES antes de cada expansão |
| Docentes sem formação no modelo | Certificação pelo NAPED como pré-requisito |
| Sobrecarga de registros (portfólio, feedback) | Limite de volume; formulários curtos |
| Dependência do Capi para funções oficiais | Caminho oficial independente (seção 10.4 d) |
| Continuidade técnica do Capi (uma pessoa) | Responsável técnico institucional |

### 13.5 Avaliação do próprio currículo
Modelo **CIPP** (contexto, insumos, processo, produto), com coleta desde a primeira turma. Gera evidência para o NDE e produção científica (Arts. 16–17).

---

## 14. Decisões para o NDE

| # | Decisão | Opções |
|---|---|---|
| 1 | Número de portais | 6 portais (recomendado) · 5 portais + trilha obrigatória de Saúde Mental e Paliativos |
| 2 | Tamanho dos grupos tutoriais | 4 grupos de ~10 (atual) · 5 grupos de 6–8 (+8 tutores) |
| 3 | Distribuição do internato | Proposta da seção 5.5 · outra que atenda §2º e §3º |
| 4 | Áreas verdes no internato | 20 semanas × 36 h · 18 semanas com janela de 4 h e compensação |
| 5 | Eletivo no internato | Manter (via estágio externo com residência CNRM) · retirar |
| 6 | OSCE pré-internato | Número de estações e método de nota de corte |
| 7 | Lista de APCs e escala de confiança | Seção 7.2 como ponto de partida |
| 8 | Acesso de mentores a dados de desempenho | Compartilhamento pelo estudante (agora) · papel de mentor com acesso restrito (após LGPD) |
| 9 | Nomenclatura | "Casas" para a mentoria; "Conversa sobre o erro" para o papel de IA |
| 10 | Paciente virtual conversacional | Dentro do Capi, encenado como simulação · fora do ecossistema |

---

## 15. Informações a confirmar

1. Capacidade real de **Saúde Mental** (CAPS, Hospital Samária) para internos.
2. Instituições do internato externo com **residência credenciada pela CNRM**.
3. **Regime de trabalho** dos ~100 docentes (PIT no Mentor Web).
4. Conta de **hora-relógio** da matriz.
5. Número real de **salas de tutoria** e capacidade de cada cenário (inventário).
6. **Outros cursos da saúde** disponíveis para atividades interprofissionais.
7. Código atual do **Capi** (acesso de leitura ao repositório ainda não disponível nesta sessão).
8. Manuais do internato e das demais fases, para conferir o detalhamento atual de cada área.

---

## 16. Referências

- BRASIL. Conselho Nacional de Educação. Câmara de Educação Superior. **Resolução CNE/CES nº 3, de 30 de setembro de 2025.** Institui Diretrizes Curriculares Nacionais do Curso de Graduação em Medicina. DOU, 01/10/2025.
- BRASIL. CNE/CES. **Parecer CNE/CES nº 536/2025.**
- BRASIL. CNE/CES. **Resolução CNE/CES nº 7, de 18 de dezembro de 2018** (Extensão na Educação Superior).
- BRASIL. Inep. **Portaria nº 478/2025** (Matriz de Referência do ENAMED).
- ABEM; ANUP. **Ofício nº 132** — análise das DCN de Medicina (Arts. 38 e 39), nov. 2025.
- ABEM. **Caderno de orientações para implementação das DCN**, 2026.
- AAMC. **Core Entrustable Professional Activities for Entering Residency.**
- Synthea — Synthetic Patient Population Simulator (documentação).
- UNIDAVI. **Projeto Pedagógico do Curso de Medicina**, set. 2023.
- UNIDAVI. **Manual Docente — 7ª fase**, 2026/2; **Semana Padrão 2026/2**.
- Capi MedUNIDAVI. **Descritivo do sistema**, 01/11/2026.

---

## Anexo A — Checagem de conformidade com a DCN 2025

Situação de cada exigência em quatro níveis: **(1)** parâmetro atendido no desenho · **(2)** previsto no PPC · **(3)** capacidade confirmada · **(4)** funcionamento demonstrado.

| Exigência | Onde é atendida | Nível atual |
|---|---|---|
| ≥ 7.200 h, presencial (Art. 13) | 8.032 h | 2 (verificar hora-relógio) |
| Internato ≥ 35%, ≥ 2 anos (Art. 32) | 2.880 h (35,86%), 4 fases | 4 |
| ≥ 30% do internato em MFC + U/E SUS (§2º) | Seção 5.5 (30%) | 1 (proposto) |
| Saúde Mental no internato (§3º) | 288 h (seção 5.5) | 1 (confirmar cenário) |
| ≤ 25% externo com residência CNRM (§1º) | Até 720 h | 1 (verificar convênios) |
| Teoria de 5% a 15% por área (Art. 34) | ~10% | 1 |
| ≤ 12 h/dia, ≤ 40 h/semana (Art. 35) | 40 h atuais; proposta de 36 h | 2 |
| Prática desde o início, progressiva (Art. 31) | IESC desde a 1ª fase | 4 |
| Simulação preparatória, prática real predominante (Art. 24) | Seção 5.3 | 2 (demonstrar por modalidade) |
| Áreas verdes, inclusive no internato (Art. 28) | Pré-internato ✔; internato: seção 5.5 | 4 / 1 |
| Avaliação programática, 3 domínios, feedback (Arts. 36–37) | Seção 7 | 2 (parcial) |
| Avaliação pré-internato (Art. 36, parágrafo único) | Seção 7.5 | 1 |
| Plano individualizado (Art. 37, §1º) | Exercício de Melhoria + seção 7.4 | 2 |
| Mentoria longitudinal (Art. 29) | Casas (seção 8.1) | 1 |
| NAPED (Art. 21) | Seção 8.2 | 1 |
| Saúde do estudante (Art. 27) | SAPEM, apoio psicopedagógico, Casa do Ser | 4 |
| Inclusão e pertencimento (Art. 30) | NAI ampliado (seção 8.4) | 2 (parcial) |
| Formação dos profissionais da rede (Art. 26) | Seção 8.3 | 1 |
| Extensão ≥ 10% (Res. 7/2018) | 810 h (10,08%) | 4 (separar de assistência) |

---

## Anexo B — Correções incorporadas ao longo das versões

| Ponto | Versão anterior | Correção |
|---|---|---|
| Vazão da OSCE | "~60 alunos/hora" | **Erro de fator 10.** 1 circuito de 10 estações: 40 alunos em 6h40 |
| Fórmula de capacidade | Estações × alunos × turnos × 0,80 | Menor valor entre físico, supervisão e oportunidade |
| Margem do internato | 7.440 h com 35,5% | Margem maior (7.680 h no modelo genérico; 8.032 h na Unidavi) |
| Horas semanais do internato | 660 h em 20 semanas "a 36 h" | 660 ÷ 20 = 33 h; corrigido para 720 h = 36 h × 20 |
| Extensão | "Em TERRITÓRIO" | Presença na UBS não é extensão |
| Mentoria | ~96 mentores (1:5) | ~40 mentores (1:9–12), com horas alocadas |
| Áreas verdes | Fila virtual dentro da área verde; espaço físico como requisito | Recuperação obrigatória em horário curricular; espaço é melhoria |
| Contrafluxo | Solução | Heurística; agenda única de todas as turmas |
| "Nenhuma nota isolada reprova" | Regra absoluta | Eventos críticos de segurança e profissionalismo |
| Consentimento como base da LGPD | Genérico | Base legal por tratamento |
| Escada de fidelidade | Progressão tecnológica | Recurso escolhido pelo objetivo |
| Nível 5 de EPA | "Supervisiona outros" | Alvo máximo na graduação: nível 3 |
| "Espelho real" da família fictícia | Cada família fictícia com uma real | Vínculo real independente da narrativa |
| Ocupação no internato | ~20 por área | Ponderada pelas horas |
| Hub | Arena de 80–120 e 5 min como requisitos | Opções a testar |
| "Gamificação estrutural" | Termo usado | Progressão por marcos de competência |
| Contexto institucional | Premissas genéricas | Dados reais do PPC, Semana Padrão e Capi |
