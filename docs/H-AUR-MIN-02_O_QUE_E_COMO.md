# H-AUR-MIN-02 — O QUE E COMO

**Status:** hipótese funcional, operacional e arquitetural inicial
**Base:** evolui H-AUR-MIN-01 sem substituir ou declarar definitiva sua hipótese.
**Finalidade:** oferecer uma arquitetura suficientemente explícita para ser testada, refutada e refinada na Fase 2.

## Formulação de segundo patamar

> Aurelian recebe artefatos heterogêneos, interpreta seu conteúdo e status epistemológico, reconstrói o objeto de transformação e seu cenário, constrói e refina progressivamente uma representação contextual, avalia sua suficiência e consistência, explora e compara alternativas de agentificação, testa sua plausibilidade diante das evidências e restrições disponíveis e produz uma recomendação rastreável para decisão humana. Essas operações são iterativas: evidências, contradições ou lacunas podem levar à revisão de interpretações, reconstruções e representações anteriores.

H-AUR-MIN-02 não afirma que Aurelian já possui tais componentes nem que eles devem ser implementados exatamente como desenhados. Ela propõe uma hipótese arquitetural inicial para experimentação.

## Hipótese de arquitetura inicial

```text
                         AURELIAN
                            │
             ┌──────────────┴──────────────┐
             │                             │
             ▼                             ▼
      INPUT / ARTIFACT              REASONING / CONTROL
             │                             │
             ▼                             │
      INTERPRETATION                       │
             │                             │
             ▼                             │
      SCENARIO RECONSTRUCTION              │
             │                             │
             ▼                             │
      SEMANTIC REPRESENTATION ◄────────────┤
             │                             │
             ▼                             │
      CONTEXT / EVIDENCE                   │
             │                             │
             └──────────────┬──────────────┘
                            ▼
                  SCENARIO REASONER
                            │
             ┌──────────────┼──────────────┐
             ▼              ▼              ▼
         EVALUATOR      EXPLORER       COMPARATOR
             │              │              │
             └──────────────┼──────────────┘
                            ▼
                  AGENTIFICATION
                    RECOMMENDATION
                            │
                            ▼
                       HUMAN / HITL
                            │
                            ▼
                         DECISION
```

## Papéis hipotéticos

| Papel | Responsabilidade proposta | Não deve fazer sozinho |
| --- | --- | --- |
| Input / Artifact | receber, identificar e preservar proveniência | declarar o conteúdo como verdade |
| Interpretation | extrair alegações, conceitos e status epistemológico | decidir a transformação |
| Scenario Reconstruction | compor hipótese de cenário a partir dos fragmentos | ocultar lacunas ou conflitos |
| Semantic Representation | manter elementos, relações, evidências e incertezas | congelar uma ontologia definitiva |
| Context / Evidence | relacionar afirmações a fontes, tempo e condições | substituir análise crítica |
| Reasoning / Control | coordenar o ciclo, retornos e critérios de suficiência | assumir autoridade de governança |
| Scenario Reasoner | analisar o cenário e possibilidades de transformação | escolher uma alternativa sem evidência |
| Evaluator | avaliar coerência, suficiência, risco e adequação | transformar avaliação em decisão |
| Explorer | gerar alternativas condicionais | tratar alternativas como recomendações finais |
| Comparator | comparar alternativas por critérios explícitos | apagar alternativas inconvenientes |
| Recommendation | tornar a avaliação rastreável e acionável para HITL | implantar ou aprovar a mudança |

Os papéis podem se revelar capacidades de um mesmo componente, componentes separados ou uma modelagem inadequada. Essa indefinição é intencional nesta etapa.

## Núcleo de controle e rastreabilidade

O núcleo de raciocínio e controle deve preservar, para cada conclusão relevante:

- artefatos e versões usados;
- interpretações e inferências realizadas;
- evidências que sustentam e que contradizem a conclusão;
- representação do cenário adotada no momento da análise;
- critérios e alternativas avaliados;
- incertezas, lacunas e condições de validade;
- recomendação emitida e decisão humana posterior, se houver.

Esse registro permite que uma atualização posterior reveja uma conclusão sem apagar a trajetória que a produziu.

## Contrato de saída para HITL

A recomendação entregue ao decisor humano deve conter, no mínimo:

1. a pergunta e o recorte do cenário;
2. a representação relevante do cenário e suas limitações;
3. alternativas consideradas;
4. recomendação e nível de confiança justificado;
5. evidências, pressupostos e objeções relevantes;
6. riscos, restrições, controles e limites de autoridade;
7. validações ou experimentos ainda necessários;
8. decisão humana requerida.

## Aurelian Entry Framework — Prototype v0.1

**Status:** evolução aprovada para prototipação e teste na Fase 2.

Esta seção acrescenta uma camada de entrada e qualificação governada à hipótese anterior. Ela não substitui a formulação de segundo patamar, os papéis hipotéticos ou o contrato de saída já registrados. Ao contrário, estabelece como Aurelian constrói progressivamente uma base epistemicamente qualificada para exercer aqueles papéis e, eventualmente, produzir uma recomendação.

O Prototype v0.1 parte de uma premissa: Aurelian não é um receptor indiferenciado de documentos, dados ou pedidos. Ele conduz a qualificação daquilo que recebe, declara o que ainda precisa compreender, expõe sua compreensão provisória e só avança quando as condições do estágio correspondente são satisfeitas.

```text
INTENÇÃO DE ANALISAR
        │
        ▼
AURELIAN ENTRY FRAMEWORK
        │
        ▼
QUALIFICAÇÃO PROGRESSIVA DO CENÁRIO
        │
        ▼
VALIDAÇÃO CONSOLIDADA DE CENÁRIO E CONTEXTO
        │
        ▼
RACIOCÍNIO DE AGENTIFICAÇÃO
        │
        ▼
CONFIGURAÇÕES CANDIDATAS → RECOMENDAÇÃO → HITL
```

### Organização estrutural

A jornada é apresentada ao interlocutor por dois eixos complementares:

- **posição estrutural:** `PHASE` e, quando necessário, `SUBPHASE`;
- **posição global:** `STEP X/N`.

`X` informa o estágio corrente e `N` a quantidade total de passos na rota que está sendo percorrida. `N` não é universal nem necessariamente fixo desde o primeiro contato: a qualificação inicial pode determinar uma rota e, se novas evidências justificarem, a rota pode ser revisada. A mudança deve ser exposta e rastreada, nunca aplicada silenciosamente.

Exemplo de comunicação de progresso:

```text
PHASE 2/4 — Scenario Discovery
STEP 6/13 — Decisions & Authority
```

### STEP Loop

Um `STEP` não é meramente uma pergunta ou campo de formulário. É um estado mínimo de conhecimento que Aurelian busca alcançar para poder avançar responsavelmente.

```text
STEP X/N
   │
   ▼
ASK
   │
   ▼
ANSWER / ARTEFACT / EVIDENCE
   │
   ▼
INTERPRET
   │
   ├── identificar conteúdo, evidência, status epistemológico,
   │   ambiguidade, contradição e lacuna
   ▼
CLARIFY
   │
   ├── solicitar complemento, correção ou evidência quando necessário
   ▼
EXPOSE UNDERSTANDING
   │
   ├── apresentar ao interlocutor a compreensão provisória de Aurelian
   ▼
VALIDATE
   │
   ▼
GATE
```

O ciclo permite que Aurelian raciocine durante a qualificação; o que fica vedado antes dos gates necessários não é o raciocínio, mas a emissão de uma recomendação de agentificação como se já existisse cenário suficientemente qualificado.

### Gates e resultados possíveis

Todo `STEP` termina em um `GATE`: uma verificação explícita de suficiência, consistência, evidência, compreensão e validação para aquele estágio.

```text
GATE X
 ├── NEXT ASK   → a informação do mesmo STEP ainda precisa de esclarecimento;
 ├── NEXT STEP  → o conhecimento mínimo do STEP foi qualificado;
 ├── REROUTE    → a evidência alterou a rota, o escopo ou a progressão necessária;
 └── BLOCK      → não existe base suficiente para avançar responsavelmente.
```

`BLOCK` é um resultado legítimo: Aurelian pode concluir que, com os dados disponíveis, não há base para seguir ou recomendar agentificação. `REROUTE` também é uma operação governada: registra a rota anterior, a evidência que motivou a mudança, a nova rota e o impacto sobre `X/N`.

### PHASES, SUBPHASES e rotas

O protótipo organiza a jornada inicialmente nas fases abaixo. Elas são uma proposta para ser testada, e não uma taxonomia definitiva.

```text
PHASE 1 — INITIAL QUALIFICATION
│
├── STEP 1/N — Intent
├── STEP 2/N — Declared Object
└── STEP 3/N — Initial Boundary
        │
        ▼
   GATE — Entry Qualified
        │
        ▼
PHASE 2 — SCENARIO DISCOVERY
│
├── STEP 4/N — Current Operation
├── STEP 5/N — Actors & Capabilities
├── STEP 6/N — Decisions & Authority
├── STEP 7/N — Information, Data & Technology
└── STEP 8/N — Constraints, Rules & Evidence
        │
        ▼
   GATE — Scenario Reconstructed
        │
        ▼
PHASE 3 — CONTEXTUAL QUALIFICATION
│
├── STEP 9/N — Dependencies & Interactions
├── STEP 10/N — Performance & Expected Outcomes
└── STEP 11/N — Risks, Exceptions & Human Boundaries
        │
        ▼
   GATE — Context Qualified
        │
        ▼
PHASE 4 — CONSOLIDATION & VALIDATION
│
├── STEP 12/N — Gaps & Contradictions
└── STEP N/N — Scenario & Context Validation
```

Após a qualificação inicial, Aurelian determina a rota contextual apropriada. Rotas como atividade, departamento e corporação são exemplos de escala, não categorias aprovadas. Uma rota pode exigir subfases, passos adicionais ou uma reabertura de passo anterior; essa possibilidade é parte do protótipo.

### STEP N/N — validação consolidada de cenário e contexto

`STEP N/N` é a fronteira explícita entre qualificar o cenário e raciocinar sobre sua agentificação. Antes de atravessá-la, Aurelian apresenta a compreensão consolidada que construiu: objeto declarado e objeto qualificado, fronteira, operação atual, atores, capacidades, decisões, autoridade, dados, restrições, dependências, riscos, lacunas e contradições relevantes.

O interlocutor pode validar, corrigir ou declarar a compreensão incompleta.

```text
STEP N/N — SCENARIO & CONTEXT VALIDATION
        │
        ▼
COMPREENSÃO CONSOLIDADA EXPOSTA
        │
        ▼
HITL-A
 ├── VALIDATED  → atravessa a fronteira de qualificação;
 ├── CORRECT    → retorna para reconstrução ou STEP pertinente;
 └── INCOMPLETE → investiga lacunas, evidências ou rota adicional.
```

Regra do protótipo:

> Aurelian não atravessa a fronteira entre qualificação do cenário e raciocínio de agentificação sem expor sua compreensão consolidada de cenário e contexto e obter validação explícita do interlocutor.

### HITL-A e HITL-B

Os dois momentos de intervenção humana têm finalidades diferentes e não devem ser confundidos.

| Marco | Finalidade | Não autoriza |
| --- | --- | --- |
| **HITL-A** | validar ou corrigir a compreensão consolidada do cenário e do contexto | aprovar uma recomendação de agentificação |
| **HITL-B** | deliberar sobre a recomendação e as configurações candidatas produzidas após o raciocínio de agentificação | reescrever retroativamente a evidência ou a trajetória de qualificação |

```text
STEP N/N → HITL-A → AGENTIFICATION REASONING
                       │
                       ▼
             CANDIDATE CONFIGURATIONS
                       │
                       ▼
                RECOMMENDATION
                       │
                       ▼
                     HITL-B
                       │
                       ▼
                    DECISION
```

HITL-A valida a base de compreensão; HITL-B preserva a regra anterior de que Aurelian produz recomendação e o humano decide.

### Proposta inicial: STEP 1/N — Intent

`STEP 1/N — Intent` inicia a qualificação sem presumir que o interlocutor já conhece o objeto de transformação correto. Seu propósito é estabelecer por que a análise está sendo iniciada e que transformação, decisão ou entendimento se busca informar.

Informações mínimas propostas:

- intenção declarada do interlocutor ao acionar Aurelian;
- resultado ou decisão que a análise pretende informar;
- objeto, problema ou oportunidade inicialmente declarados;
- contexto e fronteira inicial conhecidos;
- artefatos, evidências ou fontes já disponíveis;
- urgências, restrições ou limites explicitamente conhecidos.

Aurelian deve devolver uma leitura provisória da intenção e separar o que foi declarado do que ainda é hipótese, ambiguidade ou lacuna. O gate do STEP 1 não declara um cenário qualificado: ele apenas verifica se há base suficiente para avançar à qualificação do objeto declarado e da fronteira inicial.

```text
INTENT DECLARED
      │
      ▼
AURELIAN EXPOSES ITS UNDERSTANDING
      │
      ▼
GATE — Intent Sufficient?
 ├── NEXT ASK / CLARIFY
 ├── NEXT STEP — Declared Object
 ├── REROUTE
 └── BLOCK
```

### Relação com o histórico conceitual

O Entry Framework não converte a representação de cenário em formulário fechado nem exige que todo cenário possua previamente o mesmo schema. Ele permite que a representação necessária seja descoberta progressivamente, preservando a hipótese anterior de que o objeto de transformação pode emergir e ser redefinido durante o raciocínio.

Assim, `Declared Object` permanece como ponto de entrada e `Qualified Object` como resultado provisório da qualificação, sempre relacionável às evidências, correções, rotas e gates que levaram a essa compreensão.

## Hipóteses que a Fase 2 deve testar

- interpretação, reconstrução e representação são capacidades separáveis?
- autoridade deve ser modelada como restrição contextual ou como elemento nuclear?
- o avaliador, explorador e comparador são papéis necessários e distintos?
- a representação precisa ser temporal, causal ou orientada a eventos?
- a qualidade da recomendação exige simulação, experimentação ou novas classes de evidência?
- quais limites de automação e supervisão emergem de cenários reais?

## Regra de evolução

Qualquer evolução desta arquitetura deve ser registrada como hipótese, evidência, recomendação e decisão humana quando aplicável. A arquitetura não pode ser alterada silenciosamente para fazer parecer que uma conclusão já era conhecida.
